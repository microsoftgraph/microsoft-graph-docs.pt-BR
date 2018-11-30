---
title: tipo de recurso de skypeForBusinessPeerToPeerActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: ad3b409f3abc4cc9e7476825f9dbf5b7c2120d92
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038141"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="3b639-103">tipo de recurso de skypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="3b639-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3b639-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b639-104">Properties</span></span>

| <span data-ttu-id="3b639-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b639-105">Property</span></span>          | <span data-ttu-id="3b639-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b639-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="3b639-107">mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="3b639-107">im</span></span>                | <span data-ttu-id="3b639-108">Int64</span><span class="sxs-lookup"><span data-stu-id="3b639-108">Int64</span></span>  |
| <span data-ttu-id="3b639-109">audio</span><span class="sxs-lookup"><span data-stu-id="3b639-109">audio</span></span>             | <span data-ttu-id="3b639-110">Int64</span><span class="sxs-lookup"><span data-stu-id="3b639-110">Int64</span></span>  |
| <span data-ttu-id="3b639-111">video</span><span class="sxs-lookup"><span data-stu-id="3b639-111">video</span></span>             | <span data-ttu-id="3b639-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3b639-112">Int64</span></span>  |
| <span data-ttu-id="3b639-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="3b639-113">appSharing</span></span>        | <span data-ttu-id="3b639-114">Int64</span><span class="sxs-lookup"><span data-stu-id="3b639-114">Int64</span></span>  |
| <span data-ttu-id="3b639-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="3b639-115">fileTransfer</span></span>      | <span data-ttu-id="3b639-116">Int64</span><span class="sxs-lookup"><span data-stu-id="3b639-116">Int64</span></span>  |
| <span data-ttu-id="3b639-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3b639-117">reportRefreshDate</span></span> | <span data-ttu-id="3b639-118">Data</span><span class="sxs-lookup"><span data-stu-id="3b639-118">Date</span></span>   |
| <span data-ttu-id="3b639-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="3b639-119">reportDate</span></span>        | <span data-ttu-id="3b639-120">Data</span><span class="sxs-lookup"><span data-stu-id="3b639-120">Date</span></span>   |
| <span data-ttu-id="3b639-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3b639-121">reportPeriod</span></span>      | <span data-ttu-id="3b639-122">String</span><span class="sxs-lookup"><span data-stu-id="3b639-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3b639-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b639-123">JSON representation</span></span>

<span data-ttu-id="3b639-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b639-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
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
