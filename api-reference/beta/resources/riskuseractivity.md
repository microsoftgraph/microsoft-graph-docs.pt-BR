---
title: tipo de recurso riskUserActivity
description: autor
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 26dc0cf4d8309e2cc116b4b4265a3d592d316a56
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43178889"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="97a17-103">tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="97a17-103">riskUserActivity resource type</span></span>

<span data-ttu-id="97a17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97a17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="97a17-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97a17-105">Properties</span></span>

| <span data-ttu-id="97a17-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97a17-106">Property</span></span>       | <span data-ttu-id="97a17-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="97a17-107">Type</span></span>    |<span data-ttu-id="97a17-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="97a17-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="97a17-109">eventType</span><span class="sxs-lookup"><span data-stu-id="97a17-109">eventTypes</span></span> | <span data-ttu-id="97a17-110">coleção riskEventType</span><span class="sxs-lookup"><span data-stu-id="97a17-110">riskEventType collection</span></span> |<span data-ttu-id="97a17-111">Os valores possíveis são unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="97a17-111">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="97a17-112">detalhada</span><span class="sxs-lookup"><span data-stu-id="97a17-112">detail</span></span>     | <span data-ttu-id="97a17-113">riskDetail</span><span class="sxs-lookup"><span data-stu-id="97a17-113">riskDetail</span></span>  | <span data-ttu-id="97a17-114">Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, Hidden, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="97a17-114">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="97a17-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97a17-115">JSON representation</span></span>

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
