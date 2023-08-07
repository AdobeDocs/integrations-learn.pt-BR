---
title: Integrar [!DNL Analytics] e dados do cliente em tempo real [!DNL Platform] com experiência [!DNL Platform] tutorial do conector de origem
description: Saiba como integrar o Adobe [!DNL Analytics] com dados do cliente em tempo real [!DNL Platform] usar a experiência [!DNL Platform] conector de origem.
solution: Real-Time Customer Data [!DNL Platform], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integração" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 19%

---


# Integrar Adobe [!DNL Analytics] e dados do cliente em tempo real [!DNL Platform] com experiência [!DNL Platform] conector de origem

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=pt-BR#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crie esquemas</a> para os dados que serão assimilados.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Crie conjuntos de dados</a> para os dados que serão assimilados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configure as identidades e os namespaces de identidade corretos no esquema</a> para garantir que os dados assimilados possam se unir a um perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Ativar os esquemas e conjuntos de dados para o perfil</a>.</li>
    <li>Assimilar [!DNL Analytics] dados na Experience Platform usando o <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] conector de origem</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html" _target="_blank" rel="noopener noreferrer">Criar segmentos na Experience Cloud [!DNL Platform].</a> O sistema determina automaticamente se o segmento é avaliado como batch (conector de dados) ou streaming (rede de borda).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Configure destinos para o compartilhamento de atributos de perfil e associações de público-alvo com os destinos desejados.</a></li>   
</ol>

>[!NOTE]
>
>As etapas de fluxo de trabalho padrão para o Adobe [!DNL Analytics] conector de origem crie o esquema e o conjunto de dados usados para assimilar os dados do [!DNL Analytics] &quot;como está&quot;. Portanto, as duas primeiras etapas são tratadas pelo sistema. O fluxo de trabalho de mapeamento requer a criação de atributos personalizados; portanto, siga a sequência de etapas completamente.
