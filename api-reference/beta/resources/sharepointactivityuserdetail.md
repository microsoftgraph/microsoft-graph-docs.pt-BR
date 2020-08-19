---
title: tipo de recurso sharePointActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 20b99e3c6431d945200db868cc02302600e0e76c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807112"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="34e20-103">tipo de recurso sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="34e20-103">sharePointActivityUserDetail resource type</span></span>

<span data-ttu-id="34e20-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34e20-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="34e20-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34e20-105">Properties</span></span>

| <span data-ttu-id="34e20-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34e20-106">Property</span></span>                  | <span data-ttu-id="34e20-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="34e20-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="34e20-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="34e20-108">reportRefreshDate</span></span>         | <span data-ttu-id="34e20-109">Data</span><span class="sxs-lookup"><span data-stu-id="34e20-109">Date</span></span>              |
| <span data-ttu-id="34e20-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34e20-110">userPrincipalName</span></span>         | <span data-ttu-id="34e20-111">String</span><span class="sxs-lookup"><span data-stu-id="34e20-111">String</span></span>            |
| <span data-ttu-id="34e20-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="34e20-112">isDeleted</span></span>                 | <span data-ttu-id="34e20-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="34e20-113">Boolean</span></span>           |
| <span data-ttu-id="34e20-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="34e20-114">deletedDate</span></span>               | <span data-ttu-id="34e20-115">Data</span><span class="sxs-lookup"><span data-stu-id="34e20-115">Date</span></span>              |
| <span data-ttu-id="34e20-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="34e20-116">lastActivityDate</span></span>          | <span data-ttu-id="34e20-117">Data</span><span class="sxs-lookup"><span data-stu-id="34e20-117">Date</span></span>              |
| <span data-ttu-id="34e20-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="34e20-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="34e20-119">Int64</span><span class="sxs-lookup"><span data-stu-id="34e20-119">Int64</span></span>             |
| <span data-ttu-id="34e20-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="34e20-120">syncedFileCount</span></span>           | <span data-ttu-id="34e20-121">Int64</span><span class="sxs-lookup"><span data-stu-id="34e20-121">Int64</span></span>             |
| <span data-ttu-id="34e20-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="34e20-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="34e20-123">Int64</span><span class="sxs-lookup"><span data-stu-id="34e20-123">Int64</span></span>             |
| <span data-ttu-id="34e20-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="34e20-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="34e20-125">Int64</span><span class="sxs-lookup"><span data-stu-id="34e20-125">Int64</span></span>             |
| <span data-ttu-id="34e20-126">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="34e20-126">visitedPageCount</span></span>          | <span data-ttu-id="34e20-127">Int64</span><span class="sxs-lookup"><span data-stu-id="34e20-127">Int64</span></span>             |
| <span data-ttu-id="34e20-128">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="34e20-128">assignedProducts</span></span>          | <span data-ttu-id="34e20-129">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34e20-129">String collection</span></span> |
| <span data-ttu-id="34e20-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="34e20-130">reportPeriod</span></span>              | <span data-ttu-id="34e20-131">String</span><span class="sxs-lookup"><span data-stu-id="34e20-131">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="34e20-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34e20-132">JSON representation</span></span>

<span data-ttu-id="34e20-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34e20-133">The following is a JSON representation of the resource.</span></span>

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
