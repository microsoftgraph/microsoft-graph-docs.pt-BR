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
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="287fd-102">tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="287fd-102">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="287fd-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="287fd-103">Properties</span></span>

| <span data-ttu-id="287fd-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="287fd-104">Property</span></span>       | <span data-ttu-id="287fd-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="287fd-105">Type</span></span>    |<span data-ttu-id="287fd-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="287fd-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="287fd-107">eventType</span><span class="sxs-lookup"><span data-stu-id="287fd-107">eventTypes</span></span> | <span data-ttu-id="287fd-108">coleção riskEventType</span><span class="sxs-lookup"><span data-stu-id="287fd-108">riskEventType collection</span></span> |<span data-ttu-id="287fd-109">Os valores possíveis são unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, genérico, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="287fd-109">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="287fd-110">detalhada</span><span class="sxs-lookup"><span data-stu-id="287fd-110">detail</span></span>     | <span data-ttu-id="287fd-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="287fd-111">riskDetail</span></span>  | <span data-ttu-id="287fd-112">Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, oculto, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="287fd-112">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="287fd-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="287fd-113">JSON representation</span></span>

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
