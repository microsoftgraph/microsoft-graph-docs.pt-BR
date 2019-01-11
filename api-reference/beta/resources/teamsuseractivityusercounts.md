---
title: tipo de recurso de teamsUserActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8a48a80992d8370a3b6b198862a3af901737fa04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836656"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="8281a-103">tipo de recurso de teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8281a-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8281a-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8281a-104">Properties</span></span>

| <span data-ttu-id="8281a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8281a-105">Property</span></span>            | <span data-ttu-id="8281a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="8281a-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="8281a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8281a-107">reportRefreshDate</span></span>   | <span data-ttu-id="8281a-108">Data</span><span class="sxs-lookup"><span data-stu-id="8281a-108">Date</span></span>   |
| <span data-ttu-id="8281a-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="8281a-109">reportDate</span></span>          | <span data-ttu-id="8281a-110">Data</span><span class="sxs-lookup"><span data-stu-id="8281a-110">Date</span></span>   |
| <span data-ttu-id="8281a-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="8281a-111">teamChatMessages</span></span>    | <span data-ttu-id="8281a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8281a-112">Int64</span></span>  |
| <span data-ttu-id="8281a-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="8281a-113">privateChatMessages</span></span> | <span data-ttu-id="8281a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="8281a-114">Int64</span></span>  |
| <span data-ttu-id="8281a-115">chamadas</span><span class="sxs-lookup"><span data-stu-id="8281a-115">calls</span></span>               | <span data-ttu-id="8281a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8281a-116">Int64</span></span>  |
| <span data-ttu-id="8281a-117">reuniões</span><span class="sxs-lookup"><span data-stu-id="8281a-117">meetings</span></span>            | <span data-ttu-id="8281a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="8281a-118">Int64</span></span>  |
| <span data-ttu-id="8281a-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="8281a-119">otherActions</span></span>        | <span data-ttu-id="8281a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="8281a-120">Int64</span></span>  |
| <span data-ttu-id="8281a-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8281a-121">reportPeriod</span></span>        | <span data-ttu-id="8281a-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8281a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8281a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8281a-123">JSON representation</span></span>

<span data-ttu-id="8281a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8281a-124">The following is a JSON representation of the resource.</span></span>

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
