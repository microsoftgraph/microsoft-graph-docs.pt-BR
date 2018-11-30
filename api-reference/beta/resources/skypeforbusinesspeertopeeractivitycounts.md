---
title: tipo de recurso de skypeForBusinessPeerToPeerActivityCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: cdc8ec2a63c4a03ac8b77bedba06c6addfba4584
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036466"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="4043b-103">tipo de recurso de skypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4043b-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4043b-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4043b-104">Properties</span></span>

| <span data-ttu-id="4043b-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4043b-105">Property</span></span>          | <span data-ttu-id="4043b-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4043b-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4043b-107">mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="4043b-107">im</span></span>                | <span data-ttu-id="4043b-108">Int64</span><span class="sxs-lookup"><span data-stu-id="4043b-108">Int64</span></span>  |
| <span data-ttu-id="4043b-109">audio</span><span class="sxs-lookup"><span data-stu-id="4043b-109">audio</span></span>             | <span data-ttu-id="4043b-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4043b-110">Int64</span></span>  |
| <span data-ttu-id="4043b-111">video</span><span class="sxs-lookup"><span data-stu-id="4043b-111">video</span></span>             | <span data-ttu-id="4043b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4043b-112">Int64</span></span>  |
| <span data-ttu-id="4043b-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="4043b-113">appSharing</span></span>        | <span data-ttu-id="4043b-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4043b-114">Int64</span></span>  |
| <span data-ttu-id="4043b-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="4043b-115">fileTransfer</span></span>      | <span data-ttu-id="4043b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4043b-116">Int64</span></span>  |
| <span data-ttu-id="4043b-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4043b-117">reportRefreshDate</span></span> | <span data-ttu-id="4043b-118">Data</span><span class="sxs-lookup"><span data-stu-id="4043b-118">Date</span></span>   |
| <span data-ttu-id="4043b-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="4043b-119">reportDate</span></span>        | <span data-ttu-id="4043b-120">Data</span><span class="sxs-lookup"><span data-stu-id="4043b-120">Date</span></span>   |
| <span data-ttu-id="4043b-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4043b-121">reportPeriod</span></span>      | <span data-ttu-id="4043b-122">String</span><span class="sxs-lookup"><span data-stu-id="4043b-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4043b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4043b-123">JSON representation</span></span>

<span data-ttu-id="4043b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4043b-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
