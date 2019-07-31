---
title: tipo de recurso riskUserActivity
description: autor
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b4b33d4f9344f8031076f00b1b442b882fffe6d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965352"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="596b8-103">tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="596b8-103">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="596b8-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="596b8-104">Properties</span></span>

| <span data-ttu-id="596b8-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="596b8-105">Property</span></span>       | <span data-ttu-id="596b8-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="596b8-106">Type</span></span>    |<span data-ttu-id="596b8-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="596b8-107">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="596b8-108">eventType</span><span class="sxs-lookup"><span data-stu-id="596b8-108">eventTypes</span></span> | <span data-ttu-id="596b8-109">coleção riskEventType</span><span class="sxs-lookup"><span data-stu-id="596b8-109">riskEventType collection</span></span> |<span data-ttu-id="596b8-110">Os valores possíveis são unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, genérico, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="596b8-110">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="596b8-111">detalhada</span><span class="sxs-lookup"><span data-stu-id="596b8-111">detail</span></span>     | <span data-ttu-id="596b8-112">riskDetail</span><span class="sxs-lookup"><span data-stu-id="596b8-112">riskDetail</span></span>  | <span data-ttu-id="596b8-113">Os valores possíveis são None, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, oculto, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="596b8-113">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="596b8-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="596b8-114">JSON representation</span></span>

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
