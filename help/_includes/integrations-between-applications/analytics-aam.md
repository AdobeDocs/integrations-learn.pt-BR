---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# [!DNL Analytics] e integração com o Audience Manager

{{analytics-description}}

{{audience-manager-description}}

Habilitar essa integração, encaminhando dados do lado do servidor do Adobe [!DNL Analytics] para o Audience Manager, fornece ao Audience Manager uma de suas principais fontes de dados, ou seja, dados comportamentais online do cliente. Esses dados podem ser combinados com outros, como dados de CRM primários ou dados de parceiros de terceiros, para criar segmentos de clientes avançados. Além disso, os segmentos de Audience Manager são enviados de volta à página da Web na resposta para análise adicional do visitante. Ambos os casos de uso valiosos estão descritos abaixo.

Os principais benefícios da integração do Adobe [!DNL Analytics] e do Audience Manager são:

+ **Segmentação aprimorada**: combine dados de Adobe [!DNL Analytics] e Audience Manager para obter segmentos precisos e personalizados de público em campanhas de marketing.
+ **Perfis de clientes unificados**: integre fontes de dados para compreender interações e comportamentos, criando perfis de clientes abrangentes.
+ **Eficácia do anúncio aprimorada**: otimize anúncios com direcionamento orientado por dados da integração de Adobe [!DNL Analytics] e Audience Manager.
+ **Decisões orientadas por dados**: informe opções usando insights detalhados, mesclando Adobe [!DNL Analytics] e dados Audience Manager.
+ **Experiências personalizadas**: personalize seu conteúdo e ofertas, enriquecendo as interações do cliente em pontos de contato usando ambas as plataformas.

Em geral, essa integração reúne dados valiosos e insights do público-alvo. Ele permite que as empresas criem campanhas de marketing mais direcionadas e relevantes, ao mesmo tempo que obtêm uma compreensão mais profunda das preferências e comportamentos dos clientes.

## Integrações comuns

<table>
    <thead>
        <tr>
            <th>aplicativos Experience Cloud</th>
            <th>Integra-se usando o</th>
            <th>Quando usar</th>
            <th>Casos de uso comuns</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] enviando dados para Audience Manager</a>
            </td>
            <td>Extensão de tags do Adobe [!DNL Analytics] ou AppMeasurement.js com encaminhamento pelo lado do servidor ativado</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Quando quiser enviar dados de Adobe [!DNL Analytics] para o Audience Manager para criar segmentos que podem ser compartilhados com outros destinos da Adobe Experience Cloud, destinos com base em pessoas ou outros destinos com base em dispositivos e personalizados com suporte do Audience Manager.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Compartilhe segmentos com plataformas de publicidade que incluem atributos comportamentais coletados em [!DNL Analytics].</li>
                    <li>Enriqueça os segmentos com dados do [!DNL Analytics] para criar segmentos de alto valor entre canais para usar no direcionamento no site.</li>
                    <li>Camada nos dados [!DNL Analytics] para segmentos desativados em identificadores com hash, como email, para uso em plataformas de redes sociais.</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html?lang=pt-BR" target="_blank" rel="noreferrer">Audience Manager enviando dados de volta para [!DNL Analytics]</a>
            </td>
            <td>Extensão de tags do Adobe [!DNL Analytics] ou AppMeasurement.js com encaminhamento pelo lado do servidor ativado</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Quando quiser compartilhar segmentos do Audience Manager para o [!DNL Analytics] para informar a descoberta, a segmentação e a otimização de públicos-alvo.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Use segmentos Audience Manager que incluem dados demográficos de provedores de terceiros nos relatórios [!DNL Analytics].</li>
                    <li>Use segmentos de Audience Manager que incluem dados de campanha de servidores de anúncios em relatórios [!DNL Analytics].</li>
                    <li>Use segmentos de Audience Manager que incluem dados do CRM integrados nos relatórios [!DNL Analytics].</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
