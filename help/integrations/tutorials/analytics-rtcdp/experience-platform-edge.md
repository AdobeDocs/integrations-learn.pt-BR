---
title: Integre [!DNL Analytics] os Dados do cliente em tempo real [!DNL Platform] ao tutorial da Experience [!DNL Platform] Edge
description: Saiba como integrar o Adobe [!DNL Analytics] com Dados do cliente em tempo real [!DNL Platform] usando o SDK da Web da AEP, o SDK móvel da AEP ou a API do servidor Edge Network.
solution: Real-Time Customer Data [!DNL Platform], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
hidefromtoc: true
kt: 13732
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integração" type="positive"
exl-id: 07c2c329-0810-4f66-a91a-e315695f3fb4
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 3%

---

# Integrar o Adobe [!DNL Analytics] e o Real-Time Customer Data [!DNL Platform] ao tutorial do Experience [!DNL Platform] Edge

<ol>
    <li><a href="https://experienceleague.adobe.com/pt-br?lang=pt-BR#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crie esquemas</a> para os dados que serão assimilados.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Crie conjuntos de dados</a> para os dados que serão assimilados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Configure as identidades e os namespaces de identidade corretos no esquema</a> para garantir que os dados assimilados possam se unir a um perfil unificado.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Habilitar os esquemas e conjuntos de dados para o perfil</a>.</li>
    <li>Assimile dados na Experiência [!DNL Platform] usando um destes métodos:</li>
        <ul>
           <li>Experiência [!DNL Platform] SDK da Web:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Lista de verificação</a></li>
                </ul>
            <li>Experiência [!DNL Platform] SDK móvel:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Lista de verificação</a></li>
                </ul></li>
            <li>API do servidor Edge Network:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/segments/create-segments.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Criar segmentos na Experiência [!DNL Platform].</a> O sistema determina automaticamente se o segmento é avaliado como lote (conector de dados) ou fluxo (rede Edge).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Configure destinos para o compartilhamento de atributos de perfil e associações de público-alvo com os destinos desejados.</a></li>
</ol>

>[!NOTE]
>
>As etapas padrão do fluxo de trabalho para o conector de origem do Adobe [!DNL Analytics] criam o esquema e o conjunto de dados usados para assimilar os dados do [!DNL Analytics] &quot;no estado em que se encontram&quot;. Portanto, as duas primeiras etapas são tratadas pelo sistema. O fluxo de trabalho de mapeamento requer a criação de atributos personalizados; portanto, siga a sequência de etapas completamente.
