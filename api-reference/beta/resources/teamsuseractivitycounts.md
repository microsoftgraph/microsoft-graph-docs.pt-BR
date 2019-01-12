---
title: tipo de recurso de teamsUserActivityCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcc0e9d1ed5c93c3d9f4ba97165d0413025a89cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987521"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="0502c-103">tipo de recurso de teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="0502c-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0502c-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0502c-104">Properties</span></span>

| <span data-ttu-id="0502c-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0502c-105">Property</span></span>            | <span data-ttu-id="0502c-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="0502c-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="0502c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0502c-107">reportRefreshDate</span></span>   | <span data-ttu-id="0502c-108">Data</span><span class="sxs-lookup"><span data-stu-id="0502c-108">Date</span></span>   |
| <span data-ttu-id="0502c-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="0502c-109">reportDate</span></span>          | <span data-ttu-id="0502c-110">Data</span><span class="sxs-lookup"><span data-stu-id="0502c-110">Date</span></span>   |
| <span data-ttu-id="0502c-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="0502c-111">teamChatMessages</span></span>    | <span data-ttu-id="0502c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0502c-112">Int64</span></span>  |
| <span data-ttu-id="0502c-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="0502c-113">privateChatMessages</span></span> | <span data-ttu-id="0502c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="0502c-114">Int64</span></span>  |
| <span data-ttu-id="0502c-115">chamadas</span><span class="sxs-lookup"><span data-stu-id="0502c-115">calls</span></span>               | <span data-ttu-id="0502c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="0502c-116">Int64</span></span>  |
| <span data-ttu-id="0502c-117">reuniões</span><span class="sxs-lookup"><span data-stu-id="0502c-117">meetings</span></span>            | <span data-ttu-id="0502c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="0502c-118">Int64</span></span>  |
| <span data-ttu-id="0502c-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0502c-119">reportPeriod</span></span>        | <span data-ttu-id="0502c-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0502c-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="0502c-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0502c-121">JSON representation</span></span>

<span data-ttu-id="0502c-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0502c-122">The following is a JSON representation of the resource.</span></span>

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
