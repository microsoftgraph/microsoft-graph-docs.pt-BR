---
title: tipo de recurso teamsUserActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcb69c09d621ce3cce006fd9130afa0a70e4cdb8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582910"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="3d858-103">tipo de recurso teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="3d858-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3d858-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d858-104">Properties</span></span>

| <span data-ttu-id="3d858-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d858-105">Property</span></span>            | <span data-ttu-id="3d858-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d858-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="3d858-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3d858-107">reportRefreshDate</span></span>   | <span data-ttu-id="3d858-108">Data</span><span class="sxs-lookup"><span data-stu-id="3d858-108">Date</span></span>   |
| <span data-ttu-id="3d858-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="3d858-109">reportDate</span></span>          | <span data-ttu-id="3d858-110">Data</span><span class="sxs-lookup"><span data-stu-id="3d858-110">Date</span></span>   |
| <span data-ttu-id="3d858-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="3d858-111">teamChatMessages</span></span>    | <span data-ttu-id="3d858-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3d858-112">Int64</span></span>  |
| <span data-ttu-id="3d858-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="3d858-113">privateChatMessages</span></span> | <span data-ttu-id="3d858-114">Int64</span><span class="sxs-lookup"><span data-stu-id="3d858-114">Int64</span></span>  |
| <span data-ttu-id="3d858-115">calls</span><span class="sxs-lookup"><span data-stu-id="3d858-115">calls</span></span>               | <span data-ttu-id="3d858-116">Int64</span><span class="sxs-lookup"><span data-stu-id="3d858-116">Int64</span></span>  |
| <span data-ttu-id="3d858-117">treinamento</span><span class="sxs-lookup"><span data-stu-id="3d858-117">meetings</span></span>            | <span data-ttu-id="3d858-118">Int64</span><span class="sxs-lookup"><span data-stu-id="3d858-118">Int64</span></span>  |
| <span data-ttu-id="3d858-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="3d858-119">otherActions</span></span>        | <span data-ttu-id="3d858-120">Int64</span><span class="sxs-lookup"><span data-stu-id="3d858-120">Int64</span></span>  |
| <span data-ttu-id="3d858-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3d858-121">reportPeriod</span></span>        | <span data-ttu-id="3d858-122">String</span><span class="sxs-lookup"><span data-stu-id="3d858-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3d858-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d858-123">JSON representation</span></span>

<span data-ttu-id="3d858-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d858-124">The following is a JSON representation of the resource.</span></span>

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
