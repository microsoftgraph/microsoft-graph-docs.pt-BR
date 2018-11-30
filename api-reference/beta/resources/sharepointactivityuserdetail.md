---
title: tipo de recurso de sharePointActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: a5b6de8a4a9b82d9e6d34a2ae289f0c7589798ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033807"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="b5875-103">tipo de recurso de sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b5875-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b5875-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5875-104">Properties</span></span>

| <span data-ttu-id="b5875-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5875-105">Property</span></span>                  | <span data-ttu-id="b5875-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5875-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="b5875-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b5875-107">reportRefreshDate</span></span>         | <span data-ttu-id="b5875-108">Data</span><span class="sxs-lookup"><span data-stu-id="b5875-108">Date</span></span>              |
| <span data-ttu-id="b5875-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b5875-109">userPrincipalName</span></span>         | <span data-ttu-id="b5875-110">String</span><span class="sxs-lookup"><span data-stu-id="b5875-110">String</span></span>            |
| <span data-ttu-id="b5875-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="b5875-111">isDeleted</span></span>                 | <span data-ttu-id="b5875-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5875-112">Boolean</span></span>           |
| <span data-ttu-id="b5875-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="b5875-113">deletedDate</span></span>               | <span data-ttu-id="b5875-114">Data</span><span class="sxs-lookup"><span data-stu-id="b5875-114">Date</span></span>              |
| <span data-ttu-id="b5875-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="b5875-115">lastActivityDate</span></span>          | <span data-ttu-id="b5875-116">Data</span><span class="sxs-lookup"><span data-stu-id="b5875-116">Date</span></span>              |
| <span data-ttu-id="b5875-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="b5875-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="b5875-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b5875-118">Int64</span></span>             |
| <span data-ttu-id="b5875-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="b5875-119">syncedFileCount</span></span>           | <span data-ttu-id="b5875-120">Int64</span><span class="sxs-lookup"><span data-stu-id="b5875-120">Int64</span></span>             |
| <span data-ttu-id="b5875-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="b5875-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="b5875-122">Int64</span><span class="sxs-lookup"><span data-stu-id="b5875-122">Int64</span></span>             |
| <span data-ttu-id="b5875-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="b5875-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="b5875-124">Int64</span><span class="sxs-lookup"><span data-stu-id="b5875-124">Int64</span></span>             |
| <span data-ttu-id="b5875-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="b5875-125">visitedPageCount</span></span>          | <span data-ttu-id="b5875-126">Int64</span><span class="sxs-lookup"><span data-stu-id="b5875-126">Int64</span></span>             |
| <span data-ttu-id="b5875-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="b5875-127">assignedProducts</span></span>          | <span data-ttu-id="b5875-128">String collection</span><span class="sxs-lookup"><span data-stu-id="b5875-128">String collection</span></span> |
| <span data-ttu-id="b5875-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b5875-129">reportPeriod</span></span>              | <span data-ttu-id="b5875-130">String</span><span class="sxs-lookup"><span data-stu-id="b5875-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="b5875-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5875-131">JSON representation</span></span>

<span data-ttu-id="b5875-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b5875-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "viewedOrEditedFileCount": 1024, 
  "syncedFileCount": 1024, 
  "sharedInternallyFileCount": 1024, 
  "sharedExternallyFileCount": 1024, 
  "visitedPageCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
