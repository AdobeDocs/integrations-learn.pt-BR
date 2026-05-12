---
title: 'Integrar o  [!DNL Analytics] e a Jornada ao cliente [!DNL Analytics] ao tutorial do conector de origem da Experiência [!DNL Platform] '
description: Saiba como integrar o Adobe [!DNL Analytics] ao Customer Jornada [!DNL Analytics] usando o conector de origem da Experience [!DNL Platform] .
solution: Customer Journey Analytics, Target
feature: Integrations
topic: Integrations
role: Leader, Admin, Developer
level: Beginner
index: true
kt: 13727
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integração" type="positive"
exl-id: f0dbd59d-d5e5-40e6-b4a4-e4789e7dd7e3
TQID: https://experienceleague.adobe.com/o3HCX8vz8ZKn2j1Hl3W4XWMOudx7MBZCMNRWxO-eKbw
product_v2:
  - id: e43347a8-f2c5-4aa4-8623-6f13875d7e3a
  - id: e98b7246-966c-4318-9e95-cad2f7a17dc7
feature_v2:
  - id: e75a4a9c-d354-4ca4-9b02-1afeca73fa5e
  - id: f7c7de77-382f-4f48-8b36-61a170f06d3d
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 341
ht-degree: 19%

---

# Integrar o Adobe [!DNL Analytics] e a Jornada do cliente [!DNL Analytics] ao conector de origem da Experiência [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/pt-br?lang=pt-BR#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crie esquemas</a> para os dados que serão assimilados.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Crie conjuntos de dados</a> para os dados que serão assimilados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Configure as identidades e os namespaces de identidade corretos no esquema</a> para garantir que os dados assimilados possam se unir a um perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Habilitar os esquemas e conjuntos de dados para o perfil</a>.</li>
    <li>Assimilar dados na Experiência [!DNL Platform] usando o <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Conector de origem do Adobe [!DNL Analytics]</a></li>
    <li><i>(Opcional)</i>. Se estiver usando vários conjuntos de dados, junte as IDs de pessoa para <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">gerar um conjunto de dados combinado</a>. Se estiver usando um único conjunto de dados do [!DNL Analytics] ou se existir um identificador comum em todos os conjuntos de dados que você planeja usar na Jornada do cliente [!DNL Analytics], ignore esta etapa.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Criar uma conexão</a> na Jornada do cliente [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Criar uma visualização de dados</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">definir as configurações de componente</a> e <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">formatar métricas</a> na Jornada do cliente [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Crie um projeto na Jornada do cliente [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>As etapas de fluxo de trabalho padrão do conector de origem [!DNL Analytics] do Adobe criam o esquema e o conjunto de dados usados para assimilar os dados de [!DNL Analytics] &quot;no estado em que se encontram&quot;. Portanto, as duas primeiras etapas são tratadas pelo sistema. O fluxo de trabalho de mapeamento requer a criação de atributos personalizados; portanto, siga a sequência de etapas completamente.
