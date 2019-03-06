---
title: Usar a API de Segurança do Microsoft Graph
description: 'A API de Segurança do Microsoft Graph fornece uma interface unificada e um esquema para integrar soluções de segurança da Microsoft e parceiros de ecossistema. Isso permite aos clientes agilizar as operações de segurança e a se proteger melhor contra as crescentes ameaças cibernéticas. A API de Segurança do Microsoft Graph pode ser usada como um serviço de agregação de segurança federado para enviar consultas a todos os provedores de segurança participantes e obter respostas agregadas. Use a API de Segurança do Microsoft Graph para compilar aplicativos que:'
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: b3f1d041d6b1a525ba9eff63aca19baf287376ae
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30364588"
---
# <a name="use-the-microsoft-graph-security-api"></a>Usar a API de Segurança do Microsoft Graph

A API de Segurança do Microsoft Graph fornece uma interface unificada e um esquema para integrar soluções de segurança da Microsoft e parceiros de ecossistema. Isso permite aos clientes agilizar as operações de segurança e a se proteger melhor contra as crescentes ameaças cibernéticas. A API de segurança do Microsoft Graph consulta todos os provedores de segurança integrados e agrega respostas. Use a API de Segurança do Microsoft Graph para compilar aplicativos que:

- Consolidem e correlacionem alertas de segurança de várias fontes
- Desbloqueiem dados contextuais para informar investigações
- Automatizem tarefas de segurança, processos de negócios, fluxos de trabalho e relatórios
- Enviem indicadores de ameaças para produtos da Microsoft para detecções personalizados
- Usem ações em resposta à novas ameaças
- Dão visibilidade aos dados de segurança para permitir o gerenciamento proativo dos riscos

A API de Segurança do Microsoft Graph inclui as entidades principais a seguir.

## <a name="alerts"></a>Alertas

Os alertas são possíveis problemas de segurança no locatário de um cliente identificado pela Microsoft ou por soluções de segurança de parceiros identificados e sinalizados para ação ou notificação. Com a entidade de [alertas](alert.md) de Segurança do Microsoft Graph, é possível unificar e simplificar o gerenciamento dos problemas de segurança de todas as soluções integradas. Isso também permite que os aplicativos correlacionem alertas e contextos para melhorar a resposta e a proteção contra ameaças. Com o recurso de atualização de alertas, é possível sincronizar o status de alertas específicos em diferentes produtos e serviços de segurança que estão integrados à API de Segurança do Microsoft Graph atualizando sua entidade de [alertas](alert.md).

Alertas dos seguintes provedores estão disponíveis por meio da API de segurança do Microsoft Graph. O suporte para alertas GET, alertas PATCH (as atualizações estão disponíveis por meio da API de segurança do Microsoft Graph, mas não podem ser expostas no experiência de gerenciamento do provedor), e assinatura (via webhooks) é indicado na tabela a seguir.

| Provedor de segurança | Alerta GET| Alerta PATCH| Assinar o alerta|
|:------------------|:---------|:-----------|:------------------|
|[Central de Segurança do Azure](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)| &#x2713; | &#x2713; | &#x2713; |
|[Proteção de identidade do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook) | &#x2713; | &#x2713; | &#x2713; |
| [Segurança no Aplicativo da Microsoft Cloud](https://docs.microsoft.com/cloud-app-security/monitor-alerts) | &#x2713; | &#x2713; | &#x2713; |
|[Proteção Avançada contra Ameaças do Windows Defender](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)| &#x2713; | &#x2713; | [Problema no arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) |
|[Proteção Avançada contra Ameaças do Azure](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories)| &#x2713; | [Problema no arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) | [Problema no arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) |
|Office 365 </br> <li> [Padrão](https://docs.microsoft.com/pt-BR/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Segurança no Aplicativo na Nuvem](https://docs.microsoft.com/pt-BR/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li> | &#x2713; | [Problema no arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) | [Problema no arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) |
|[Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(visualização)**| &#x2713; | &#x2713; | &#x2713; |
|[Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility) **(visualização)**| &#x2713; | [Problema no arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) | [Problema no arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) |
|[Palo Alto Networks](https://docs.paloaltonetworks.com/pan-os/9-0/pan-os-web-interface-help/monitor/monitor-logs/log-types.html)| &#x2713; | [Problema no arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) | [Problema no arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) |
> **Observação:** Novos provedores estão se integrando continuamente ao ecossistema de Segurança do Microsoft Graph. Para requerer suporte aos novos provedores ou suporte estendido para os provedores existentes, [registre o problema no repositório GitHub de segurança do Microsoft Graph](https://github.com/microsoftgraph/security-api-solutions/issues/new).

## <a name="common-use-cases"></a>Casos de usos comuns

A seguir, há algumas das solicitações mais populares para trabalhar com a API de Segurança do Microsoft Graph:

| **Casos de uso**   | **Recursos REST** | **Experimentar no Explorador do Graph** |
|:---------------|:--------|:----------|
| Listar alertas | [List alerts](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| Atualizar alertas | [Atualizar alertas](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

Você pode usar o Microsoft Graph [webhooks](/graph/webhooks) para assinar e receber notificações sobre as atualizações de entidades de Segurança do Microsoft Graph.

## <a name="resources"></a>Recursos

Codifique e contribua com esses exemplos da API de Segurança do Microsoft Graph:

- [Amostra do ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Amostra do Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Amostra do Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Participe da comunidade:

- [Junte-se à comunidade técnica](https://aka.ms/graphsecuritycommunity)
- [Discussão no StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>Próximas etapas

A API de Segurança do Microsoft Graph pode abrir novas formas de interagir com soluções de segurança diferentes da Microsoft e de parceiros. Siga estas etapas para iniciar:

- Fazer busca detalhada em [alertas](alert.md).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer). Em **Consultas de Exemplo**, escolha **mostrar mais amostras** e defina a categoria Segurança como **on**.
- Experimente [assinar e receber notificações](/graph/webhooks) sobre alterações de entidade.

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

## <a name="see-also"></a>Confira também

[Codifique e contribua](https://github.com/microsoftgraph/security-api-solutions/blob/master/CONTRIBUTING.md) com esses exemplos da API de Segurança do Microsoft Graph:

- [Amostra do ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Amostra do Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Amostra do Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)
- [Exemplo do PowerShell](https://aka.ms/graphsecuritypowershellsample)
- [Outros exemplos ou contribuir com um novo exemplo](https://aka.ms/graphsecurityapicode)

Explore outras opções para se conectar com a API de segurança da Microsoft Graph:

- [Conectores de segurança do Microsoft Graph para Aplicativos de Lógica, Flow e PowerApps](https://aka.ms/graphsecurityconnectors)
- [Conector de segurança do Microsoft Graph para Power BI](https://aka.ms/graphsecuritypowerbiconnectordoc)
- [Exemplos de bloco de anotações Jupyter](https://aka.ms/graphsecurityjupyternotebooks)

Participe da comunidade:

- [Junte-se à comunidade técnica](https://aka.ms/graphsecuritycommunity)
- [Discussão no StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)