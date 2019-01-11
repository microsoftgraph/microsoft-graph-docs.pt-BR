---
title: tipo de recurso de skypeForBusinessParticipantActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: de86c49da34c9af48478a912a6ab042a354a7bf5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808187"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="364d4-103">tipo de recurso de skypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="364d4-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="364d4-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="364d4-104">Properties</span></span>

| <span data-ttu-id="364d4-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="364d4-105">Property</span></span>          | <span data-ttu-id="364d4-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="364d4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="364d4-107">mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="364d4-107">im</span></span>                | <span data-ttu-id="364d4-108">Int64</span><span class="sxs-lookup"><span data-stu-id="364d4-108">Int64</span></span>  |
| <span data-ttu-id="364d4-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="364d4-109">audioVideo</span></span>        | <span data-ttu-id="364d4-110">Int64</span><span class="sxs-lookup"><span data-stu-id="364d4-110">Int64</span></span>  |
| <span data-ttu-id="364d4-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="364d4-111">appSharing</span></span>        | <span data-ttu-id="364d4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="364d4-112">Int64</span></span>  |
| <span data-ttu-id="364d4-113">web</span><span class="sxs-lookup"><span data-stu-id="364d4-113">web</span></span>               | <span data-ttu-id="364d4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="364d4-114">Int64</span></span>  |
| <span data-ttu-id="364d4-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="364d4-115">dialInOut3rdParty</span></span> | <span data-ttu-id="364d4-116">Int64</span><span class="sxs-lookup"><span data-stu-id="364d4-116">Int64</span></span>  |
| <span data-ttu-id="364d4-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="364d4-117">reportRefreshDate</span></span> | <span data-ttu-id="364d4-118">Data</span><span class="sxs-lookup"><span data-stu-id="364d4-118">Date</span></span>   |
| <span data-ttu-id="364d4-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="364d4-119">reportDate</span></span>        | <span data-ttu-id="364d4-120">Data</span><span class="sxs-lookup"><span data-stu-id="364d4-120">Date</span></span>   |
| <span data-ttu-id="364d4-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="364d4-121">reportPeriod</span></span>      | <span data-ttu-id="364d4-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="364d4-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="364d4-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="364d4-123">JSON representation</span></span>

<span data-ttu-id="364d4-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="364d4-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
