---
title: Integrar Adobe [!DNL Analytics] e Jornada do cliente [!DNL Analytics] com a experiência [!DNL Platform] Tutorial do Edge
description: Saiba como integrar o Adobe [!DNL Analytics] com a Jornada do cliente [!DNL Analytics] usando o SDK da Web da AEP, o SDK móvel da AEP ou a API do servidor da rede de borda.
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
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 21%

---


# Integrar Adobe [!DNL Analytics] e Jornada do cliente [!DNL Analytics] com a experiência [!DNL Platform] Tutorial do Edge

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=pt-BR#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crie esquemas</a> para os dados que serão assimilados.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Crie conjuntos de dados</a> para os dados que serão assimilados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configure as identidades e os namespaces de identidade corretos no esquema</a> para garantir que os dados assimilados possam se unir a um perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Ativar os esquemas e conjuntos de dados para o perfil</a>.</li>
    <li>Assimilar dados na Experience Cloud [!DNL Platform] usando um destes métodos:</li>
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
            <li>API do servidor da rede de borda:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><i>(Opcional)</i>. Se estiver usando vários conjuntos de dados, identifique as IDs de pessoa para <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">gerar um conjunto de dados combinado</a>. Se estiver usando uma única [!DNL Analytics] ou se existir um identificador comum em todos os conjuntos de dados que você planeja usar na Jornada do cliente [!DNL Analytics], ignore esta etapa.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer"></a>Criar uma conexão no Customer Journey [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">Criar uma visualização de dados</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">definir as configurações de componente</a>, e <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">formatar métricas</a> na Jornada do cliente [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html" _target="_blank" rel="noopener noreferrer">Criar um projeto na Jornada ao cliente [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>As etapas de fluxo de trabalho padrão para o Adobe [!DNL Analytics] conector de origem crie o esquema e o conjunto de dados usados para assimilar os dados do [!DNL Analytics] &quot;como está&quot;. Portanto, as duas primeiras etapas são tratadas pelo sistema. O fluxo de trabalho de mapeamento requer a criação de atributos personalizados; portanto, siga a sequência de etapas completamente.
