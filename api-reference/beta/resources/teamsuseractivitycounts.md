---
title: tipo de recurso de teamsUserActivityCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 39e90b4c9dc6b9929959139ba67ddb090d143e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039797"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="87a7e-103">tipo de recurso de teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="87a7e-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="87a7e-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87a7e-104">Properties</span></span>

| <span data-ttu-id="87a7e-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87a7e-105">Property</span></span>            | <span data-ttu-id="87a7e-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="87a7e-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="87a7e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="87a7e-107">reportRefreshDate</span></span>   | <span data-ttu-id="87a7e-108">Data</span><span class="sxs-lookup"><span data-stu-id="87a7e-108">Date</span></span>   |
| <span data-ttu-id="87a7e-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="87a7e-109">reportDate</span></span>          | <span data-ttu-id="87a7e-110">Data</span><span class="sxs-lookup"><span data-stu-id="87a7e-110">Date</span></span>   |
| <span data-ttu-id="87a7e-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="87a7e-111">teamChatMessages</span></span>    | <span data-ttu-id="87a7e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="87a7e-112">Int64</span></span>  |
| <span data-ttu-id="87a7e-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="87a7e-113">privateChatMessages</span></span> | <span data-ttu-id="87a7e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="87a7e-114">Int64</span></span>  |
| <span data-ttu-id="87a7e-115">chamadas</span><span class="sxs-lookup"><span data-stu-id="87a7e-115">calls</span></span>               | <span data-ttu-id="87a7e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="87a7e-116">Int64</span></span>  |
| <span data-ttu-id="87a7e-117">reuniões</span><span class="sxs-lookup"><span data-stu-id="87a7e-117">meetings</span></span>            | <span data-ttu-id="87a7e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="87a7e-118">Int64</span></span>  |
| <span data-ttu-id="87a7e-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="87a7e-119">reportPeriod</span></span>        | <span data-ttu-id="87a7e-120">String</span><span class="sxs-lookup"><span data-stu-id="87a7e-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="87a7e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87a7e-121">JSON representation</span></span>

<span data-ttu-id="87a7e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87a7e-122">The following is a JSON representation of the resource.</span></span>

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
