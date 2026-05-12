---
title: Integrar o Adobe [!DNL Analytics] e o Customer Jornada [!DNL Analytics] ao tutorial da Experience [!DNL Platform] Edge
description: Saiba como integrar o Adobe [!DNL Analytics] ao Customer Jornada [!DNL Analytics] usando o AEP Web SDK, o AEP Mobile SDK ou a API do Edge Network Server.
solution: Customer Journey Analytics, Analytics
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
kt: null
thumbnail: 13728
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integração" type="positive"
exl-id: e39dac5d-6ad5-47c8-94e8-070011233161
TQID: https://experienceleague.adobe.com/ClZddWXeWp51gWTBjRDQBZ2xNiO1bTRq-AoAdmucNEg
product_v2: id: e55547f1-a1ff-40c6-8978-026e40ab7fa4id: e98b7246-966c-4318-9e95-cad2f7a17dc7
feature_v2: id: b3f03848-ae12-48b2-8aab-cad18567eb32id: e75a4a9c-d354-4ca4-9b02-1afeca73fa5eid: eb9732ab-8232-4b21-bc4c-89de86dbe4d7id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
subfeature_v2: id: e6c28e30-8689-4bf4-8fa8-561343d308a9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 413
ht-degree: 16%

---

# Integrar o Adobe [!DNL Analytics] e a Jornada do cliente [!DNL Analytics] ao tutorial do Edge da experiência [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=pt-BR#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crie esquemas</a> para os dados que serão assimilados.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Crie conjuntos de dados</a> para os dados que serão assimilados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configure as identidades e os namespaces de identidade corretos no esquema</a> para garantir que os dados assimilados possam se unir a um perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Habilitar os esquemas e conjuntos de dados para o perfil</a>.</li>
    <li>Assimile dados na Experiência [!DNL Platform] usando um destes métodos:</li>
        <ul>
            <li>Experimentar o Web SDK [!DNL Platform]:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Lista de verificação</a></li>
                </ul>
            <li>Experimentar o [!DNL Platform] Mobile SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Lista de verificação</a></li>
                </ul></li>
            <li>API do Edge Network Server:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><i>(Opcional)</i>. Se estiver usando vários conjuntos de dados, junte as IDs de pessoa para <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">gerar um conjunto de dados combinado</a>. Se estiver usando um único conjunto de dados do [!DNL Analytics] ou se existir um identificador comum em todos os conjuntos de dados que você planeja usar na Jornada do cliente [!DNL Analytics], ignore esta etapa.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Criar uma conexão</a> na Jornada do cliente [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">Criar uma visualização de dados</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">definir as configurações de componente</a> e <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">formatar métricas</a> na Jornada do cliente [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Crie um projeto na Jornada do cliente [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>As etapas de fluxo de trabalho padrão do conector de origem [!DNL Analytics] do Adobe criam o esquema e o conjunto de dados usados para assimilar os dados de [!DNL Analytics] &quot;no estado em que se encontram&quot;. Portanto, as duas primeiras etapas são tratadas pelo sistema. O fluxo de trabalho de mapeamento requer a criação de atributos personalizados; portanto, siga a sequência de etapas completamente.
