---
title: tipo de recurso de skypeForBusinessOrganizerActivityCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 0729aef6367ebcb0a5edfaa461d80ffd8cb0775c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041160"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a><span data-ttu-id="2954d-103">tipo de recurso de skypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="2954d-103">skypeForBusinessOrganizerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2954d-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2954d-104">Properties</span></span>

| <span data-ttu-id="2954d-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2954d-105">Property</span></span>           | <span data-ttu-id="2954d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="2954d-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="2954d-107">mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="2954d-107">im</span></span>                 | <span data-ttu-id="2954d-108">Int64</span><span class="sxs-lookup"><span data-stu-id="2954d-108">Int64</span></span>  |
| <span data-ttu-id="2954d-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="2954d-109">audioVideo</span></span>         | <span data-ttu-id="2954d-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2954d-110">Int64</span></span>  |
| <span data-ttu-id="2954d-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="2954d-111">appSharing</span></span>         | <span data-ttu-id="2954d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2954d-112">Int64</span></span>  |
| <span data-ttu-id="2954d-113">web</span><span class="sxs-lookup"><span data-stu-id="2954d-113">web</span></span>                | <span data-ttu-id="2954d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2954d-114">Int64</span></span>  |
| <span data-ttu-id="2954d-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="2954d-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="2954d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2954d-116">Int64</span></span>  |
| <span data-ttu-id="2954d-117">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="2954d-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="2954d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2954d-118">Int64</span></span>  |
| <span data-ttu-id="2954d-119">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2954d-119">reportRefreshDate</span></span>  | <span data-ttu-id="2954d-120">Data</span><span class="sxs-lookup"><span data-stu-id="2954d-120">Date</span></span>   |
| <span data-ttu-id="2954d-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="2954d-121">reportDate</span></span>         | <span data-ttu-id="2954d-122">Data</span><span class="sxs-lookup"><span data-stu-id="2954d-122">Date</span></span>   |
| <span data-ttu-id="2954d-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2954d-123">reportPeriod</span></span>       | <span data-ttu-id="2954d-124">String</span><span class="sxs-lookup"><span data-stu-id="2954d-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2954d-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2954d-125">JSON representation</span></span>

<span data-ttu-id="2954d-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2954d-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "dialInOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
