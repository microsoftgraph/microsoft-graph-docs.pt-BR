---
title: tipo de recurso de oneDriveActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 2f498c7c9507c4210f12f76d57f62729f84da578
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820787"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="bee63-103">tipo de recurso de oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="bee63-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bee63-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bee63-104">Properties</span></span>

| <span data-ttu-id="bee63-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bee63-105">Property</span></span>                  | <span data-ttu-id="bee63-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="bee63-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="bee63-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bee63-107">reportRefreshDate</span></span>         | <span data-ttu-id="bee63-108">Data</span><span class="sxs-lookup"><span data-stu-id="bee63-108">Date</span></span>              |
| <span data-ttu-id="bee63-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bee63-109">userPrincipalName</span></span>         | <span data-ttu-id="bee63-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bee63-110">String</span></span>            |
| <span data-ttu-id="bee63-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="bee63-111">isDeleted</span></span>                 | <span data-ttu-id="bee63-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="bee63-112">Boolean</span></span>           |
| <span data-ttu-id="bee63-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="bee63-113">deletedDate</span></span>               | <span data-ttu-id="bee63-114">Data</span><span class="sxs-lookup"><span data-stu-id="bee63-114">Date</span></span>              |
| <span data-ttu-id="bee63-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="bee63-115">lastActivityDate</span></span>          | <span data-ttu-id="bee63-116">Data</span><span class="sxs-lookup"><span data-stu-id="bee63-116">Date</span></span>              |
| <span data-ttu-id="bee63-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="bee63-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="bee63-118">Int64</span><span class="sxs-lookup"><span data-stu-id="bee63-118">Int64</span></span>             |
| <span data-ttu-id="bee63-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="bee63-119">syncedFileCount</span></span>           | <span data-ttu-id="bee63-120">Int64</span><span class="sxs-lookup"><span data-stu-id="bee63-120">Int64</span></span>             |
| <span data-ttu-id="bee63-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="bee63-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="bee63-122">Int64</span><span class="sxs-lookup"><span data-stu-id="bee63-122">Int64</span></span>             |
| <span data-ttu-id="bee63-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="bee63-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="bee63-124">Int64</span><span class="sxs-lookup"><span data-stu-id="bee63-124">Int64</span></span>             |
| <span data-ttu-id="bee63-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="bee63-125">assignedProducts</span></span>          | <span data-ttu-id="bee63-126">String collection</span><span class="sxs-lookup"><span data-stu-id="bee63-126">String collection</span></span> |
| <span data-ttu-id="bee63-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bee63-127">reportPeriod</span></span>              | <span data-ttu-id="bee63-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bee63-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="bee63-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bee63-129">JSON representation</span></span>

<span data-ttu-id="bee63-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bee63-130">The following is a JSON representation of the resource.</span></span>

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
