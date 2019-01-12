---
title: tipo de recurso de sharePointActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7dc324d821dca26ff1083f1e48c258e1955d72f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979940"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="209f9-103">tipo de recurso de sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="209f9-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="209f9-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="209f9-104">Properties</span></span>

| <span data-ttu-id="209f9-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="209f9-105">Property</span></span>                  | <span data-ttu-id="209f9-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="209f9-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="209f9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="209f9-107">reportRefreshDate</span></span>         | <span data-ttu-id="209f9-108">Data</span><span class="sxs-lookup"><span data-stu-id="209f9-108">Date</span></span>              |
| <span data-ttu-id="209f9-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="209f9-109">userPrincipalName</span></span>         | <span data-ttu-id="209f9-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="209f9-110">String</span></span>            |
| <span data-ttu-id="209f9-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="209f9-111">isDeleted</span></span>                 | <span data-ttu-id="209f9-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="209f9-112">Boolean</span></span>           |
| <span data-ttu-id="209f9-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="209f9-113">deletedDate</span></span>               | <span data-ttu-id="209f9-114">Data</span><span class="sxs-lookup"><span data-stu-id="209f9-114">Date</span></span>              |
| <span data-ttu-id="209f9-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="209f9-115">lastActivityDate</span></span>          | <span data-ttu-id="209f9-116">Data</span><span class="sxs-lookup"><span data-stu-id="209f9-116">Date</span></span>              |
| <span data-ttu-id="209f9-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="209f9-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="209f9-118">Int64</span><span class="sxs-lookup"><span data-stu-id="209f9-118">Int64</span></span>             |
| <span data-ttu-id="209f9-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="209f9-119">syncedFileCount</span></span>           | <span data-ttu-id="209f9-120">Int64</span><span class="sxs-lookup"><span data-stu-id="209f9-120">Int64</span></span>             |
| <span data-ttu-id="209f9-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="209f9-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="209f9-122">Int64</span><span class="sxs-lookup"><span data-stu-id="209f9-122">Int64</span></span>             |
| <span data-ttu-id="209f9-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="209f9-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="209f9-124">Int64</span><span class="sxs-lookup"><span data-stu-id="209f9-124">Int64</span></span>             |
| <span data-ttu-id="209f9-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="209f9-125">visitedPageCount</span></span>          | <span data-ttu-id="209f9-126">Int64</span><span class="sxs-lookup"><span data-stu-id="209f9-126">Int64</span></span>             |
| <span data-ttu-id="209f9-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="209f9-127">assignedProducts</span></span>          | <span data-ttu-id="209f9-128">String collection</span><span class="sxs-lookup"><span data-stu-id="209f9-128">String collection</span></span> |
| <span data-ttu-id="209f9-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="209f9-129">reportPeriod</span></span>              | <span data-ttu-id="209f9-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="209f9-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="209f9-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="209f9-131">JSON representation</span></span>

<span data-ttu-id="209f9-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="209f9-132">The following is a JSON representation of the resource.</span></span>

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
