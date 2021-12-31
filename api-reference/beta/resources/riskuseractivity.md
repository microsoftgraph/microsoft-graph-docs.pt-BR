---
title: Tipo de recurso riskUserActivity
description: autor
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 210f05deca42c1deed6863633b48cc5edeb42494
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647102"
---
# <a name="riskuseractivity-resource-type"></a>Tipo de recurso riskUserActivity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
| riskEventType | Coleção String | O tipo de evento de risco detectado. Os valores possíveis são: `unlikelyTravel` , , , , , , , , `anonymizedIPAddress` , , , , `maliciousIPAddress` , , `unfamiliarFeatures` , `malwareInfectedIPAddress` , `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` . |
| detail     | riskDetail  | Os valores possíveis `none` são , , , , , , , `adminGeneratedTemporaryPassword` , , , `userPerformedSecuredPasswordChange` , , `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` .  |
| eventTypes (preterido) | Coleção riskEventType |Lista de tipos de eventos de risco. Depreciado. Use **riskEventType** em vez disso. |
|riskEventType|Coleção String|O tipo de evento de risco detectado. Os valores possíveis `unlikelyTravel` são , , , , , , , `anonymizedIPAddress` , , , , `maliciousIPAddress` , , `unfamiliarFeatures` , , `malwareInfectedIPAddress` e `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` . |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskUserActivity"
}-->
```json
{
    "eventTypes": ["String"],
    "riskEventType": ["String"],
    "detail": "String"
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


