---
title: tipo de recurso riskUserActivity
description: autor
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1601f34b7d54a2c5304f3b20b04b8cb4c69c6323
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521065"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="48fe1-103">tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="48fe1-103">riskUserActivity resource type</span></span>

<span data-ttu-id="48fe1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="48fe1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="48fe1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48fe1-105">Properties</span></span>

| <span data-ttu-id="48fe1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48fe1-106">Property</span></span>       | <span data-ttu-id="48fe1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="48fe1-107">Type</span></span>    |<span data-ttu-id="48fe1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="48fe1-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48fe1-109">eventType</span><span class="sxs-lookup"><span data-stu-id="48fe1-109">eventTypes</span></span> | <span data-ttu-id="48fe1-110">coleção riskEventType</span><span class="sxs-lookup"><span data-stu-id="48fe1-110">riskEventType collection</span></span> |<span data-ttu-id="48fe1-111">Os valores possíveis são unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, genérico, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="48fe1-111">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="48fe1-112">detalhada</span><span class="sxs-lookup"><span data-stu-id="48fe1-112">detail</span></span>     | <span data-ttu-id="48fe1-113">riskDetail</span><span class="sxs-lookup"><span data-stu-id="48fe1-113">riskDetail</span></span>  | <span data-ttu-id="48fe1-114">Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, oculto, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="48fe1-114">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="48fe1-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48fe1-115">JSON representation</span></span>

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
