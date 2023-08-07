---
title: Integrar [!DNL Analytics] com [!DNL Commerce] tutorial
description: Saiba como integrar [!DNL Analytics] com [!DNL Commerce].
solution: Analytics, Commerce
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: null
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integração" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 5%

---


# Integrar [!DNL Analytics] com [!DNL Commerce]

## Integração inicial

Estas instruções são para o Adobe [!DNL Commerce] Projetos hospedados na nuvem. A auto-hospedagem pode variar até certo ponto, mas o processo geral deve ser semelhante.

1. Verifique o código no seu ambiente local
1. Usar o compositor e o módulo de instalação
1. Siga as instruções individuais aqui e volte quando terminar as etapas restantes
   [Instalar e configurar a experiência [!DNL Platform] conector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. Confirmar o composer.json e, se estiver na nuvem, os arquivos composer.lock
1. Verifique se o módulo está nos ambientes de preparo e/ou produção. Você pode fazer isso fazendo logon na seção de administrador do Adobe [!DNL Commerce] e procure essas novas seções em Sistema > Serviços
   ![Experiência [!DNL Platform] extensão do conector](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Configure o módulo com suas credenciais no Adobe [!DNL Commerce] back office.
   * Primeiro, o [!DNL Commerce] Configurações do conector de serviços, conforme mostrado abaixo.
     ![[!DNL Commerce] Instalação do Services Connector](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * Em seguida, a experiência [!DNL Platform] configurações do conector, conforme mostrado abaixo.
     ![Experiência [!DNL Platform] conector](./assets/analytics-commerce/experience-platform-connector.png)

Para obter mais detalhes sobre cada fase e etapa do processo de integração, siga as instruções no [Experiência [!DNL Platform] visão geral do conector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"}. A experiência [!DNL Platform] O tutorial do conector aborda cada seção em profundidade e responde a quaisquer perguntas que você possa ter. Use este tutorial para o resto das etapas de configuração rápida.

## Configuração do Experience Edge e do Adobe [!DNL Analytics]

1. Verifique se sua organização tem (e você tem) acesso ao Adobe [!DNL Analytics]. Isso pode ser confirmado acessando o [Página inicial do Adobe Experience Cloud](https://experience.adobe.com/) e clicando no alternador de aplicativos (nove pontos) na navegação superior.

1. Criar um novo conjunto de relatórios no Adobe [!DNL Analytics]ou identifique a ID do conjunto de relatórios que você enviará [!DNL Commerce] entrada de dados. Para obter mais informações, assista a um tutorial sobre [criação de um novo conjunto de relatórios](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html?lang=pt-BR). Você precisará dessa ID de conjunto de relatórios na etapa de sequência de dados abaixo.

1. Navegue até a [Adobe Experience [!DNL Platform] interface](https://platform.adobe.com) se você tiver acesso ao Experience Platform [!DNL Platform]. Se você não tiver acesso a essa interface, poderá executar todas as etapas necessárias listadas abaixo na Adobe Experience Platform [!DNL Platform] [Interface da coleção de dados](https://experience.adobe.com/#/data-collection).

1. Criar ou atualizar o esquema XDM com [!DNL Commerce]-grupos de campos específicos. Para obter mais informações sobre como criar um schema, consulte [&quot;Criar esquemas&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html?lang=pt-BR) tutorial.
   * Você precisará selecionar esse esquema entre as opções na etapa de fluxo de dados abaixo. Para criar um esquema, procure na coluna à esquerda em **Gerenciamento de dados** e localizar **Esquemas**. Agora, na parte superior direita da interface, clique em **Criar esquema**. Selecione XDM ExperienceEvent.
   * Depois de criar um novo schema, você adicionará o [!DNL Commerce] grupos de campos. No lado esquerdo da interface do usuário do, localize os Grupos de campos e clique em **Adicionar**
      * Na pesquisa, você pode filtrar inserindo `ExperienceEvent [!DNL Commerce]`
      * Selecione o **Adobe [!DNL Analytics] ExperienceEvent[!DNL Commerce]** marcando a caixa
      * Clique em **Adicionar grupos de campos** na parte superior direita para salvar e continuar

1. Opcionalmente (e somente se você estiver na [!DNL Platform] ) - Criar um novo conjunto de dados
   * Essa etapa permite trazer a [!DNL Commerce] na experiência [!DNL Platform] (separadamente de trazer os dados para o Adobe [!DNL Analytics]). Execute esta etapa se tiver acesso ao Experience Platform [!DNL Platform]e planejam usar o [!DNL Commerce] dados na experiência [!DNL Platform]aplicativos compatíveis com, como Real-Time Customer Data [!DNL Platform], Jornada ao cliente [!DNL Analytics]ou Journey Optimizer.
   * Você precisará selecionar esse conjunto de dados nas opções na etapa de fluxo de dados abaixo.
   * Abaixo da coluna à esquerda **Gerenciamento de dados** no cabeçalho da navegação à esquerda, selecione **Conjuntos de dados**.
   * Clique em **Criar conjunto de dados** no canto superior direito. Escolha o **Criar conjunto de dados a partir do esquema** opção.
   * Procure e use o esquema criado na última etapa

1. Criar a sequência de dados para enviar o [!DNL Commerce] dados para Adobe [!DNL Analytics]
   * No **Coleta de dados** na coluna à esquerda, selecione **Datastreams**.
   * Clique em **Nova sequência de dados** na parte superior direita da interface.
   * Forneça um nome e uma descrição opcional.
   * Localize e selecione o schema que você criou/identificou na etapa anterior.
   * Adicione as opções avançadas desejadas. Para obter mais informações sobre as opções avançadas, visite o [documentação](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=pt-BR).
   * Clique em **Salvar** para continuar.
   * Clique em **Adicionar serviço** e escolha **Adobe[!DNL Analytics]** no campo suspenso.
   * Clique em **Adicionar conjunto de relatórios** e insira a ID do conjunto de relatórios que você criou/identificou em uma etapa anterior. Você pode adicionar mais de um conjunto de relatórios se quiser que os dados fluam para vários conjuntos de relatórios.
   * Opcionalmente e se você tiver criado um conjunto de dados em uma etapa anterior, clique em **Adicionar serviço** novamente, escolhendo **Adobe Experience[!DNL Platform]** no campo suspenso. No campo Conjunto de dados do evento, selecione o conjunto de dados criado anteriormente.
   * Salve a sequência de dados.

1. Por fim, para visualizar suas [!DNL Commerce] dados, será necessário navegar até o Analysis Workspace no Adobe [!DNL Analytics], criar um projeto, escolher seu conjunto de relatórios e adicionar tabelas de forma livre e outras visualizações para relatar e analisar seu [!DNL Commerce] dados. A imagem a seguir mostra um exemplo de uma tabela que você pode criar no Analysis Workspace.

   ![[!DNL Analytics] Captura de tela de alguns dados comerciais](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   Estes são alguns recursos adicionais para ajudar você a trabalhar no Analysis Workspace:

   * [Visão geral do Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [Criação de um projeto do Espaço de trabalho do zero](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [Utilização de tabelas, visualizações e painéis no Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [Casos de uso de visualização](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   Além disso, há cursos gratuitos disponíveis no Experience League. Consulte [!DNL Analytics] cursos disponíveis [AQUI](https://experienceleague.adobe.com/?lang=en&amp;Solution=[!DNL Analytics]#courses).
