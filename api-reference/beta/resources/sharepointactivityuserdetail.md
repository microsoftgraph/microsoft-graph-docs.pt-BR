---
title: tipo de recurso de sharePointActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 4503739a7b2e13cade72951ae56ab410f22608b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880693"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="1cb4b-103">tipo de recurso de sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="1cb4b-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1cb4b-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cb4b-104">Properties</span></span>

| <span data-ttu-id="1cb4b-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cb4b-105">Property</span></span>                  | <span data-ttu-id="1cb4b-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cb4b-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="1cb4b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1cb4b-107">reportRefreshDate</span></span>         | <span data-ttu-id="1cb4b-108">Data</span><span class="sxs-lookup"><span data-stu-id="1cb4b-108">Date</span></span>              |
| <span data-ttu-id="1cb4b-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1cb4b-109">userPrincipalName</span></span>         | <span data-ttu-id="1cb4b-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cb4b-110">String</span></span>            |
| <span data-ttu-id="1cb4b-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1cb4b-111">isDeleted</span></span>                 | <span data-ttu-id="1cb4b-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="1cb4b-112">Boolean</span></span>           |
| <span data-ttu-id="1cb4b-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="1cb4b-113">deletedDate</span></span>               | <span data-ttu-id="1cb4b-114">Data</span><span class="sxs-lookup"><span data-stu-id="1cb4b-114">Date</span></span>              |
| <span data-ttu-id="1cb4b-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="1cb4b-115">lastActivityDate</span></span>          | <span data-ttu-id="1cb4b-116">Data</span><span class="sxs-lookup"><span data-stu-id="1cb4b-116">Date</span></span>              |
| <span data-ttu-id="1cb4b-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="1cb4b-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="1cb4b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1cb4b-118">Int64</span></span>             |
| <span data-ttu-id="1cb4b-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="1cb4b-119">syncedFileCount</span></span>           | <span data-ttu-id="1cb4b-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1cb4b-120">Int64</span></span>             |
| <span data-ttu-id="1cb4b-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="1cb4b-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="1cb4b-122">Int64</span><span class="sxs-lookup"><span data-stu-id="1cb4b-122">Int64</span></span>             |
| <span data-ttu-id="1cb4b-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="1cb4b-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="1cb4b-124">Int64</span><span class="sxs-lookup"><span data-stu-id="1cb4b-124">Int64</span></span>             |
| <span data-ttu-id="1cb4b-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="1cb4b-125">visitedPageCount</span></span>          | <span data-ttu-id="1cb4b-126">Int64</span><span class="sxs-lookup"><span data-stu-id="1cb4b-126">Int64</span></span>             |
| <span data-ttu-id="1cb4b-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="1cb4b-127">assignedProducts</span></span>          | <span data-ttu-id="1cb4b-128">String collection</span><span class="sxs-lookup"><span data-stu-id="1cb4b-128">String collection</span></span> |
| <span data-ttu-id="1cb4b-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1cb4b-129">reportPeriod</span></span>              | <span data-ttu-id="1cb4b-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cb4b-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="1cb4b-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cb4b-131">JSON representation</span></span>

<span data-ttu-id="1cb4b-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1cb4b-132">The following is a JSON representation of the resource.</span></span>

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
