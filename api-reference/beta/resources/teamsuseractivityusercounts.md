---
title: tipo de recurso de teamsUserActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcb69c09d621ce3cce006fd9130afa0a70e4cdb8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912817"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="9683d-103">tipo de recurso de teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="9683d-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9683d-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9683d-104">Properties</span></span>

| <span data-ttu-id="9683d-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9683d-105">Property</span></span>            | <span data-ttu-id="9683d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="9683d-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="9683d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9683d-107">reportRefreshDate</span></span>   | <span data-ttu-id="9683d-108">Data</span><span class="sxs-lookup"><span data-stu-id="9683d-108">Date</span></span>   |
| <span data-ttu-id="9683d-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="9683d-109">reportDate</span></span>          | <span data-ttu-id="9683d-110">Data</span><span class="sxs-lookup"><span data-stu-id="9683d-110">Date</span></span>   |
| <span data-ttu-id="9683d-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="9683d-111">teamChatMessages</span></span>    | <span data-ttu-id="9683d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="9683d-112">Int64</span></span>  |
| <span data-ttu-id="9683d-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="9683d-113">privateChatMessages</span></span> | <span data-ttu-id="9683d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="9683d-114">Int64</span></span>  |
| <span data-ttu-id="9683d-115">chamadas</span><span class="sxs-lookup"><span data-stu-id="9683d-115">calls</span></span>               | <span data-ttu-id="9683d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="9683d-116">Int64</span></span>  |
| <span data-ttu-id="9683d-117">reuniões</span><span class="sxs-lookup"><span data-stu-id="9683d-117">meetings</span></span>            | <span data-ttu-id="9683d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="9683d-118">Int64</span></span>  |
| <span data-ttu-id="9683d-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="9683d-119">otherActions</span></span>        | <span data-ttu-id="9683d-120">Int64</span><span class="sxs-lookup"><span data-stu-id="9683d-120">Int64</span></span>  |
| <span data-ttu-id="9683d-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9683d-121">reportPeriod</span></span>        | <span data-ttu-id="9683d-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9683d-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9683d-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9683d-123">JSON representation</span></span>

<span data-ttu-id="9683d-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9683d-124">The following is a JSON representation of the resource.</span></span>

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
