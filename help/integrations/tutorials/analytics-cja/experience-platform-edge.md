---
title: Integrar o Adobe [!DNL Analytics] e o Customer Jornada [!DNL Analytics] ao tutorial da Experience [!DNL Platform] Edge
description: Saiba como integrar o Adobe [!DNL Analytics] ao Customer Jornada [!DNL Analytics] usando o AEP Web SDK, o AEP Mobile SDK ou a API do Edge Network Server.
solution: Customer Journey [!DNL Analytics], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
hidefromtoc: true
kt: null
thumbnail: 13728
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integração" type="positive"
exl-id: e39dac5d-6ad5-47c8-94e8-070011233161
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 3%

---

# Integrar o Adobe [!DNL Analytics] e a Jornada do cliente [!DNL Analytics] ao tutorial do Edge da experiência [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=pt-BR#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crie esquemas</a> para os dados que serão assimilados.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Crie conjuntos de dados</a> para os dados que serão assimilados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configure as identidades e os namespaces de identidade corretos no esquema</a> para garantir que os dados assimilados possam se unir a um perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Habilitar os esquemas e conjuntos de dados para o perfil</a>.</li>
    <li>Assimile dados na Experiência [!DNL Platform] usando um destes métodos:</li>
        <ul>
            <li>Experiência [!DNL Platform] SDK da Web:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Lista de verificação</a></li>
                </ul>
            <li>Experiência [!DNL Platform] SDK móvel:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Lista de verificação</a></li>
                </ul></li>
            <li>API do servidor Edge Network:</li>
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
>As etapas padrão do fluxo de trabalho para o conector de origem do Adobe [!DNL Analytics] criam o esquema e o conjunto de dados usados para assimilar os dados do [!DNL Analytics] &quot;no estado em que se encontram&quot;. Portanto, as duas primeiras etapas são tratadas pelo sistema. O fluxo de trabalho de mapeamento requer a criação de atributos personalizados; portanto, siga a sequência de etapas completamente.
