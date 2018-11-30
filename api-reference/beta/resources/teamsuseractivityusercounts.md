---
title: tipo de recurso de teamsUserActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: f6478175252e99af2bfe5561d29eebe75b638eb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034093"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="a6055-103">tipo de recurso de teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="a6055-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a6055-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6055-104">Properties</span></span>

| <span data-ttu-id="a6055-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6055-105">Property</span></span>            | <span data-ttu-id="a6055-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6055-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="a6055-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a6055-107">reportRefreshDate</span></span>   | <span data-ttu-id="a6055-108">Data</span><span class="sxs-lookup"><span data-stu-id="a6055-108">Date</span></span>   |
| <span data-ttu-id="a6055-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="a6055-109">reportDate</span></span>          | <span data-ttu-id="a6055-110">Data</span><span class="sxs-lookup"><span data-stu-id="a6055-110">Date</span></span>   |
| <span data-ttu-id="a6055-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="a6055-111">teamChatMessages</span></span>    | <span data-ttu-id="a6055-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a6055-112">Int64</span></span>  |
| <span data-ttu-id="a6055-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="a6055-113">privateChatMessages</span></span> | <span data-ttu-id="a6055-114">Int64</span><span class="sxs-lookup"><span data-stu-id="a6055-114">Int64</span></span>  |
| <span data-ttu-id="a6055-115">chamadas</span><span class="sxs-lookup"><span data-stu-id="a6055-115">calls</span></span>               | <span data-ttu-id="a6055-116">Int64</span><span class="sxs-lookup"><span data-stu-id="a6055-116">Int64</span></span>  |
| <span data-ttu-id="a6055-117">reuniões</span><span class="sxs-lookup"><span data-stu-id="a6055-117">meetings</span></span>            | <span data-ttu-id="a6055-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a6055-118">Int64</span></span>  |
| <span data-ttu-id="a6055-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="a6055-119">otherActions</span></span>        | <span data-ttu-id="a6055-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a6055-120">Int64</span></span>  |
| <span data-ttu-id="a6055-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a6055-121">reportPeriod</span></span>        | <span data-ttu-id="a6055-122">String</span><span class="sxs-lookup"><span data-stu-id="a6055-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6055-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6055-123">JSON representation</span></span>

<span data-ttu-id="a6055-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6055-124">The following is a JSON representation of the resource.</span></span>

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
