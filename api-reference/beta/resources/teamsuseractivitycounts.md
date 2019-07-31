---
title: tipo de recurso teamsUserActivityCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9e1a40d962ded7825b72d31675cefb9869750866
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007617"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="749ec-103">tipo de recurso teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="749ec-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="749ec-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="749ec-104">Properties</span></span>

| <span data-ttu-id="749ec-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="749ec-105">Property</span></span>            | <span data-ttu-id="749ec-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="749ec-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="749ec-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="749ec-107">reportRefreshDate</span></span>   | <span data-ttu-id="749ec-108">Data</span><span class="sxs-lookup"><span data-stu-id="749ec-108">Date</span></span>   |
| <span data-ttu-id="749ec-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="749ec-109">reportDate</span></span>          | <span data-ttu-id="749ec-110">Data</span><span class="sxs-lookup"><span data-stu-id="749ec-110">Date</span></span>   |
| <span data-ttu-id="749ec-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="749ec-111">teamChatMessages</span></span>    | <span data-ttu-id="749ec-112">Int64</span><span class="sxs-lookup"><span data-stu-id="749ec-112">Int64</span></span>  |
| <span data-ttu-id="749ec-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="749ec-113">privateChatMessages</span></span> | <span data-ttu-id="749ec-114">Int64</span><span class="sxs-lookup"><span data-stu-id="749ec-114">Int64</span></span>  |
| <span data-ttu-id="749ec-115">calls</span><span class="sxs-lookup"><span data-stu-id="749ec-115">calls</span></span>               | <span data-ttu-id="749ec-116">Int64</span><span class="sxs-lookup"><span data-stu-id="749ec-116">Int64</span></span>  |
| <span data-ttu-id="749ec-117">treinamento</span><span class="sxs-lookup"><span data-stu-id="749ec-117">meetings</span></span>            | <span data-ttu-id="749ec-118">Int64</span><span class="sxs-lookup"><span data-stu-id="749ec-118">Int64</span></span>  |
| <span data-ttu-id="749ec-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="749ec-119">reportPeriod</span></span>        | <span data-ttu-id="749ec-120">String</span><span class="sxs-lookup"><span data-stu-id="749ec-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="749ec-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="749ec-121">JSON representation</span></span>

<span data-ttu-id="749ec-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="749ec-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```
