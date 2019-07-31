---
title: tipo de recurso sharePointActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 3d1c1f1b2bcf919769009bbb65a917c4b9cb84f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008429"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="b1bf8-103">tipo de recurso sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b1bf8-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b1bf8-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1bf8-104">Properties</span></span>

| <span data-ttu-id="b1bf8-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1bf8-105">Property</span></span>                  | <span data-ttu-id="b1bf8-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1bf8-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="b1bf8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b1bf8-107">reportRefreshDate</span></span>         | <span data-ttu-id="b1bf8-108">Data</span><span class="sxs-lookup"><span data-stu-id="b1bf8-108">Date</span></span>              |
| <span data-ttu-id="b1bf8-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1bf8-109">userPrincipalName</span></span>         | <span data-ttu-id="b1bf8-110">String</span><span class="sxs-lookup"><span data-stu-id="b1bf8-110">String</span></span>            |
| <span data-ttu-id="b1bf8-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="b1bf8-111">isDeleted</span></span>                 | <span data-ttu-id="b1bf8-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1bf8-112">Boolean</span></span>           |
| <span data-ttu-id="b1bf8-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="b1bf8-113">deletedDate</span></span>               | <span data-ttu-id="b1bf8-114">Data</span><span class="sxs-lookup"><span data-stu-id="b1bf8-114">Date</span></span>              |
| <span data-ttu-id="b1bf8-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="b1bf8-115">lastActivityDate</span></span>          | <span data-ttu-id="b1bf8-116">Data</span><span class="sxs-lookup"><span data-stu-id="b1bf8-116">Date</span></span>              |
| <span data-ttu-id="b1bf8-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="b1bf8-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="b1bf8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b1bf8-118">Int64</span></span>             |
| <span data-ttu-id="b1bf8-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="b1bf8-119">syncedFileCount</span></span>           | <span data-ttu-id="b1bf8-120">Int64</span><span class="sxs-lookup"><span data-stu-id="b1bf8-120">Int64</span></span>             |
| <span data-ttu-id="b1bf8-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="b1bf8-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="b1bf8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="b1bf8-122">Int64</span></span>             |
| <span data-ttu-id="b1bf8-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="b1bf8-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="b1bf8-124">Int64</span><span class="sxs-lookup"><span data-stu-id="b1bf8-124">Int64</span></span>             |
| <span data-ttu-id="b1bf8-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="b1bf8-125">visitedPageCount</span></span>          | <span data-ttu-id="b1bf8-126">Int64</span><span class="sxs-lookup"><span data-stu-id="b1bf8-126">Int64</span></span>             |
| <span data-ttu-id="b1bf8-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="b1bf8-127">assignedProducts</span></span>          | <span data-ttu-id="b1bf8-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1bf8-128">String collection</span></span> |
| <span data-ttu-id="b1bf8-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b1bf8-129">reportPeriod</span></span>              | <span data-ttu-id="b1bf8-130">String</span><span class="sxs-lookup"><span data-stu-id="b1bf8-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="b1bf8-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1bf8-131">JSON representation</span></span>

<span data-ttu-id="b1bf8-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1bf8-132">The following is a JSON representation of the resource.</span></span>

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
