---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---


# Integrar o Adobe [!DNL Analytics] aos Dados do cliente em tempo real [!DNL Platform]

{{analytics-description}}

{{real-time-cdp-description}}

Integrar o Adobe [!DNL Analytics] com o Adobe Real-time Customer Data [!DNL Platform] (Real-Time CDP) pode oferecer vários benefícios para as empresas que buscam aprimorar suas experiências com os clientes e esforços de marketing. Estas são algumas das principais vantagens:

+ **Direcionamento e personalização aprimorados do público-alvo**: marketing preciso em dispositivos e canais, mensagens personalizadas para envolvimento otimizado.
+ **Otimização aprimorada da página de aterrissagem**: experiências personalizadas com base no dispositivo e no comportamento, melhorando a satisfação e a conversão do usuário.
+ **Ativação perfeita do público-alvo**: utilize perfis de clientes para um direcionamento eficaz por meio de canais preferenciais, fornecendo mensagens relevantes.

Ao combinar o Adobe [!DNL Analytics] e o Real-Time CDP, as empresas podem elevar seus esforços de marketing a um novo patamar, fornecendo experiências personalizadas, aumentando o engajamento do cliente e otimizando conversões em vários pontos de contato digitais.

<table>
    <thead>
        <tr>
            <th>aplicativos Experience Cloud</th>
            <th>Integra-se usando o</th>
            <th>Quando usar</th>
            <th>Casos de uso comuns</th>
        </tr>
    </thead>
    <tr>
        <td rowspan="2">[!DNL Analytics] com o Real-Time CDP</td>
        <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Experiência do conector de origem [!DNL Platform]</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Abordagem recomendada para clientes que já implementaram o Adobe [!DNL Analytics] e desejam a maneira mais rápida de assimilar esses dados na Experiência [!DNL Platform] para usar no Perfil do Cliente em Tempo Real.</li>
                <li>Quando a disponibilidade dos dados para o Perfil do cliente em tempo real puder estar entre 2 e 30 minutos a partir do momento da coleta de dados, e a disponibilidade para o Data Lake for de até 90 minutos.</li>
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
       <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-edge.md" target="_blank" rel="noreferrer">Experimentar o [!DNL Platform] Edge</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Abordagem recomendada para novas implementações do [!DNL Analytics] ou quando você deseja implementar uma estratégia de longo prazo.</li>
                <li>Envia dados diretamente de um dispositivo para a Experiência [!DNL Platform] usando o SDK da Web da AEP, o SDK móvel da AEP ou a API do servidor Edge Network.</li>
                <li>Clientes novos ou existentes que precisam da disponibilidade de dados do [!DNL Analytics] para o Perfil do cliente em tempo real para oferecer suporte a casos de uso de personalização da mesma página e da próxima página.</li>
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
</table>
