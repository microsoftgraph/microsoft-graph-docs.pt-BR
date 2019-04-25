---
title: tipo de recurso skypeForBusinessPeerToPeerActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 4baf218ed9398a8f208c4d1d44a28579773dea6f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523452"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="1bf88-103">tipo de recurso skypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="1bf88-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1bf88-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bf88-104">Properties</span></span>

| <span data-ttu-id="1bf88-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bf88-105">Property</span></span>          | <span data-ttu-id="1bf88-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bf88-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1bf88-107">respectiva</span><span class="sxs-lookup"><span data-stu-id="1bf88-107">im</span></span>                | <span data-ttu-id="1bf88-108">Int64</span><span class="sxs-lookup"><span data-stu-id="1bf88-108">Int64</span></span>  |
| <span data-ttu-id="1bf88-109">audio</span><span class="sxs-lookup"><span data-stu-id="1bf88-109">audio</span></span>             | <span data-ttu-id="1bf88-110">Int64</span><span class="sxs-lookup"><span data-stu-id="1bf88-110">Int64</span></span>  |
| <span data-ttu-id="1bf88-111">video</span><span class="sxs-lookup"><span data-stu-id="1bf88-111">video</span></span>             | <span data-ttu-id="1bf88-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1bf88-112">Int64</span></span>  |
| <span data-ttu-id="1bf88-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="1bf88-113">appSharing</span></span>        | <span data-ttu-id="1bf88-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1bf88-114">Int64</span></span>  |
| <span data-ttu-id="1bf88-115">transferência de</span><span class="sxs-lookup"><span data-stu-id="1bf88-115">fileTransfer</span></span>      | <span data-ttu-id="1bf88-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1bf88-116">Int64</span></span>  |
| <span data-ttu-id="1bf88-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1bf88-117">reportRefreshDate</span></span> | <span data-ttu-id="1bf88-118">Data</span><span class="sxs-lookup"><span data-stu-id="1bf88-118">Date</span></span>   |
| <span data-ttu-id="1bf88-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="1bf88-119">reportDate</span></span>        | <span data-ttu-id="1bf88-120">Data</span><span class="sxs-lookup"><span data-stu-id="1bf88-120">Date</span></span>   |
| <span data-ttu-id="1bf88-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1bf88-121">reportPeriod</span></span>      | <span data-ttu-id="1bf88-122">String</span><span class="sxs-lookup"><span data-stu-id="1bf88-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1bf88-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bf88-123">JSON representation</span></span>

<span data-ttu-id="1bf88-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1bf88-124">The following is a JSON representation of the resource.</span></span>

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
