---
title: Integrações de aplicativos para personalização em escala
description: Torne as experiências personalizadas parte de cada momento.
exl-id: 6d18813d-950c-40ae-8d5b-80bf389358fc
source-git-commit: 509b227f360718e81fb19d3a4d30aebf9de49e5a
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# Personalization em escala

No cenário altamente competitivo e orientado por tecnologias digitais atual, os clientes acabaram esperando experiências personalizadas de acordo com suas preferências e necessidades exclusivas. Aproveitar os recursos do Adobe Experience Cloud nos permite coletar e analisar dados abrangentes do cliente, fornecendo insights inestimáveis sobre comportamentos, interesses e preferências. Essa compreensão profunda facilita a entrega de experiências personalizadas em vários pontos de contato, garantindo interações significativas e envolventes. Aproveitar o potencial do Adobe Experience Cloud libera todo o potencial de personalização, promovendo conexões mais fortes com o cliente, incentivando a fidelidade e impulsionando o crescimento dos negócios.

<table>
 <thead>
    <tr>
      <th>Caso de uso</th>
      <th>Descrição</th>
      <th>Exemplos</th>
      <th>Aplicativos</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Criar documentos personalizados do PDF</strong></td>
      <td>
        Gerar documentos de comunicação para assinatura com base no usuário
        seleções/preferências.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Apresentar um NDA gerado dinamicamente com base nos dados de um AEM
            Envio do Forms para assinatura
          </li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-acrobat-sign.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Forms e Sign</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>Análise de dados e relatórios</strong></td>
      <td>
        Analisar dados comportamentais de experiências digitais <br />Usar Adobe
        [!DNL Analytics] dados comportamentais no Analysis Workspace na Jornada do cliente
        [!DNL Analytics].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Analisar caminhos de conversão de cima/baixo</li>
          <li>Analisar o engajamento e a conversão do canal</li>
          <li>Entender o conteúdo visualizado principal</li>
          <li>Entender as principais categorias e produtos</li>
          <li>
            Realizar análise de uso da ferramenta para otimizar as experiências de autoatendimento
          </li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-customer-journey-analytics.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] e Jornada do cliente [!DNL Analytics]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Relatórios para atividades de personalização<br />Otimização de análise
        resultados de testes, incluindo testes A/B, utilizando o Adobe [!DNL Target] e
        gerando relatórios abrangentes por meio do Adobe [!DNL Analytics].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Mostrar resultados do teste A/B em relatórios de análise avançada</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] e [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>Personalizar entregas de email</strong></td>
      <td>
        Personalize deliveries de email com conteúdo dinâmico aproveitando o
        recursos do Adobe [!DNL Target].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Adicionar ofertas personalizadas a emails de clientes</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/campaign//campaign-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Campaign] e [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2">
        <strong>Expandir públicos para plataformas de personalização e publicidade</strong>
      </td>
      <td>
        Use segmentos Audience Manager para criar públicos-alvo no Real-Time CDP para
        uso em táticas de personalização e re-marketing.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Executar direcionamento e personalização de público-alvo digital anônimo no
            site, aplicativo móvel ou nos canais de publicidade suportados
          </li>
          <li>
            Otimizar experiências de página de aterrissagem e pré-autenticação com base em
            características de dispositivo e comportamento conhecidas
          </li>
          <li>
            Aproveite a rede de dados de terceiros do Audience Manager para
            refinar e expandir seus públicos para direcionamento
          </li>
          <li>Compartilhar segmentos de Audience Manager para a RTCDP</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/aam/aam-rtcdp.md"
          target="_blank"
          rel="noopener noreferrer"
          >Dados do Audience Manager e do cliente em tempo real [!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Use dados do [!DNL Analytics] para criar públicos-alvo a serem usados na personalização ou
        táticas de re-marketing.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Realizar o direcionamento e a personalização de público-alvo digital em dispositivos ou
            canais de publicidade suportados.
          </li>
          <li>
            Otimizar páginas de aterrissagem conhecidas do cliente e experiências anônimas
            com base em atributos de dispositivo e comportamentais.
          </li>
          <li>Ative públicos para canais conhecidos, como email e SMS.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-customer-journey-analytics.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] e dados do cliente em tempo real [!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>Personalizar experiências da Web</strong></td>
      <td>
        Personalize experiências de aplicativo de página única (SPA) com eficiência
        utilizando AEM Headless em conjunto com o Adobe [!DNL Target].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalização de SPA e aplicativo móvel</li>
          <li>Respostas da API personalizadas.</li>
          <li>[!DNL Target]Enviar entrega de conteúdo.</li>
          <li>Variações do teste A/B.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Headless e [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Ofereça experiências de site personalizadas utilizando o AEM Sites de maneira eficiente
        e Adobe [!DNL Target] para personalização.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalização do site do AEM.</li>
          <li>Personalizar o conteúdo do site.</li>
          <li>Otimize as experiências do usuário.</li>
          <li>Variações do teste A/B.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Sites e [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>Personalizar experiências digitais</strong></td>
      <td>
        Usar Perfis de clientes em tempo real e [!DNL Platform] segmentos gerenciados centralmente
        para personalizar mensagens na web, dispositivos móveis e outros canais digitais
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalização de conteúdo para visitantes conhecidos</li>
          <li>Aumentar a inscrição e a participação no programa de fidelidade</li>
          <li>Identificar e envolver clientes em risco de churn</li>
          <li>Personalização de oferta em tempo real</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/rtcdp/rtcdp-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >Dados do cliente em tempo real [!DNL Platform] e [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>Aprimorar a geração de clientes potenciais</strong></td>
      <td>
        Usar Perfis de clientes em tempo real e [!DNL Platform] segmentos gerenciados centralmente
        para personalizar mensagens na web, dispositivos móveis e outros canais digitais
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalização de conteúdo para visitantes conhecidos</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/rtcdp/rtcdp-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >Dados do cliente em tempo real [!DNL Platform] e [!DNL Target]</a
        >
      </td>
    </tr>
  </tbody>
</table>
