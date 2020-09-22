---
title: tipo de recurso sharePointActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 7394e2fab0604286e8066b64e86f413f421472cf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997792"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="66ddd-103">tipo de recurso sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="66ddd-103">sharePointActivityUserDetail resource type</span></span>

<span data-ttu-id="66ddd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66ddd-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="66ddd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66ddd-105">Properties</span></span>

| <span data-ttu-id="66ddd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66ddd-106">Property</span></span>                  | <span data-ttu-id="66ddd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="66ddd-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="66ddd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="66ddd-108">reportRefreshDate</span></span>         | <span data-ttu-id="66ddd-109">Data</span><span class="sxs-lookup"><span data-stu-id="66ddd-109">Date</span></span>              |
| <span data-ttu-id="66ddd-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="66ddd-110">userPrincipalName</span></span>         | <span data-ttu-id="66ddd-111">String</span><span class="sxs-lookup"><span data-stu-id="66ddd-111">String</span></span>            |
| <span data-ttu-id="66ddd-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="66ddd-112">isDeleted</span></span>                 | <span data-ttu-id="66ddd-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="66ddd-113">Boolean</span></span>           |
| <span data-ttu-id="66ddd-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="66ddd-114">deletedDate</span></span>               | <span data-ttu-id="66ddd-115">Data</span><span class="sxs-lookup"><span data-stu-id="66ddd-115">Date</span></span>              |
| <span data-ttu-id="66ddd-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="66ddd-116">lastActivityDate</span></span>          | <span data-ttu-id="66ddd-117">Data</span><span class="sxs-lookup"><span data-stu-id="66ddd-117">Date</span></span>              |
| <span data-ttu-id="66ddd-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="66ddd-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="66ddd-119">Int64</span><span class="sxs-lookup"><span data-stu-id="66ddd-119">Int64</span></span>             |
| <span data-ttu-id="66ddd-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="66ddd-120">syncedFileCount</span></span>           | <span data-ttu-id="66ddd-121">Int64</span><span class="sxs-lookup"><span data-stu-id="66ddd-121">Int64</span></span>             |
| <span data-ttu-id="66ddd-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="66ddd-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="66ddd-123">Int64</span><span class="sxs-lookup"><span data-stu-id="66ddd-123">Int64</span></span>             |
| <span data-ttu-id="66ddd-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="66ddd-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="66ddd-125">Int64</span><span class="sxs-lookup"><span data-stu-id="66ddd-125">Int64</span></span>             |
| <span data-ttu-id="66ddd-126">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="66ddd-126">visitedPageCount</span></span>          | <span data-ttu-id="66ddd-127">Int64</span><span class="sxs-lookup"><span data-stu-id="66ddd-127">Int64</span></span>             |
| <span data-ttu-id="66ddd-128">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="66ddd-128">assignedProducts</span></span>          | <span data-ttu-id="66ddd-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="66ddd-129">String collection</span></span> |
| <span data-ttu-id="66ddd-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="66ddd-130">reportPeriod</span></span>              | <span data-ttu-id="66ddd-131">String</span><span class="sxs-lookup"><span data-stu-id="66ddd-131">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="66ddd-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66ddd-132">JSON representation</span></span>

<span data-ttu-id="66ddd-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66ddd-133">The following is a JSON representation of the resource.</span></span>

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


