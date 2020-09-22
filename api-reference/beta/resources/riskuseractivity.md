---
title: tipo de recurso riskUserActivity
description: autor
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ecfe618a8db9f03bbf088ea053476fe6e51bcbf7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988937"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="64019-103">tipo de recurso riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="64019-103">riskUserActivity resource type</span></span>

<span data-ttu-id="64019-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64019-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="64019-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64019-105">Properties</span></span>

| <span data-ttu-id="64019-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64019-106">Property</span></span>       | <span data-ttu-id="64019-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="64019-107">Type</span></span>    |<span data-ttu-id="64019-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="64019-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="64019-109">eventType</span><span class="sxs-lookup"><span data-stu-id="64019-109">eventTypes</span></span> | <span data-ttu-id="64019-110">coleção riskEventType</span><span class="sxs-lookup"><span data-stu-id="64019-110">riskEventType collection</span></span> |<span data-ttu-id="64019-111">Lista de tipos de eventos de risco.</span><span class="sxs-lookup"><span data-stu-id="64019-111">List of risk event types.</span></span> <span data-ttu-id="64019-112">Depreciado.</span><span class="sxs-lookup"><span data-stu-id="64019-112">Deprecated.</span></span> <span data-ttu-id="64019-113">Use **riskEventType** em vez disso.</span><span class="sxs-lookup"><span data-stu-id="64019-113">Use **riskEventType** instead.</span></span> |
|<span data-ttu-id="64019-114">riskEventType</span><span class="sxs-lookup"><span data-stu-id="64019-114">riskEventType</span></span>|<span data-ttu-id="64019-115">string</span><span class="sxs-lookup"><span data-stu-id="64019-115">string</span></span>|<span data-ttu-id="64019-116">O tipo de evento de risco detectado.</span><span class="sxs-lookup"><span data-stu-id="64019-116">The type of risk event detected.</span></span> <span data-ttu-id="64019-117">Os valores possíveis são:,,,,,,,,,,, `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` e `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="64019-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="64019-118">detalhada</span><span class="sxs-lookup"><span data-stu-id="64019-118">detail</span></span>     | <span data-ttu-id="64019-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="64019-119">riskDetail</span></span>  | <span data-ttu-id="64019-120">Os valores possíveis são:,,,,,,,,, `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` , `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="64019-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="64019-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64019-121">JSON representation</span></span>

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


