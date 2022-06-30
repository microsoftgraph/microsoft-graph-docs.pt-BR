---
title: Oportunidades de parceria com o Microsoft Graph API de Segurança
description: Este artigo ajuda os gerentes de produto e as funções de desenvolvimento de negócios a entender os caminhos de investimento e fornece insights sobre as propostas de valor de parceria.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
ms.openlocfilehash: 23a155e42030217046b5af7091cac52d47498b62
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446074"
---
# <a name="partnering-opportunities-with-the-microsoft-graph-security-api"></a>Oportunidades de parceria com o Microsoft Graph API de Segurança

Este artigo descreve as oportunidades de parceria habilitadas pelo Microsoft Graph API de Segurança. Ele foi projetado para ajudar os gerentes de produtos e as funções de desenvolvimento de negócios a entender os caminhos de investimento e fornecer insights sobre as propostas de valor de parceria.

## <a name="background"></a>Histórico

A maioria das organizações lida com grandes volumes de dados de segurança e tem dezenas de soluções de segurança em sua empresa, tornando a tarefa de integrar vários produtos e serviços assustadores e complexos. Esses desafios impedem que as organizações se movam rapidamente ao detectar e corrigir ameaças em um mundo de ataques de interrupção em rápida movimentação.

Os parceiros de tecnologia podem se integrar à plataforma Microsoft usando o Microsoft Graph API de Segurança para resolver esses desafios do cliente.

## <a name="introduction-to-the-microsoft-graph-security-api"></a>Introdução ao microsoft graph API de Segurança

A API de Segurança do Microsoft Graph é uma API unificada que fornece uma interface padrão e um esquema uniforme para integrar alertas de segurança e inteligência contra ameaças de várias fontes, enriquecer alertas e dados com informações contextuais e automatizar operações de segurança.

A API de segurança faz parte do Microsoft Graph, que é uma API REST unificada para integrar dados e inteligência de produtos e serviços da Microsoft e parceiros. Usando o Microsoft Graph, clientes e parceiros podem criar rapidamente soluções que são autenticadas uma vez e usam uma única chamada de API para acessar ou agir em informações de segurança de várias soluções de segurança. O valor adicional é descoberto quando você explora as outras entidades do [Microsoft Graph](./overview.md) (Microsoft 365, Azure Active Directory, Intune e muito mais) para vincular o contexto de negócios aos seus insights de segurança.

A Microsoft permite a integração de parceiros de tecnologia de duas maneiras principais.

1. Como consumidor de informações do Microsoft Graph, você pode enriquecer suas soluções com informações contidas no Microsoft Graph, bem como usar o Microsoft API do Graph para executar tarefas em nome de um cliente.
2. Você também pode contribuir com seus alertas e ações para o Microsoft Graph junto com os provedores da Microsoft.

|Como você se integra?|Dados disponíveis|Funcionalidades com suporte|
|:--------------------|:-------------|:---------------------|
|Integre seu aplicativo ao Microsoft Graph API de Segurança.|<li>Alertas de provedores de segurança do Microsoft Graph</li><li>Classificações seguras da Microsoft</li>| <li>Alertas de consulta/Classificação de Segurança</li> <li>Chamar uma ação de segurança do Microsoft Graph</li> <li>Atualizar um alerta de Segurança do Microsoft Graph</li> <li>Carregar indicadores de ameaça do cliente para a Microsoft</li> |
|Permitir que outras pessoas se integrem aos seus produtos por meio do Microsoft Graph API de Segurança.|<li>Alertas de seus produtos de segurança</li>|<li>Ações de segurança para seu produto de segurança</li>|

Vamos nos aprofundar um pouco e explorar alguns cenários comuns em que a integração do Microsoft Graph API de Segurança amplia os investimentos de integração de segurança e os benefícios para os clientes que podemos obter juntos.

## <a name="featured-technology-partner-scenarios"></a>Cenários de parceiros de tecnologia em destaque

A seguir estão três benefícios principais que você pode derivar integrando-se ao Microsoft Graph API de Segurança:

1. Seus clientes se beneficiam de melhorias na eficácia e nas operações de segurança.
2. Seus clientes se beneficiam das informações avançadas fornecidas pelos seus e outros produtos de parceiros integrados.
3. O investimento em engenharia para parceiros de tecnologia é simplificado e o valor do cliente é ampliado por meio da integração com o Microsoft Graph API de Segurança.

### <a name="enhance-threat-protection-with-the-microsoft-graph-security-api"></a>Aprimorar a proteção contra ameaças com o microsoft graph API de Segurança

*Habilitando a integração mais fácil de alertas de segurança para informar a detecção e a resposta de ameaças.*

- Correlacione alertas/detecções de provedores de Segurança do Microsoft Graph com suas detecções para melhorar os resultados da investigação e as automações de suporte.
- Acesse detecções e contexto por meio do Microsoft Graph para melhorar a resposta a ameaças – triagem, investigação, correção.
- Acesse a inteligência contra ameaças do cliente (hash, IP, URL, domínio etc.) para bloquear/alertar sobre atividades mal-intencionadas.

### <a name="streamline-it-and-security-management"></a>Simplifique o gerenciamento de segurança e TI

*Fornecendo maior visibilidade e simplificando o gerenciamento do ciclo de vida de incidentes.*

- Agregar alertas de vários provedores para criar incidentes.
- Acesse contexto adicional para informar a priorização e a resposta de alertas.
- Mantenha o status do alerta sincronizado entre sistemas que gerenciam alertas.
- Obtenha visibilidade sobre a postura de segurança e a recomendação sobre como aprimozá-la com o Secure Scores.

### <a name="share-threat-intelligence-to-enable-custom-detections"></a>Compartilhar inteligência contra ameaças para habilitar detecções personalizadas

*Aproveite sua inteligência contra ameaças para aproveitar as detecções personalizadas em soluções da Microsoft.*

- Envie automaticamente seus indicadores de ameaça para soluções de segurança da Microsoft para habilitar ações de Alerta, Bloquear ou Permitir.
- Habilite uma ação rápida para se defender contra novas ameaças, como arquivo de bloco, URL, domínio, endereço IP de dentro de suas ferramentas de segurança e fluxos de trabalho.
- A TI fornecida pelo cliente é usada apenas para o cliente que fornece e não para nenhum outro cliente da Microsoft.

## <a name="technical-integrations-overview"></a>Visão geral das integrações técnicas

As oportunidades de API de Segurança Microsoft Graph são disponibilizadas por meio de dois caminhos de integração principais, que podem ser usados de forma independente ou em conjunto.  Descreveremos os requisitos de alto nível e forneceremos algumas informações sobre como investir nesses caminhos aqui, mas explicações técnicas detalhadas são deixadas para os documentos referenciados posteriormente neste documento.

Entidades com suporte:

- **Os alertas** são "conclusões com um impacto de segurança" em vez de dados de log brutos ou outras informações não corrigidas. [Saiba mais](/graph/api/resources/security-api-overview#alerts).
- **Os Indicadores de** Ameaças, também chamados de indicadores de comprometimento ou IoCs, representam dados sobre ameaças conhecidas, como arquivos mal-intencionados, URLs, domínios e endereços IP. Os clientes podem gerar indicadores por meio da coleta interna de inteligência contra ameaças ou adquirir indicadores de comunidades de inteligência contra ameaças, feeds licenciados e outras fontes. [Saiba mais](/graph/api/resources/tiindicator).
- **As Ações de Segurança** permitem que os parceiros de tecnologia exponham funcionalidades funcionais por meio do Graph.  Por exemplo, se sua solução de segurança der suporte à capacidade de bloquear endereços IP, você poderá expor "IP de bloco" como uma funcionalidade no Graph. Outros produtos API de Segurança Graph podem chamar sua ação por meio do Graph. [Saiba mais](/graph/api/resources/securityaction).
- **Classificação de Segurança**... [Saiba mais](/graph/api/resources/securescores).

### <a name="integrate-your-application-with-the-microsoft-graph-security-api"></a>Integrar seu aplicativo ao microsoft graph API de Segurança

Todos os aplicativos [integrados devem ser registrados](./auth-register-app-v2.md) com o Microsoft Graph. Há suporte para ambos os aplicativos usados por um único cliente, bem como aqueles usados por muitos clientes (multilocatário).  Em ambos os casos, o cliente deve conceder consentimento para seu aplicativo. Ao chamar o Microsoft Graph, cada solicitação do seu aplicativo conterá o identificador do aplicativo e o cliente do qual você está chamando em nome. Há suporte para os seguintes tipos de solicitações:

- **Obter alertas** – obtenha informações de alerta com filtragem conforme necessário.  Por exemplo: mostre-me todos os alertas de alta prioridade ou "todos os alertas de alta prioridade" para um usuário, host etc. específico.
- **Atualizar o Status do Alerta** – Habilitando o gerenciamento de um ciclo de vida de alerta.  Por exemplo: definir um status de alertas como "resolvido" de "em andamento" ou adicionar comentários a um alerta.
- **Obter Classificação de Segurança** – o Microsoft Secure Score é um valor de tipo de "classificação de crédito" para configurações de segurança de produtos da Microsoft.
- **Assinar** – Permitindo a notificação de alterações em alertas ou consultas.
- **Alimentar indicadores de ameaça personalizados** – envie automaticamente seus indicadores de ameaça para soluções de segurança da Microsoft para habilitar ações de Alerta, Bloquear ou Permitir. Use o Microsoft Graph API de Segurança diretamente ou aproveite as integrações com as principais plataformas de inteligência contra ameaças.
- **Invocar uma ação de segurança do Microsoft Graph** – tome medidas imediatas para se defender contra ameaças usando a entidade [securityActions](/graph/api/resources/securityaction) de segurança do Microsoft Graph.

### <a name="enable-others-to-integrate-with-your-products-through-the-microsoft-graph-security-api"></a>Permitir que outras pessoas se integrem aos seus produtos por meio do Microsoft Graph API de Segurança

Os provedores de Segurança do Microsoft Graph disponibilizam seus alertas de segurança para outras pessoas por meio do Microsoft Graph.  Todos os produtos da Microsoft que geram alertas de segurança têm provedores que expõem seus respectivos alertas ao Microsoft Graph. Além disso, o Microsoft Graph API de Segurança permite que provedores externos, permitindo que você, como um parceiro de tecnologia da Microsoft, compartilhe alertas de segurança relevantes de seus aplicativos no Microsoft Graph para que os clientes usem. Além dos alertas, o SecurityActions do Microsoft Graph permite que os parceiros de tecnologia exponham recursos funcionais por meio do Microsoft Graph.  Por exemplo, se sua solução de segurança der suporte à capacidade de bloquear endereços IP, você poderá expor "IP de bloco" como uma funcionalidade no Microsoft Graph. Outros produtos de Segurança do Microsoft Graph podem chamar sua ação por meio do Microsoft Graph.

Um Provedor de Segurança do Microsoft Graph é essencialmente um ponto de extremidade de nuvem que responde a solicitações do Microsoft Graph API de Segurança e retorna os alertas de segurança relevantes ou executa ações para clientes mútuos. A autenticação de cliente e serviço a serviço garante que o acesso a alertas e ações do cliente seja protegido.

Os cenários de provedor são amplamente variados. Um processo de integração coletado começa com a identificação de cenários relevantes. Depois que os cenários forem acordados, a documentação, o código de exemplo e os ambientes de desenvolvimento estarão disponíveis para dar suporte ao desenvolvimento do Provedor de Segurança do Microsoft Graph.

## <a name="get-started"></a>Introdução

### <a name="onboarding-guides-and-technical-documentation"></a>Guias de integração e documentação técnica

- [Visão geral do microsoft graph API de Segurança](./security-concept-overview.md)
- [Referência da API](/graph/api/resources/security-api-overview)
- [esquema de alerta](/graph/api/resources/alert)
- [Esquema tiIndicator](/graph/api/resources/tiindicator)
- [Esquema de Ações de Segurança](/graph/api/resources/securityaction)
- [Esquema de Classificação de Segurança](/graph/api/resources/securescores)

### <a name="sample-code"></a>Código de exemplo

- [Exemplos de Segurança do Microsoft Graph](https://aka.ms/graphsecurityapicode)
- [Contribuir com exemplos de Segurança do Microsoft Graph](https://aka.ms/graphsecurityapicodecontribute)

### <a name="help-and-support"></a>Ajuda e suporte

- Se você tiver dúvidas sobre integrações de aplicativos ou serviços ou produtos com o microsoft graph API de Segurança, entre em contato com a comunidade técnica Using [Microsoft Security API do Graph tech](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/bd-p/SecurityGraphAPI)
- Siga as discussões [sobre o Microsoft Q&A](/answers/topics/microsoft-graph-security.html)  com a marca: microsoft-graph-security.
- Se você encontrar bugs nos exemplos ou solicitações de documentação ou problemas de arquivo de bugs no respectivo [repositório de exemplo](https://github.com/microsoftgraph/security-api-solutions/blob/master/sample-repos.md).
- Se você tiver novas solicitações de exemplo ou problemas que não estão no escopo de um único [exemplo, arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) problemas no repositório soluções de segurança do [Microsoft Graph](https://github.com/microsoftgraph/security-api-solutions).

### <a name="getting-to-market"></a>Introdução ao mercado

- [Microsoft Partner Network](https://partner.microsoft.com/) – O principal programa para parceria com a Microsoft é o Microsoft Partner Network. As integrações de Segurança do Microsoft Graph se enquadram na faixa [de ISV (Fornecedor Independente de Software) do MPN](https://partner.microsoft.com/isv-resource-hub) .
- [A Associação de Segurança](https://www.microsoft.com/security/partnerships/intelligent-security-association) Inteligente da Microsoft é o programa especificamente para parceiros de segurança da Microsoft para ajudar a enriquecer seus produtos de segurança e melhorar a capacidade de descoberta do cliente de suas integrações aos produtos de Segurança da Microsoft.
- Microsoft AppSource – Como parceiro de API de Segurança Microsoft Graph, você pode listar sua integração do Microsoft Graph no [Microsoft AppSource Marketplace](https://appsource.microsoft.com/partners/signup).
