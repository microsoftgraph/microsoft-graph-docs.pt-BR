---
title: tipo de recurso de oneDriveActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29c9c8b723d4f87fa9858e26906878c973b37b09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948244"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="4b0e1-103">tipo de recurso de oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="4b0e1-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4b0e1-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b0e1-104">Properties</span></span>

| <span data-ttu-id="4b0e1-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b0e1-105">Property</span></span>                  | <span data-ttu-id="4b0e1-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b0e1-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="4b0e1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4b0e1-107">reportRefreshDate</span></span>         | <span data-ttu-id="4b0e1-108">Data</span><span class="sxs-lookup"><span data-stu-id="4b0e1-108">Date</span></span>              |
| <span data-ttu-id="4b0e1-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4b0e1-109">userPrincipalName</span></span>         | <span data-ttu-id="4b0e1-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b0e1-110">String</span></span>            |
| <span data-ttu-id="4b0e1-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4b0e1-111">isDeleted</span></span>                 | <span data-ttu-id="4b0e1-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="4b0e1-112">Boolean</span></span>           |
| <span data-ttu-id="4b0e1-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="4b0e1-113">deletedDate</span></span>               | <span data-ttu-id="4b0e1-114">Data</span><span class="sxs-lookup"><span data-stu-id="4b0e1-114">Date</span></span>              |
| <span data-ttu-id="4b0e1-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="4b0e1-115">lastActivityDate</span></span>          | <span data-ttu-id="4b0e1-116">Data</span><span class="sxs-lookup"><span data-stu-id="4b0e1-116">Date</span></span>              |
| <span data-ttu-id="4b0e1-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="4b0e1-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="4b0e1-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4b0e1-118">Int64</span></span>             |
| <span data-ttu-id="4b0e1-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="4b0e1-119">syncedFileCount</span></span>           | <span data-ttu-id="4b0e1-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4b0e1-120">Int64</span></span>             |
| <span data-ttu-id="4b0e1-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="4b0e1-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="4b0e1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4b0e1-122">Int64</span></span>             |
| <span data-ttu-id="4b0e1-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="4b0e1-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="4b0e1-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4b0e1-124">Int64</span></span>             |
| <span data-ttu-id="4b0e1-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="4b0e1-125">assignedProducts</span></span>          | <span data-ttu-id="4b0e1-126">String collection</span><span class="sxs-lookup"><span data-stu-id="4b0e1-126">String collection</span></span> |
| <span data-ttu-id="4b0e1-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4b0e1-127">reportPeriod</span></span>              | <span data-ttu-id="4b0e1-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b0e1-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="4b0e1-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b0e1-129">JSON representation</span></span>

<span data-ttu-id="4b0e1-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b0e1-130">The following is a JSON representation of the resource.</span></span>

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
