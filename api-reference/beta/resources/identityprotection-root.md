---
title: Use a proteção de identidade do Windows Azure AD API (preview)
description: Você pode usar o Microsoft Graph para consultar o recurso de identityRiskEvent para cada tipo de evento de risco detectado pelo proteção de identidade do Windows Azure AD. Esses eventos estão disponíveis para clientes com o Windows Azure AD Premium P2. Um subconjunto de eventos está disponível para clientes com o Windows Azure AD Premium P1.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 597ff7ed156dede995b10f07ee6ac6945745b83c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515094"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>Use a proteção de identidade do Windows Azure AD API (preview)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar o Microsoft Graph para consultar o recurso de [identityRiskEvent](identityriskevent.md) para cada tipo de evento de risco detectado pelo [proteção de identidade do Windows Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection). Esses eventos estão disponíveis para clientes com o Windows Azure AD Premium P2. Um subconjunto de eventos está disponível para clientes com o Windows Azure AD Premium P1.

* [entradas de endereços IP anônimos](anonymousipriskevent.md)
* [entradas de dispositivos infectados por malware](malwareriskevent.md)
* [Impossível viajar para locais atípicos](impossibletravelriskevent.md)
* [usuários com credenciais perdidas](leakedcredentialsriskevent.md)
* [entradas de endereços IP suspeitos](suspiciousipriskevent.md)
* [entradas de familiarizado locais](unfamiliarlocationriskevent.md)

Use as operações a seguir para obter essas informações associadas e eventos:

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| Obter a coleção de identityRiskEvent. |
|[Obter identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| Obtenha o objeto identityRiskEvent. |
|[Lista anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| Obter a coleção de anonymousIpRiskEvent. |
|[Obter anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| Obtenha o objeto anonymousIpRiskEvent. |
|[Lista impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| Obter a coleção de impossibleTravelRiskEvent. |
|[Obter impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| Obtenha o objeto impossibleTravelRiskEvent. |
|[Lista leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| Obter a coleção de leakedCredentialsRiskEvent. |
|[Obter leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| Obtenha o objeto leakedCredentialsRiskEvent. |
|[Lista malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| Obter a coleção de malwareRiskEvent. |
|[Obter malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| Obtenha o objeto malwareRiskEvent. |
|[Lista suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| Obter a coleção de suspiciousIpRiskEvent. |
|[Obter suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| Obtenha o objeto suspiciousIpRiskEvent. |
|[Lista unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| Obter a coleção de unfamiliarLocationRiskEvent. |
|[Obter unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| Obtenha o objeto unfamiliarLocationRiskEvent. |

# <a name="see-also"></a>Confira também

* [Sobre a proteção de identidade do Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)
* [Noções básicas sobre proteção de identidade do Windows Azure Active Directory e do Microsoft Graph](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/identityprotection-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
