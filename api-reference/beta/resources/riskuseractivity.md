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
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="2e676-103">tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="2e676-103">riskUserActivity resource type</span></span>

<span data-ttu-id="2e676-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e676-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="2e676-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e676-105">Properties</span></span>

| <span data-ttu-id="2e676-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e676-106">Property</span></span>       | <span data-ttu-id="2e676-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e676-107">Type</span></span>    |<span data-ttu-id="2e676-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e676-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2e676-109">eventType</span><span class="sxs-lookup"><span data-stu-id="2e676-109">eventTypes</span></span> | <span data-ttu-id="2e676-110">coleção riskEventType</span><span class="sxs-lookup"><span data-stu-id="2e676-110">riskEventType collection</span></span> |<span data-ttu-id="2e676-111">Lista de tipos de eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="2e676-111">List of risk event types.</span></span> <span data-ttu-id="2e676-112">Obsoleto.</span><span class="sxs-lookup"><span data-stu-id="2e676-112">Deprecated.</span></span> <span data-ttu-id="2e676-113">Use **riskEventTypes** em vez disso.</span><span class="sxs-lookup"><span data-stu-id="2e676-113">Use **riskEventTypes** instead.</span></span> |
|<span data-ttu-id="2e676-114">riskEventType</span><span class="sxs-lookup"><span data-stu-id="2e676-114">riskEventType</span></span>|<span data-ttu-id="2e676-115">string</span><span class="sxs-lookup"><span data-stu-id="2e676-115">string</span></span>|<span data-ttu-id="2e676-116">O tipo de evento de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="2e676-116">The type of risk event detected.</span></span> <span data-ttu-id="2e676-117">Os valores possíveis são `unlikelyTravel`: `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue`,,,,,,,,,,, e. `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised`</span><span class="sxs-lookup"><span data-stu-id="2e676-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="2e676-118">detalhada</span><span class="sxs-lookup"><span data-stu-id="2e676-118">detail</span></span>     | <span data-ttu-id="2e676-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="2e676-119">riskDetail</span></span>  | <span data-ttu-id="2e676-120">Os valores possíveis são `none`: `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue`,,,,,,,,,,. `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised`</span><span class="sxs-lookup"><span data-stu-id="2e676-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="2e676-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e676-121">JSON representation</span></span>

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
