---
title: tipo de recurso teamsUserActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7a330223a7b72b32387998d458456f0661979ae2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519817"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="11c48-103">tipo de recurso teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="11c48-103">teamsUserActivityUserCounts resource type</span></span>

<span data-ttu-id="11c48-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="11c48-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="11c48-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11c48-105">Properties</span></span>

| <span data-ttu-id="11c48-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11c48-106">Property</span></span>            | <span data-ttu-id="11c48-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="11c48-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="11c48-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="11c48-108">reportRefreshDate</span></span>   | <span data-ttu-id="11c48-109">Data</span><span class="sxs-lookup"><span data-stu-id="11c48-109">Date</span></span>   |
| <span data-ttu-id="11c48-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="11c48-110">reportDate</span></span>          | <span data-ttu-id="11c48-111">Data</span><span class="sxs-lookup"><span data-stu-id="11c48-111">Date</span></span>   |
| <span data-ttu-id="11c48-112">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="11c48-112">teamChatMessages</span></span>    | <span data-ttu-id="11c48-113">Int64</span><span class="sxs-lookup"><span data-stu-id="11c48-113">Int64</span></span>  |
| <span data-ttu-id="11c48-114">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="11c48-114">privateChatMessages</span></span> | <span data-ttu-id="11c48-115">Int64</span><span class="sxs-lookup"><span data-stu-id="11c48-115">Int64</span></span>  |
| <span data-ttu-id="11c48-116">calls</span><span class="sxs-lookup"><span data-stu-id="11c48-116">calls</span></span>               | <span data-ttu-id="11c48-117">Int64</span><span class="sxs-lookup"><span data-stu-id="11c48-117">Int64</span></span>  |
| <span data-ttu-id="11c48-118">treinamento</span><span class="sxs-lookup"><span data-stu-id="11c48-118">meetings</span></span>            | <span data-ttu-id="11c48-119">Int64</span><span class="sxs-lookup"><span data-stu-id="11c48-119">Int64</span></span>  |
| <span data-ttu-id="11c48-120">otherActions</span><span class="sxs-lookup"><span data-stu-id="11c48-120">otherActions</span></span>        | <span data-ttu-id="11c48-121">Int64</span><span class="sxs-lookup"><span data-stu-id="11c48-121">Int64</span></span>  |
| <span data-ttu-id="11c48-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="11c48-122">reportPeriod</span></span>        | <span data-ttu-id="11c48-123">String</span><span class="sxs-lookup"><span data-stu-id="11c48-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="11c48-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11c48-124">JSON representation</span></span>

<span data-ttu-id="11c48-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11c48-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
