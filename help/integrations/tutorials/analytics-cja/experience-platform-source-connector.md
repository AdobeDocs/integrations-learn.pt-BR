---
title: Integrar o  [!DNL Analytics] e a Jornada ao cliente [!DNL Analytics] ao tutorial do conector de origem da Experiência [!DNL Platform]
description: Saiba como integrar o Adobe [!DNL Analytics] com o Customer Jornada [!DNL Analytics] usando o conector de origem da Experience [!DNL Platform] .
solution: Customer Journey [!DNL Analytics], [!DNL Target]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13727
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integração" type="positive"
exl-id: f0dbd59d-d5e5-40e6-b4a4-e4789e7dd7e3
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 2%

---

# Integrar o Adobe [!DNL Analytics] e a Jornada do cliente [!DNL Analytics] ao conector de origem da experiência [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/pt-br?lang=pt-BR#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crie esquemas</a> para os dados que serão assimilados.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Crie conjuntos de dados</a> para os dados que serão assimilados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Configure as identidades e os namespaces de identidade corretos no esquema</a> para garantir que os dados assimilados possam se unir a um perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Habilitar os esquemas e conjuntos de dados para o perfil</a>.</li>
    <li>Assimilar dados na Experiência [!DNL Platform] usando o <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">conector de origem do Adobe [!DNL Analytics]</a></li>
    <li><i>(Opcional)</i>. Se estiver usando vários conjuntos de dados, junte as IDs de pessoa para <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">gerar um conjunto de dados combinado</a>. Se estiver usando um único conjunto de dados do [!DNL Analytics] ou se existir um identificador comum em todos os conjuntos de dados que você planeja usar na Jornada do cliente [!DNL Analytics], ignore esta etapa.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Criar uma conexão</a> na Jornada do cliente [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Criar uma visualização de dados</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">definir as configurações de componente</a> e <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">formatar métricas</a> na Jornada do cliente [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Crie um projeto na Jornada do cliente [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>As etapas padrão do fluxo de trabalho para o conector de origem do Adobe [!DNL Analytics] criam o esquema e o conjunto de dados usados para assimilar os dados do [!DNL Analytics] &quot;no estado em que se encontram&quot;. Portanto, as duas primeiras etapas são tratadas pelo sistema. O fluxo de trabalho de mapeamento requer a criação de atributos personalizados; portanto, siga a sequência de etapas completamente.
