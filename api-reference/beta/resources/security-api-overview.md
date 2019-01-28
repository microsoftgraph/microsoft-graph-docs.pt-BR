---
title: Usar a API de Segurança do Microsoft Graph
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: cd55b2d26d7460e7421b9da19658990b53dd7580
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571692"
---
# <a name="use-the-microsoft-graph-security-api"></a>Usar a API de Segurança do Microsoft Graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A API de Segurança do Microsoft Graph fornece uma interface unificada e um esquema para integrar soluções de segurança da Microsoft e parceiros de ecossistema. Isso permite aos clientes agilizar as operações de segurança e a se proteger melhor contra as crescentes ameaças cibernéticas. A API de Segurança do Microsoft Graph pode ser usada como um serviço de agregação de segurança federado para enviar consultas a todos os provedores de segurança participantes e obter respostas agregadas. Use a API de Segurança do Microsoft Graph para compilar aplicativos que:

- Consolidem e correlacionem alertas de segurança de várias fontes
- Desbloqueiem dados contextuais para informar investigações
- Automatizem as operações de segurança para maior eficiência
- Forneçam visibilidade a dados de segurança para permitir o gerenciamento proativo de riscos

A API de Segurança do Microsoft Graph inclui as entidades principais a seguir.

## <a name="alerts"></a>Alertas

Os alertas são possíveis problemas de segurança no locatário de um cliente identificado pela Microsoft ou por soluções de segurança de parceiros e são sinalizados para ação ou notificação. Com a entidade de [alertas](alert.md) de Segurança do Microsoft Graph, é  possível unificar e simplificar os problemas de segurança em todas as soluções integradas. Isso também permite que os aplicativos correlacionem alertas e contextos para melhorar a resposta e a proteção contra ameaças também. Eles desbloqueiam as eficiências operacionais de segurança ao reduzir o tempo de investigação e de resolução de incidentes. Com o recurso de atualização de alertas, é possível sincronizar o status de alertas específicos em diferentes produtos e serviços de segurança que estão integrados à API de Segurança do Microsoft Graph atualizando sua entidade de [alertas](alert.md).

As soluções integradas de Segurança do Microsoft Graph receberão alertas dos seguintes provedores de segurança:

- [Central de Segurança do Azure](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Segurança no Aplicativo da Microsoft Cloud](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [Proteção Avançada contra Ameaças do Windows Defender](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- [Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(versão prévia)**
- Microsoft Intune **(versão prévia privada)**
- Office 365 **(em breve)**
- Proteção Avançada contra Ameaças do Azure **(em breve)**
- Soluções de parceiros, como a Estrutura de Aplicativo da Palo Alto Networks

> **Observação:** novos provedores estão se integrando continuamente ao ecossistema de Segurança do Microsoft Graph.

## <a name="secure-score-preview"></a>Classificação de Segurança (versão prévia)

A [Microsoft Secure Score](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358) é uma solução de análise da segurança que fornece visibilidade ao seu portfólio de segurança e mostra como melhorá-lo. Com uma única classificação, é possível entender melhor o que você fez para reduzir o risco em soluções da Microsoft. Você pode também comparar sua classificação com outras organizações e ver como tem sido a tendência ao longo do tempo. As entidades [secureScore](securescores.md) e [secureScoreControlProfile](securescorecontrolprofiles.md) de Segurança do Microsoft Graph ajudam a equilibrar a segurança e a produtividade de que sua organização precisa, além de habilitar o mix adequado de recursos de segurança. Você também pode projetar qual seria sua classificação depois de adotar recursos de segurança.

## <a name="common-use-cases"></a>Casos de uso comuns

A seguir, há algumas das solicitações mais populares para trabalhar com a API de Segurança do Microsoft Graph.

| **Casos de uso**   | **Recursos REST** | **Experimentar no Explorador do Graph** |
|:---------------|:--------|:----------|
| Listar alertas | [List alerts](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| Atualizar alertas | [Update alert](../api/alert-update.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) |
|Listar classificações de segurança|[List secureScores](../api/securescores-list.md) (versão prévia)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Listar perfis de controle da classificação de segurança|[List secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) (versão prévia)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Atualizar perfis de controle da classificação de segurança|[Update secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md) (versão prévia)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

Você pode usar o Microsoft Graph [webhooks](/graph/webhooks) para assinar e receber notificações sobre as atualizações de entidades de Segurança do Microsoft Graph.

## <a name="next-steps"></a>Próximas etapas

A API de Segurança do Microsoft Graph pode abrir novas formas de interagir com soluções de segurança diferentes da Microsoft e de parceiros. Para começar, faça o seguinte:

- Detalhe [alerts](alert.md), [secureScore](securescores.md) (versão prévia) e [secureScoreControlProfile](securescorecontrolprofiles.md) (versão prévia).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer). Em **Consultas de Exemplo**, escolha **mostrar mais amostras** e defina a categoria Segurança como **on**.
- Experimente [assinar e receber notificações](/graph/webhooks) sobre alterações de entidade.

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

## <a name="see-also"></a>Confira também

Codifique e contribua com esses exemplos da API de Segurança do Microsoft Graph:

- [Amostra do ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Amostra do Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Amostra do Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Participe da comunidade:

- [Junte-se à comunidade técnica](https://aka.ms/graphsecuritycommunity)
- [Discussão no StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
