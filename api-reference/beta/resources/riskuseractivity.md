---
title: tipo de recurso riskUserActivity
description: autor
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8032a721a8f8a94d7cd1481edf58ee785092bcfd
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556314"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="12f97-103">tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="12f97-103">riskUserActivity resource type</span></span>

<span data-ttu-id="12f97-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12f97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="12f97-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12f97-105">Properties</span></span>

| <span data-ttu-id="12f97-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12f97-106">Property</span></span>       | <span data-ttu-id="12f97-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="12f97-107">Type</span></span>    |<span data-ttu-id="12f97-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="12f97-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12f97-109">eventType</span><span class="sxs-lookup"><span data-stu-id="12f97-109">eventTypes</span></span> | <span data-ttu-id="12f97-110">coleção riskEventType</span><span class="sxs-lookup"><span data-stu-id="12f97-110">riskEventType collection</span></span> |<span data-ttu-id="12f97-111">Lista de tipos de eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="12f97-111">List of risk event types.</span></span> <span data-ttu-id="12f97-112">Obsoleto.</span><span class="sxs-lookup"><span data-stu-id="12f97-112">Deprecated.</span></span> <span data-ttu-id="12f97-113">Use **riskEventType** em vez disso.</span><span class="sxs-lookup"><span data-stu-id="12f97-113">Use **riskEventType** instead.</span></span> |
|<span data-ttu-id="12f97-114">riskEventType</span><span class="sxs-lookup"><span data-stu-id="12f97-114">riskEventType</span></span>|<span data-ttu-id="12f97-115">string</span><span class="sxs-lookup"><span data-stu-id="12f97-115">string</span></span>|<span data-ttu-id="12f97-116">O tipo de evento de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="12f97-116">The type of risk event detected.</span></span> <span data-ttu-id="12f97-117">Os valores possíveis são:,,,,,,,,,,, `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` e `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="12f97-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="12f97-118">detalhada</span><span class="sxs-lookup"><span data-stu-id="12f97-118">detail</span></span>     | <span data-ttu-id="12f97-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="12f97-119">riskDetail</span></span>  | <span data-ttu-id="12f97-120">Os valores possíveis são:,,,,,,,,, `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` , `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="12f97-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="12f97-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12f97-121">JSON representation</span></span>

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
