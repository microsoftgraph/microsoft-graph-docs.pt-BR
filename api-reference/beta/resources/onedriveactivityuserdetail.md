---
title: tipo de recurso oneDriveActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 22702a392a76a21951c24667da0e8a1e61c8b36c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522390"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="c4c4a-103">tipo de recurso oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="c4c4a-103">oneDriveActivityUserDetail resource type</span></span>

<span data-ttu-id="c4c4a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c4c4a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c4c4a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4c4a-105">Properties</span></span>

| <span data-ttu-id="c4c4a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4c4a-106">Property</span></span>                  | <span data-ttu-id="c4c4a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4c4a-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="c4c4a-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c4c4a-108">reportRefreshDate</span></span>         | <span data-ttu-id="c4c4a-109">Data</span><span class="sxs-lookup"><span data-stu-id="c4c4a-109">Date</span></span>              |
| <span data-ttu-id="c4c4a-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c4c4a-110">userPrincipalName</span></span>         | <span data-ttu-id="c4c4a-111">String</span><span class="sxs-lookup"><span data-stu-id="c4c4a-111">String</span></span>            |
| <span data-ttu-id="c4c4a-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c4c4a-112">isDeleted</span></span>                 | <span data-ttu-id="c4c4a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4c4a-113">Boolean</span></span>           |
| <span data-ttu-id="c4c4a-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="c4c4a-114">deletedDate</span></span>               | <span data-ttu-id="c4c4a-115">Data</span><span class="sxs-lookup"><span data-stu-id="c4c4a-115">Date</span></span>              |
| <span data-ttu-id="c4c4a-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c4c4a-116">lastActivityDate</span></span>          | <span data-ttu-id="c4c4a-117">Data</span><span class="sxs-lookup"><span data-stu-id="c4c4a-117">Date</span></span>              |
| <span data-ttu-id="c4c4a-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="c4c4a-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="c4c4a-119">Int64</span><span class="sxs-lookup"><span data-stu-id="c4c4a-119">Int64</span></span>             |
| <span data-ttu-id="c4c4a-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="c4c4a-120">syncedFileCount</span></span>           | <span data-ttu-id="c4c4a-121">Int64</span><span class="sxs-lookup"><span data-stu-id="c4c4a-121">Int64</span></span>             |
| <span data-ttu-id="c4c4a-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="c4c4a-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="c4c4a-123">Int64</span><span class="sxs-lookup"><span data-stu-id="c4c4a-123">Int64</span></span>             |
| <span data-ttu-id="c4c4a-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="c4c4a-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="c4c4a-125">Int64</span><span class="sxs-lookup"><span data-stu-id="c4c4a-125">Int64</span></span>             |
| <span data-ttu-id="c4c4a-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="c4c4a-126">assignedProducts</span></span>          | <span data-ttu-id="c4c4a-127">String collection</span><span class="sxs-lookup"><span data-stu-id="c4c4a-127">String collection</span></span> |
| <span data-ttu-id="c4c4a-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c4c4a-128">reportPeriod</span></span>              | <span data-ttu-id="c4c4a-129">String</span><span class="sxs-lookup"><span data-stu-id="c4c4a-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="c4c4a-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c4c4a-130">JSON representation</span></span>

<span data-ttu-id="c4c4a-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c4c4a-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
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
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
