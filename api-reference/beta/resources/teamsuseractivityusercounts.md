---
title: tipo de recurso teamsUserActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3982b679802a2ca80eac5fe4e8f76fee91bbf1d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046346"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="ed889-103">tipo de recurso teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="ed889-103">teamsUserActivityUserCounts resource type</span></span>

<span data-ttu-id="ed889-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed889-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="ed889-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed889-105">Properties</span></span>

| <span data-ttu-id="ed889-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed889-106">Property</span></span>            | <span data-ttu-id="ed889-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed889-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="ed889-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ed889-108">reportRefreshDate</span></span>   | <span data-ttu-id="ed889-109">Data</span><span class="sxs-lookup"><span data-stu-id="ed889-109">Date</span></span>   |
| <span data-ttu-id="ed889-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="ed889-110">reportDate</span></span>          | <span data-ttu-id="ed889-111">Data</span><span class="sxs-lookup"><span data-stu-id="ed889-111">Date</span></span>   |
| <span data-ttu-id="ed889-112">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="ed889-112">teamChatMessages</span></span>    | <span data-ttu-id="ed889-113">Int64</span><span class="sxs-lookup"><span data-stu-id="ed889-113">Int64</span></span>  |
| <span data-ttu-id="ed889-114">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="ed889-114">privateChatMessages</span></span> | <span data-ttu-id="ed889-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ed889-115">Int64</span></span>  |
| <span data-ttu-id="ed889-116">calls</span><span class="sxs-lookup"><span data-stu-id="ed889-116">calls</span></span>               | <span data-ttu-id="ed889-117">Int64</span><span class="sxs-lookup"><span data-stu-id="ed889-117">Int64</span></span>  |
| <span data-ttu-id="ed889-118">treinamento</span><span class="sxs-lookup"><span data-stu-id="ed889-118">meetings</span></span>            | <span data-ttu-id="ed889-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ed889-119">Int64</span></span>  |
| <span data-ttu-id="ed889-120">otherActions</span><span class="sxs-lookup"><span data-stu-id="ed889-120">otherActions</span></span>        | <span data-ttu-id="ed889-121">Int64</span><span class="sxs-lookup"><span data-stu-id="ed889-121">Int64</span></span>  |
| <span data-ttu-id="ed889-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ed889-122">reportPeriod</span></span>        | <span data-ttu-id="ed889-123">String</span><span class="sxs-lookup"><span data-stu-id="ed889-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ed889-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed889-124">JSON representation</span></span>

<span data-ttu-id="ed889-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed889-125">The following is a JSON representation of the resource.</span></span>

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


