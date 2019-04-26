---
title: tipo de recurso riskUserActivity
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1685c58697f9de52e209d508c1ec104b9c044e8d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343560"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="8057e-102">tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="8057e-102">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="8057e-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8057e-103">Properties</span></span>

| <span data-ttu-id="8057e-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8057e-104">Property</span></span>       | <span data-ttu-id="8057e-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="8057e-105">Type</span></span>    |<span data-ttu-id="8057e-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="8057e-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8057e-107">eventType</span><span class="sxs-lookup"><span data-stu-id="8057e-107">eventTypes</span></span> | <span data-ttu-id="8057e-108">coleção riskEventType</span><span class="sxs-lookup"><span data-stu-id="8057e-108">riskEventType collection</span></span> |<span data-ttu-id="8057e-109">Os valores possíveis são unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, genérico, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="8057e-109">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="8057e-110">detalhada</span><span class="sxs-lookup"><span data-stu-id="8057e-110">detail</span></span>     | <span data-ttu-id="8057e-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="8057e-111">riskDetail</span></span>  | <span data-ttu-id="8057e-112">Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, oculto, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="8057e-112">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8057e-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8057e-113">JSON representation</span></span>

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
