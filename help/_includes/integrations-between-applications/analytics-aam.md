---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---


# [!DNL Analytics] e integração de Audience Manager

{{analytics-description}}

{{audience-manager-description}}

Habilitar essa integração, encaminhando o Adobe [!DNL Analytics] do lado do servidor de dados para o Audience Manager, fornece ao Audience Manager uma de suas principais fontes de dados, ou seja, dados comportamentais de clientes online. Esses dados podem ser combinados com outros, como dados de CRM primários ou dados de parceiros de terceiros, para criar segmentos de clientes avançados. Além disso, os segmentos de Audience Manager são enviados de volta à página da Web na resposta para análise adicional do visitante. Ambos os casos de uso valiosos estão descritos abaixo.

Os principais benefícios da integração do Adobe [!DNL Analytics] e Audience Manager são:

+ **Segmentação aprimorada**: Combinar Adobe [!DNL Analytics] Dados de &amp; Audience Manager para segmentos de público precisos e personalizados em campanhas de marketing.
+ **Perfis de clientes unificados**: integre fontes de dados para entender as interações e os comportamentos, criando perfis abrangentes do cliente.
+ **Maior eficácia dos anúncios**: otimize anúncios com direcionamento orientado por dados do Adobe [!DNL Analytics] integração de &amp; Audience Manager.
+ **Decisões orientadas por dados**: informe opções por meio de insights detalhados, mesclando Adobe [!DNL Analytics] dados de &amp; Audience Manager.
+ **Experiências personalizadas**: personalize seu conteúdo e suas ofertas, enriquecendo as interações do cliente em pontos de contato usando ambas as plataformas.

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
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] envio de dados para o Audience Manager</a>
            </td>
            <td>Adobe [!DNL Analytics] extensão de tags ou AppMeasurement.js com o encaminhamento pelo lado do servidor ativado</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Quando quiser enviar o Adobe [!DNL Analytics] dados para o Audience Manager para criar segmentos que podem ser compartilhados com outros destinos do Adobe Experience Cloud, destinos com base em pessoas ou outros destinos personalizados e com base em dispositivos com suporte do Audience Manager.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Compartilhar segmentos em plataformas de anúncios que incluem atributos comportamentais coletados no [!DNL Analytics].</li>
                    <li>Enriquecer segmentos com [!DNL Analytics] dados para criar segmentos de alto valor entre canais para usar no direcionamento no site.</li>
                    <li>Camada em [!DNL Analytics] dados para segmentos desativados em identificadores com hash, como email, para uso em plataformas de redes sociais.</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html" target="_blank" rel="noreferrer">Audience Manager enviando dados de volta para [!DNL Analytics]</a>
            </td>
            <td>Adobe [!DNL Analytics] extensão de tags ou AppMeasurement.js com o encaminhamento pelo lado do servidor ativado</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Quando você deseja compartilhar segmentos do Audience Manager para o [!DNL Analytics] para informar a descoberta, a segmentação e a otimização de públicos-alvo.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Use segmentos de Audience Manager que incluem dados demográficos de provedores de terceiros no [!DNL Analytics] relatórios.</li>
                    <li>Use segmentos de Audience Manager que incluem dados de campanha de servidores de anúncios em [!DNL Analytics] relatórios.</li>
                    <li>Use segmentos de Audience Manager que incluem dados de CRM integrados no [!DNL Analytics] relatórios.</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
