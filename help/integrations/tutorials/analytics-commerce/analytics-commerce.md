---
title: Tutorial Integrar [!DNL Analytics] com [!DNL Commerce] o
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
exl-id: ef50b6b3-1e2b-4fe9-98d5-555bc14ae8d6
source-git-commit: 46803595cf8e199e0c331ea8b82f7fe4a2afc801
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 0%

---

# Integrar [!DNL Analytics] a [!DNL Commerce]

## Integração inicial

Estas instruções são para projetos hospedados na nuvem do Adobe [!DNL Commerce]. A auto-hospedagem pode variar até certo ponto, mas o processo geral deve ser semelhante.

1. Verifique o código no seu ambiente local
1. Usar o compositor e o módulo de instalação
1. Siga as instruções individuais aqui e volte quando terminar as etapas restantes
   [Instalar e configurar o  [!DNL Platform] conector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html?lang=pt-BR){target="_blank"} da Experiência


1. Confirmar o composer.json e, se estiver na nuvem, os arquivos composer.lock
1. Verificar se o módulo está nos ambientes de preparo e/ou produção
Você pode fazer isso fazendo logon na seção de administrador do Adobe [!DNL Commerce] e procurando por essas novas seções em Sistema > Serviços
   ![Experiência [!DNL Platform] extensão do conector](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Configure o módulo com suas credenciais dentro do back office do Adobe [!DNL Commerce].
   * Primeiro, as configurações do Conector de serviços do [!DNL Commerce], conforme mostrado abaixo.

     Instalação do ![[!DNL Commerce] Services Connector](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * Em seguida, defina as configurações do conector da Experiência [!DNL Platform], conforme mostrado abaixo.

     ![Experiência [!DNL Platform] conector](./assets/analytics-commerce/experience-platform-connector.png)

Para obter mais detalhes sobre cada fase e etapa do processo de integração, siga as instruções na [Visão geral da experiência [!DNL Platform] do conector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html?lang=pt-BR){target="_blank"}. O tutorial do conector da Experiência [!DNL Platform] aborda cada seção detalhadamente e responde às suas perguntas. Use este tutorial para o resto das etapas de configuração rápida.

## Configuração da Experience Edge e do Adobe [!DNL Analytics]

1. Verifique se sua organização tem (e você tem) acesso ao Adobe [!DNL Analytics]. Isso pode ser confirmado indo até a [página inicial do Adobe Experience Cloud](https://experience.adobe.com/) e clicando no alternador de aplicativo (nove pontos) na navegação superior.

1. Crie um novo conjunto de relatórios no Adobe [!DNL Analytics] ou identifique a ID do conjunto de relatórios para a qual você enviará os dados de [!DNL Commerce]. Para obter mais informações, assista a um tutorial sobre [criação de um novo conjunto de relatórios](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html?lang=pt-BR). Você precisará dessa ID de conjunto de relatórios na etapa de sequência de dados abaixo.

1. Navegue até a [interface da Experiência [!DNL Platform] Adobe](https://platform.adobe.com) se tiver acesso à Experiência [!DNL Platform]. Se você não tiver acesso a essa interface, poderá executar todas as etapas necessárias listadas abaixo na [interface da Coleção de Dados](https://experience.adobe.com/#/data-collection) da Adobe Experience [!DNL Platform].

1. Crie ou atualize seu esquema XDM com grupos de campos específicos do [!DNL Commerce]. Para obter mais informações sobre como criar um esquema, consulte o tutorial [&quot;Criar esquemas&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html?lang=pt-BR).
   * Você precisará selecionar esse esquema entre as opções na etapa de fluxo de dados abaixo. Para criar um esquema, examine a coluna à esquerda em **Gerenciamento de dados** e localize **Esquemas**. Agora, na parte superior direita da interface, clique em **Criar esquema**. Selecione XDM ExperienceEvent.
   * Depois de criar um novo esquema, você adicionará os [!DNL Commerce] grupos de campos. No lado esquerdo da interface, encontre Grupos de campos e clique em **Adicionar**
      * Na pesquisa, você pode filtrar inserindo `ExperienceEvent Commerce`
      * Selecione o **Adobe [!DNL Analytics] ExperienceEvent[!DNL Commerce]** marcando a caixa
      * Clique em **Adicionar grupos de campos** na parte superior direita para salvar e continuar

1. Opcionalmente (e somente se você estiver na interface da Experiência [!DNL Platform]) - Criar um novo conjunto de dados
   * Esta etapa permite trazer os dados do [!DNL Commerce] para a Experiência [!DNL Platform] (separadamente dos dados do Adobe [!DNL Analytics]). Execute esta etapa se tiver acesso à Experiência [!DNL Platform] e estiver planejando usar os dados de [!DNL Commerce] nos aplicativos com suporte na Experiência [!DNL Platform], como Dados do Cliente em Tempo Real [!DNL Platform], Jornada do Cliente [!DNL Analytics] ou Journey Optimizer.
   * Você precisará selecionar esse conjunto de dados nas opções na etapa de fluxo de dados abaixo.
   * No cabeçalho da coluna à esquerda **Gerenciamento de dados** na navegação à esquerda, selecione **Conjuntos de dados**.
   * Clique em **Criar conjunto de dados** na parte superior direita. Escolha a opção **Criar conjunto de dados do esquema**.
   * Procure e use o esquema criado na última etapa

1. Criar a sequência de dados para enviar os dados [!DNL Commerce] para o Adobe [!DNL Analytics]
   * No cabeçalho **Coleção de dados**, na coluna à esquerda, selecione **Sequências de dados**.
   * Clique em **Nova Sequência de Dados** na parte superior direita da interface.
   * Forneça um nome e uma descrição opcional.
   * Localize e selecione o schema que você criou/identificou na etapa anterior.
   * Adicione as opções avançadas desejadas. Para obter mais informações sobre as opções avançadas, consulte a [documentação](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=pt-BR).
   * Clique em **Salvar** para continuar.
   * Clique em **Adicionar serviço** e escolha **Adobe[!DNL Analytics]** no campo suspenso.
   * Clique em **Adicionar conjunto de relatórios** e insira a ID do conjunto de relatórios que você criou/identificou em uma etapa anterior. Você pode adicionar mais de um conjunto de relatórios se quiser que os dados fluam para vários conjuntos de relatórios.
   * Como opção, e se você criou um conjunto de dados em uma etapa anterior, clique em **Adicionar serviço** novamente, escolhendo **Experiência Adobe[!DNL Platform]** no campo suspenso. No campo Conjunto de dados do evento, selecione o conjunto de dados criado anteriormente.
   * Salve a sequência de dados.

1. Finalmente, para visualizar seus dados do [!DNL Commerce], você precisará navegar até o Analysis Workspace no Adobe [!DNL Analytics], criar um projeto, escolher seu conjunto de relatórios e adicionar tabelas de forma livre e outras visualizações para relatar e analisar seus dados do [!DNL Commerce]. A imagem a seguir mostra um exemplo de uma tabela que você pode criar no Analysis Workspace.

   ![[!DNL Analytics] Captura de tela de alguns dados comerciais](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   Estes são alguns recursos adicionais para ajudar você a trabalhar no Analysis Workspace:

   * [Visão geral do Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html?lang=pt-BR)
   * [Criando um projeto do Workspace do zero](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html?lang=pt-BR)
   * [Usando Tabelas, Visualizações e Painéis no Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html?lang=pt-BR)
   * [Casos de uso de visualização](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html?lang=pt-BR)

   Além disso, há cursos gratuitos disponíveis no Experience League. Consulte [!DNL Analytics] cursos disponíveis [AQUI](https://experienceleague.adobe.com/pt-br?lang=en&amp;Solution=Analytics#courses).
