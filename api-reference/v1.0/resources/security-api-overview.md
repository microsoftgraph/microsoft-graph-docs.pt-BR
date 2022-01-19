---
title: Usar a API de Segurança do Microsoft Graph
description: A API de Segurança do Microsoft Graph fornece uma interface unificada e um esquema para integrar soluções de segurança da Microsoft e parceiros de ecossistema.
ms.localizationpriority: high
author: preetikr
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 47dccb5f8c4bf71ce5814b8f50d7ed2625f7ca01
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072646"
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

Alertas dos seguintes provedores estão disponíveis por meio da API de segurança do Microsoft Graph. O suporte para alertas GET, alertas PATCH e inscrições (via webhooks) é indicado na tabela a seguir.

| Provedor de segurança | <p align="center">Alerta GET</p>| <p align="center">Alerta PATCH</p>| <p align="center">Assinar o alerta</p>|
|:------------------|:---------|:-----------|:------------------|
|[Microsoft Defender para Nuvem](/azure/defender-for-cloud/alerts-overview)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Proteção de identidade do Azure Active Directory](/azure/active-directory/identity-protection/playbook) | <p align="center">&#x2713;</p> | <p align="center">[Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
| [Microsoft Defender for Cloud Apps](/cloud-app-security/monitor-alerts) | <p align="center">&#x2713;</p> | <p align="center">[Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Microsoft Defender para Ponto de Extremidade](/windows/security/threat-protection/microsoft-defender-atp/attack-simulations) **| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center"> [Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Microsoft Defender para Identidade](/defender-for-identity/understanding-security-alerts#security-alert-categories) ***| <p align="center">&#x2713;</p> | <p align="center">[Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|Microsoft 365 <ul><li> [Padrão](/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Segurança no Aplicativo na Nuvem](/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li><li>Alerta personalizado</li></ul> | <p align="center">&#x2713;</p> | <p align="center"> [Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Proteção de Informações do Azure](/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(visualização)**| <p align="center">&#x2713;</p> | <p align="center">[Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Azure Sentinel](/azure/sentinel/quickstart-get-visibility) **(visualização)**| <p align="center">&#x2713;</p> | <p align="center">Não possui suporte do Azure Sentinel </p> | <p align="center">&#x2713;</p> |
> **Observação:** Novos provedores estão se integrando continuamente ao ecossistema de Segurança do Microsoft Graph. Para requerer suporte aos novos provedores ou suporte estendido para os provedores existentes, [registre o problema no repositório GitHub de segurança do Microsoft Graph](https://github.com/microsoftgraph/security-api-solutions/issues/new).

\* Problema no arquivo: o status do alerta é atualizado nos aplicativos integrados da API de segurança do Microsoft Graph, mas não reflete na experiência de gerenciamento do provedor.

\*\* O Microsoft Defender para Ponto de Extremidade exige [funções de usuário](/windows/security/threat-protection/microsoft-defender-atp/user-roles) adicionais para aquelas requeridas pela API de Segurança do Microsoft Graph. Somente os usuários do Microsoft Defender para Ponto de Extremidade e as funções da API de Segurança do Microsoft Graph podem ter acesso aos dados do Microsoft Defender para Ponto de Extremidade. A autenticação somente para aplicativos não é limitada por isso. Portanto, recomendamos que você use um token de autenticação somente para aplicativos.

\*\*\* Os alertas do Microsoft Defender para Identidade estão disponíveis por meio da integração com o Microsoft Defender for Cloud Apps. Isso significa que você receberá alertas do Microsoft Defender para Identidade somente se tiver ingressado no portal Unified SecOps e conectado o Microsoft Defender para Identidade com o Microsoft Defender for Cloud Apps. Saiba mais sobre [como integrar o Microsoft Defender para Identidade com o Microsoft Defender for Cloud Apps.](/defender-for-identity/mcas-integration)

## <a name="information-protection"></a>Proteção de informações

A API de avaliação de ameaças do Microsoft Graph ajuda as organizações a avaliar a ameaça recebida por qualquer usuário em um locatário. Isso permite que os clientes relatem emails de spam, URLs de phishing ou anexos de malware recebidos na Microsoft. Os resultados da verificação de política e os resultados ao verificar novamente, podem ajudar os administradores de locatários a entender o veredicto da verificação de ameaças e ajustar sua política organizacional.

## <a name="secure-score"></a>Classificação de Segurança

A [Microsoft Secure Score](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/A-new-home-and-an-all-new-look-for-Microsoft-Secure-Score/ba-p/529641) é uma solução de análise da segurança que fornece visibilidade ao seu portfólio de segurança e mostra como melhorá-lo. Com uma única classificação, é possível entender melhor o que você fez para reduzir o risco em soluções da Microsoft. Você pode também comparar sua classificação com outras organizações e ver como tem sido a tendência ao longo do tempo. As entidades [secureScore](securescore.md) e [secureScoreControlProfile](securescorecontrolprofile.md) de Segurança do Microsoft Graph ajudam a equilibrar a segurança e a produtividade de que sua organização precisa, além de habilitar o mix adequado de recursos de segurança. Você também pode projetar qual seria sua classificação depois de adotar recursos de segurança.

## <a name="common-use-cases"></a>Casos de uso comuns

A seguir, há algumas das solicitações mais populares para trabalhar com a API de Segurança do Microsoft Graph:

| **Casos de uso**   | **Recursos REST** | **Experimentar no Explorador do Graph** |
|:---------------|:--------|:----------|
| Listar alertas | [List alerts](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| Atualizar alertas | [Update alert](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |
|Listar classificações de segurança|[Listar secureScores](../api/security-list-securescores.md) |[https://graph.microsoft.com/v1.0/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|Obter classificação de segurança|[Obter secureScore](../api/securescore-get.md) |[https://graph.microsoft.com/v1.0/security/secureScores/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores/{id}&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|Listar perfis de controle da classificação de segurança|[Listar secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md) |[https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|Obter perfis de controle da classificação de segurança|[Obter secureScoreControlProfile](../api/securescorecontrolprofile-get.md) |[https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|Atualizar perfis de controle da classificação de segurança|[Atualizar secureScoreControlProfile](../api/securescorecontrolprofile-update.md) |[https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com)|


Você pode usar o Microsoft Graph [webhooks](/graph/webhooks) para assinar e receber notificações sobre as atualizações de entidades de Segurança do Microsoft Graph.

## <a name="resources"></a>Recursos

Codifique e contribua com esses exemplos da API de Segurança do Microsoft Graph:

- [Amostra do ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Amostra do Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Amostra do Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Participe da comunidade:

- [Junte-se à comunidade técnica](https://aka.ms/graphsecuritycommunity)
- [Discussão no StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para esses conjuntos de API.

## <a name="next-steps"></a>Próximas etapas

A API de Segurança do Microsoft Graph pode abrir novas formas para você interagir com diferentes soluções de segurança da Microsoft e de parceiros. Siga estas etapas para começar:

- Expandir [alerts](alert.md), [secureScore](securescore.md) e [secureScoreControlProfiles](securescorecontrolprofile.md).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer). Em **Consultas de Exemplo**, escolha **mostrar mais amostras** e defina a categoria Segurança como **on**.
- Experimente [assinar e receber notificações](/graph/webhooks) sobre alterações de entidade.

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/partners).

## <a name="see-also"></a>Confira também

[Codifique e contribua](https://github.com/microsoftgraph/security-api-solutions/blob/master/CONTRIBUTING.md) com esses exemplos da API de Segurança do Microsoft Graph:

- [Amostra do ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Amostra do Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Amostra do Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)
- [Exemplo do PowerShell](https://aka.ms/graphsecuritypowershellsample)
- [Outros exemplos ou contribuir com um novo exemplo](https://aka.ms/graphsecurityapicode)

Explore outras opções para se conectar com a API de segurança da Microsoft Graph:

- [Conectores de Segurança do Microsoft Graph para Aplicativos de Lógica, Flow e PowerApps](/azure/connectors/connectors-integrate-security-operations-create-api-microsoft-graph-security)
- [Amostras do Bloco de anotações Jupyter](https://aka.ms/graphsecurityjupyternotebooks)

Participe da comunidade:

- [Junte-se à comunidade técnica](https://techcommunity.microsoft.com/t5/microsoft-graph-security-api/bd-p/SecurityGraphAPI)
- [Discussão no StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)