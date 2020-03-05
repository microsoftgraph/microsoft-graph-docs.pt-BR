---
title: tipo de recurso sharePointActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: d7d030bbfaff939da4be645d8003984e5dde0a7e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520692"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="0beba-103">tipo de recurso sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="0beba-103">sharePointActivityUserDetail resource type</span></span>

<span data-ttu-id="0beba-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0beba-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="0beba-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0beba-105">Properties</span></span>

| <span data-ttu-id="0beba-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0beba-106">Property</span></span>                  | <span data-ttu-id="0beba-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0beba-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="0beba-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0beba-108">reportRefreshDate</span></span>         | <span data-ttu-id="0beba-109">Data</span><span class="sxs-lookup"><span data-stu-id="0beba-109">Date</span></span>              |
| <span data-ttu-id="0beba-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0beba-110">userPrincipalName</span></span>         | <span data-ttu-id="0beba-111">String</span><span class="sxs-lookup"><span data-stu-id="0beba-111">String</span></span>            |
| <span data-ttu-id="0beba-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="0beba-112">isDeleted</span></span>                 | <span data-ttu-id="0beba-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="0beba-113">Boolean</span></span>           |
| <span data-ttu-id="0beba-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="0beba-114">deletedDate</span></span>               | <span data-ttu-id="0beba-115">Data</span><span class="sxs-lookup"><span data-stu-id="0beba-115">Date</span></span>              |
| <span data-ttu-id="0beba-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="0beba-116">lastActivityDate</span></span>          | <span data-ttu-id="0beba-117">Data</span><span class="sxs-lookup"><span data-stu-id="0beba-117">Date</span></span>              |
| <span data-ttu-id="0beba-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="0beba-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="0beba-119">Int64</span><span class="sxs-lookup"><span data-stu-id="0beba-119">Int64</span></span>             |
| <span data-ttu-id="0beba-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="0beba-120">syncedFileCount</span></span>           | <span data-ttu-id="0beba-121">Int64</span><span class="sxs-lookup"><span data-stu-id="0beba-121">Int64</span></span>             |
| <span data-ttu-id="0beba-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="0beba-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="0beba-123">Int64</span><span class="sxs-lookup"><span data-stu-id="0beba-123">Int64</span></span>             |
| <span data-ttu-id="0beba-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="0beba-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="0beba-125">Int64</span><span class="sxs-lookup"><span data-stu-id="0beba-125">Int64</span></span>             |
| <span data-ttu-id="0beba-126">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="0beba-126">visitedPageCount</span></span>          | <span data-ttu-id="0beba-127">Int64</span><span class="sxs-lookup"><span data-stu-id="0beba-127">Int64</span></span>             |
| <span data-ttu-id="0beba-128">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="0beba-128">assignedProducts</span></span>          | <span data-ttu-id="0beba-129">String collection</span><span class="sxs-lookup"><span data-stu-id="0beba-129">String collection</span></span> |
| <span data-ttu-id="0beba-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0beba-130">reportPeriod</span></span>              | <span data-ttu-id="0beba-131">String</span><span class="sxs-lookup"><span data-stu-id="0beba-131">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="0beba-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0beba-132">JSON representation</span></span>

<span data-ttu-id="0beba-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0beba-133">The following is a JSON representation of the resource.</span></span>

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
