---
title: tipo de recurso de skypeForBusinessParticipantActivityCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 1e61526b281a87370835e8f6558ab3f0cb5707a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036874"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="32bec-103">tipo de recurso de skypeForBusinessParticipantActivityCounts</span><span class="sxs-lookup"><span data-stu-id="32bec-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="32bec-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32bec-104">Properties</span></span>

| <span data-ttu-id="32bec-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32bec-105">Property</span></span>          | <span data-ttu-id="32bec-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="32bec-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="32bec-107">mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="32bec-107">im</span></span>                | <span data-ttu-id="32bec-108">Int64</span><span class="sxs-lookup"><span data-stu-id="32bec-108">Int64</span></span>  |
| <span data-ttu-id="32bec-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="32bec-109">audioVideo</span></span>        | <span data-ttu-id="32bec-110">Int64</span><span class="sxs-lookup"><span data-stu-id="32bec-110">Int64</span></span>  |
| <span data-ttu-id="32bec-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="32bec-111">appSharing</span></span>        | <span data-ttu-id="32bec-112">Int64</span><span class="sxs-lookup"><span data-stu-id="32bec-112">Int64</span></span>  |
| <span data-ttu-id="32bec-113">web</span><span class="sxs-lookup"><span data-stu-id="32bec-113">web</span></span>               | <span data-ttu-id="32bec-114">Int64</span><span class="sxs-lookup"><span data-stu-id="32bec-114">Int64</span></span>  |
| <span data-ttu-id="32bec-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="32bec-115">dialInOut3rdParty</span></span> | <span data-ttu-id="32bec-116">Int64</span><span class="sxs-lookup"><span data-stu-id="32bec-116">Int64</span></span>  |
| <span data-ttu-id="32bec-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="32bec-117">reportRefreshDate</span></span> | <span data-ttu-id="32bec-118">Data</span><span class="sxs-lookup"><span data-stu-id="32bec-118">Date</span></span>   |
| <span data-ttu-id="32bec-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="32bec-119">reportDate</span></span>        | <span data-ttu-id="32bec-120">Data</span><span class="sxs-lookup"><span data-stu-id="32bec-120">Date</span></span>   |
| <span data-ttu-id="32bec-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="32bec-121">reportPeriod</span></span>      | <span data-ttu-id="32bec-122">String</span><span class="sxs-lookup"><span data-stu-id="32bec-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="32bec-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32bec-123">JSON representation</span></span>

<span data-ttu-id="32bec-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32bec-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
