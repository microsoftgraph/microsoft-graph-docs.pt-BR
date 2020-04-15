---
title: tipo de recurso riskUserActivity
description: autor
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ddf71668af9d66c1d3ea495a8438c444b9317a23
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510991"
---
# <a name="riskuseractivity-resource-type"></a>tipo de recurso riskUserActivity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
| eventType | coleção riskEventType |Lista de tipos de eventos de risco. Obsoleto. Use **riskEventTypes** em vez disso. |
|riskEventType|string|O tipo de evento de risco detectado. Os valores possíveis são `unlikelyTravel`: `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue`,,,,,,,,,,, e. `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` |
| detalhada     | riskDetail  | Os valores possíveis são `none`: `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue`,,,,,,,,,,. `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised`  |

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
