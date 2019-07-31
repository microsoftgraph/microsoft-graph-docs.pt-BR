---
title: tipo de recurso oneDriveActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: c61db94678ed50e6cc93f123a506ce262616a1ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966479"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="a7c24-103">tipo de recurso oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="a7c24-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a7c24-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7c24-104">Properties</span></span>

| <span data-ttu-id="a7c24-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7c24-105">Property</span></span>                  | <span data-ttu-id="a7c24-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7c24-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="a7c24-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a7c24-107">reportRefreshDate</span></span>         | <span data-ttu-id="a7c24-108">Data</span><span class="sxs-lookup"><span data-stu-id="a7c24-108">Date</span></span>              |
| <span data-ttu-id="a7c24-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a7c24-109">userPrincipalName</span></span>         | <span data-ttu-id="a7c24-110">String</span><span class="sxs-lookup"><span data-stu-id="a7c24-110">String</span></span>            |
| <span data-ttu-id="a7c24-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a7c24-111">isDeleted</span></span>                 | <span data-ttu-id="a7c24-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="a7c24-112">Boolean</span></span>           |
| <span data-ttu-id="a7c24-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="a7c24-113">deletedDate</span></span>               | <span data-ttu-id="a7c24-114">Data</span><span class="sxs-lookup"><span data-stu-id="a7c24-114">Date</span></span>              |
| <span data-ttu-id="a7c24-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a7c24-115">lastActivityDate</span></span>          | <span data-ttu-id="a7c24-116">Data</span><span class="sxs-lookup"><span data-stu-id="a7c24-116">Date</span></span>              |
| <span data-ttu-id="a7c24-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="a7c24-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="a7c24-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a7c24-118">Int64</span></span>             |
| <span data-ttu-id="a7c24-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="a7c24-119">syncedFileCount</span></span>           | <span data-ttu-id="a7c24-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a7c24-120">Int64</span></span>             |
| <span data-ttu-id="a7c24-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="a7c24-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="a7c24-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a7c24-122">Int64</span></span>             |
| <span data-ttu-id="a7c24-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="a7c24-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="a7c24-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a7c24-124">Int64</span></span>             |
| <span data-ttu-id="a7c24-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="a7c24-125">assignedProducts</span></span>          | <span data-ttu-id="a7c24-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7c24-126">String collection</span></span> |
| <span data-ttu-id="a7c24-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a7c24-127">reportPeriod</span></span>              | <span data-ttu-id="a7c24-128">String</span><span class="sxs-lookup"><span data-stu-id="a7c24-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="a7c24-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7c24-129">JSON representation</span></span>

<span data-ttu-id="a7c24-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7c24-130">The following is a JSON representation of the resource.</span></span>

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
