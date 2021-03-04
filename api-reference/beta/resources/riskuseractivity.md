---
title: Tipo de recurso riskUserActivity
description: autor
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7772bde328004ffd26133421cc97a9f296ae9370
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442870"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="f8e09-103">Tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="f8e09-103">riskUserActivity resource type</span></span>

<span data-ttu-id="f8e09-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8e09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="f8e09-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8e09-105">Properties</span></span>

| <span data-ttu-id="f8e09-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8e09-106">Property</span></span>       | <span data-ttu-id="f8e09-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8e09-107">Type</span></span>    |<span data-ttu-id="f8e09-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8e09-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f8e09-109">eventTypes</span><span class="sxs-lookup"><span data-stu-id="f8e09-109">eventTypes</span></span> | <span data-ttu-id="f8e09-110">Coleção riskEventType</span><span class="sxs-lookup"><span data-stu-id="f8e09-110">riskEventType collection</span></span> |<span data-ttu-id="f8e09-111">Lista de tipos de eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="f8e09-111">List of risk event types.</span></span> <span data-ttu-id="f8e09-112">Depreciado.</span><span class="sxs-lookup"><span data-stu-id="f8e09-112">Deprecated.</span></span> <span data-ttu-id="f8e09-113">Use **riskEventType** em vez disso.</span><span class="sxs-lookup"><span data-stu-id="f8e09-113">Use **riskEventType** instead.</span></span> |
|<span data-ttu-id="f8e09-114">riskEventType</span><span class="sxs-lookup"><span data-stu-id="f8e09-114">riskEventType</span></span>|<span data-ttu-id="f8e09-115">string</span><span class="sxs-lookup"><span data-stu-id="f8e09-115">string</span></span>|<span data-ttu-id="f8e09-116">O tipo de evento de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="f8e09-116">The type of risk event detected.</span></span> <span data-ttu-id="f8e09-117">Os valores possíveis `unlikelyTravel` são , , , , , , , `anonymizedIPAddress` , , , , `maliciousIPAddress` , , `unfamiliarFeatures` , , `malwareInfectedIPAddress` e `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="f8e09-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="f8e09-118">detail</span><span class="sxs-lookup"><span data-stu-id="f8e09-118">detail</span></span>     | <span data-ttu-id="f8e09-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="f8e09-119">riskDetail</span></span>  | <span data-ttu-id="f8e09-120">Os valores possíveis `none` são , , , , , , , `adminGeneratedTemporaryPassword` , , , `userPerformedSecuredPasswordChange` , , `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="f8e09-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f8e09-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8e09-121">JSON representation</span></span>

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


