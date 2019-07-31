---
title: tipo de recurso teamsUserActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f0b6d9d77518b6e40a5793c6715bfbae69600f3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964358"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="f033b-103">tipo de recurso teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="f033b-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f033b-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f033b-104">Properties</span></span>

| <span data-ttu-id="f033b-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f033b-105">Property</span></span>            | <span data-ttu-id="f033b-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="f033b-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="f033b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f033b-107">reportRefreshDate</span></span>   | <span data-ttu-id="f033b-108">Data</span><span class="sxs-lookup"><span data-stu-id="f033b-108">Date</span></span>   |
| <span data-ttu-id="f033b-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="f033b-109">reportDate</span></span>          | <span data-ttu-id="f033b-110">Data</span><span class="sxs-lookup"><span data-stu-id="f033b-110">Date</span></span>   |
| <span data-ttu-id="f033b-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="f033b-111">teamChatMessages</span></span>    | <span data-ttu-id="f033b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f033b-112">Int64</span></span>  |
| <span data-ttu-id="f033b-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="f033b-113">privateChatMessages</span></span> | <span data-ttu-id="f033b-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f033b-114">Int64</span></span>  |
| <span data-ttu-id="f033b-115">calls</span><span class="sxs-lookup"><span data-stu-id="f033b-115">calls</span></span>               | <span data-ttu-id="f033b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f033b-116">Int64</span></span>  |
| <span data-ttu-id="f033b-117">treinamento</span><span class="sxs-lookup"><span data-stu-id="f033b-117">meetings</span></span>            | <span data-ttu-id="f033b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f033b-118">Int64</span></span>  |
| <span data-ttu-id="f033b-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="f033b-119">otherActions</span></span>        | <span data-ttu-id="f033b-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f033b-120">Int64</span></span>  |
| <span data-ttu-id="f033b-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f033b-121">reportPeriod</span></span>        | <span data-ttu-id="f033b-122">String</span><span class="sxs-lookup"><span data-stu-id="f033b-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f033b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f033b-123">JSON representation</span></span>

<span data-ttu-id="f033b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f033b-124">The following is a JSON representation of the resource.</span></span>

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
