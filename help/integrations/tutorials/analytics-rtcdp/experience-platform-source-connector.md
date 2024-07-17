---
title: Integrar [!DNL Analytics] dados do cliente em tempo real [!DNL Platform] ao tutorial do conector de origem da Experiência [!DNL Platform]
description: Saiba como integrar o Adobe [!DNL Analytics] com Dados do cliente em tempo real [!DNL Platform] usando o conector de origem da Experience [!DNL Platform] .
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
exl-id: 1e27555d-e609-4a04-91ca-9518898ad699
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 2%

---

# Integrar o Adobe [!DNL Analytics] e os Dados do cliente em tempo real [!DNL Platform] ao conector de origem da experiência [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=pt-BR#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crie esquemas</a> para os dados que serão assimilados.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Crie conjuntos de dados</a> para os dados que serão assimilados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configure as identidades e os namespaces de identidade corretos no esquema</a> para garantir que os dados assimilados possam se unir a um perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">Habilitar os esquemas e conjuntos de dados para o perfil</a>.</li>
    <li>Assimilar dados de [!DNL Analytics] na Experience Platform usando o <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=pt-BR" _target="_blank" rel="noopener noreferrer">conector de origem do Adobe [!DNL Analytics]</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html" _target="_blank" rel="noopener noreferrer">Criar segmentos na Experiência [!DNL Platform].</a> O sistema determina automaticamente se o segmento é avaliado como lote (conector de dados) ou fluxo (rede Edge).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Configure destinos para o compartilhamento de atributos de perfil e associações de público-alvo com os destinos desejados.</a></li>   
</ol>

>[!NOTE]
>
>As etapas padrão do fluxo de trabalho para o conector de origem do Adobe [!DNL Analytics] criam o esquema e o conjunto de dados usados para assimilar os dados do [!DNL Analytics] &quot;no estado em que se encontram&quot;. Portanto, as duas primeiras etapas são tratadas pelo sistema. O fluxo de trabalho de mapeamento requer a criação de atributos personalizados; portanto, siga a sequência de etapas completamente.
