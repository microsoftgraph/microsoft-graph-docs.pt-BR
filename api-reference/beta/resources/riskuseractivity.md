---
title: tipo de recurso riskUserActivity
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 258cd61b55d0ac8d19f83682fe34d53cc4b233b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563011"
---
# <a name="riskuseractivity-resource-type"></a>tipo de recurso riskUserActivity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
| eventType | coleção riskEventType |Os valores possíveis são unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, genérico, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.  |
| detalhada     | riskDetail  | Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, oculto, adminConfirmedUserCompromised, unknownFutureValue.  |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskUserActivity"
}-->
```json
{
    "eventTypes": ["String"],
    "detail": "string"
}
```
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "",
  "tocPath": "",
  "suppressions": []
}
-->
