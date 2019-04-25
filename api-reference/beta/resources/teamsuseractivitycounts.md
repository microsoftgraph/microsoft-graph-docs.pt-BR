---
title: tipo de recurso teamsUserActivityCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcc0e9d1ed5c93c3d9f4ba97165d0413025a89cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582917"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="54c08-103">tipo de recurso teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="54c08-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="54c08-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54c08-104">Properties</span></span>

| <span data-ttu-id="54c08-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54c08-105">Property</span></span>            | <span data-ttu-id="54c08-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="54c08-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="54c08-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="54c08-107">reportRefreshDate</span></span>   | <span data-ttu-id="54c08-108">Data</span><span class="sxs-lookup"><span data-stu-id="54c08-108">Date</span></span>   |
| <span data-ttu-id="54c08-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="54c08-109">reportDate</span></span>          | <span data-ttu-id="54c08-110">Data</span><span class="sxs-lookup"><span data-stu-id="54c08-110">Date</span></span>   |
| <span data-ttu-id="54c08-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="54c08-111">teamChatMessages</span></span>    | <span data-ttu-id="54c08-112">Int64</span><span class="sxs-lookup"><span data-stu-id="54c08-112">Int64</span></span>  |
| <span data-ttu-id="54c08-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="54c08-113">privateChatMessages</span></span> | <span data-ttu-id="54c08-114">Int64</span><span class="sxs-lookup"><span data-stu-id="54c08-114">Int64</span></span>  |
| <span data-ttu-id="54c08-115">calls</span><span class="sxs-lookup"><span data-stu-id="54c08-115">calls</span></span>               | <span data-ttu-id="54c08-116">Int64</span><span class="sxs-lookup"><span data-stu-id="54c08-116">Int64</span></span>  |
| <span data-ttu-id="54c08-117">treinamento</span><span class="sxs-lookup"><span data-stu-id="54c08-117">meetings</span></span>            | <span data-ttu-id="54c08-118">Int64</span><span class="sxs-lookup"><span data-stu-id="54c08-118">Int64</span></span>  |
| <span data-ttu-id="54c08-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="54c08-119">reportPeriod</span></span>        | <span data-ttu-id="54c08-120">String</span><span class="sxs-lookup"><span data-stu-id="54c08-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="54c08-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54c08-121">JSON representation</span></span>

<span data-ttu-id="54c08-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54c08-122">The following is a JSON representation of the resource.</span></span>

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
