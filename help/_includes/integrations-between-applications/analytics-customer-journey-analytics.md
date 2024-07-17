---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---


# Integrar Adobe [!DNL Analytics] com Jornada do cliente [!DNL Analytics]

{{analytics-description}}

{{customer-journey-analytics-description}}

A integração do Adobe [!DNL Analytics] com a Jornada do cliente [!DNL Analytics] oferece os principais benefícios:

+ **Insights abrangentes** sobre comportamentos e preferências do cliente.
+ **Rastreamento ininterrupto entre canais** para obter uma exibição holística.
+ **Dados e relatórios unificados** para análise precisa.
+ **Personalização aprimorada** e melhor envolvimento com o cliente.
+ **Insights de dados em tempo real** para tomada de decisão ágil.

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
            <td rowspan="2">[!DNL Analytics] e Jornada do cliente [!DNL Analytics]</td>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Experiência do conector de origem [!DNL Platform]</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Abordagem recomendada para clientes que já implementaram o Adobe [!DNL Analytics] e desejam a maneira mais rápida de assimilar esses dados na Experiência [!DNL Platform] para usar na Jornada do Cliente [!DNL Analytics].</li>
                    <li>Quando a disponibilidade dos dados para o Perfil do cliente puder estar entre 2 e 30 minutos a partir do momento da coleta de dados, e a disponibilidade para o Data Lake for de até 90 minutos.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Fluxo de trabalho direto, iniciado pela interface do usuário.</li>
                    <li>Mapeamento da interface do usuário para copiar props e eVars de [!DNL Analytics] para novos campos XDM.</li>
                    <li>A maneira mais rápida de obter valor do Perfil do Cliente em Tempo Real e da Jornada do Cliente [!DNL Analytics].</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-edge.md" target="_blank" rel="noreferrer">Experimentar o [!DNL Platform] Edge</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Abordagem recomendada para novas implementações do [!DNL Analytics] ou quando você deseja implementar uma estratégia de longo prazo.</li>
                    <li>Envia dados diretamente de um dispositivo para a Experiência [!DNL Platform] usando o SDK da Web da AEP, o SDK móvel da AEP ou a API do servidor Edge Network.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Fornece o mais alto nível de controle para os dados coletados a serem usados no suporte aos seus casos de uso.</li>
                    <li>Os dados do lado do cliente são facilmente mapeados para campos XDM.</li>
                    <li>Disponibilidade de dados mais rápida para o Perfil do cliente em tempo real.</li>
                </ul>
            </td>
        </tr>  
    </tbody>          
</table>
