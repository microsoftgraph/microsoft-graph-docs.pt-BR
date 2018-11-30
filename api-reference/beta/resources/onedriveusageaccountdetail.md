---
title: tipo de recurso de oneDriveUsageAccountDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 4b80ebc24aa45be0368dbb59d6d3e99e7adacc8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038029"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="3d8d7-103">tipo de recurso de oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="3d8d7-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3d8d7-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d8d7-104">Properties</span></span>

| <span data-ttu-id="3d8d7-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d8d7-105">Property</span></span>                | <span data-ttu-id="3d8d7-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d8d7-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="3d8d7-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3d8d7-107">reportRefreshDate</span></span>       | <span data-ttu-id="3d8d7-108">Data</span><span class="sxs-lookup"><span data-stu-id="3d8d7-108">Date</span></span>    |
| <span data-ttu-id="3d8d7-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="3d8d7-109">siteUrl</span></span>                 | <span data-ttu-id="3d8d7-110">String</span><span class="sxs-lookup"><span data-stu-id="3d8d7-110">String</span></span>  |
| <span data-ttu-id="3d8d7-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="3d8d7-111">ownerDisplayName</span></span>        | <span data-ttu-id="3d8d7-112">String</span><span class="sxs-lookup"><span data-stu-id="3d8d7-112">String</span></span>  |
| <span data-ttu-id="3d8d7-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3d8d7-113">isDeleted</span></span>               | <span data-ttu-id="3d8d7-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="3d8d7-114">Boolean</span></span> |
| <span data-ttu-id="3d8d7-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="3d8d7-115">lastActivityDate</span></span>        | <span data-ttu-id="3d8d7-116">Data</span><span class="sxs-lookup"><span data-stu-id="3d8d7-116">Date</span></span>    |
| <span data-ttu-id="3d8d7-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="3d8d7-117">fileCount</span></span>               | <span data-ttu-id="3d8d7-118">Int64</span><span class="sxs-lookup"><span data-stu-id="3d8d7-118">Int64</span></span>   |
| <span data-ttu-id="3d8d7-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="3d8d7-119">activeFileCount</span></span>         | <span data-ttu-id="3d8d7-120">Int64</span><span class="sxs-lookup"><span data-stu-id="3d8d7-120">Int64</span></span>   |
| <span data-ttu-id="3d8d7-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="3d8d7-121">storageUsedInBytes</span></span>      | <span data-ttu-id="3d8d7-122">Int64</span><span class="sxs-lookup"><span data-stu-id="3d8d7-122">Int64</span></span>   |
| <span data-ttu-id="3d8d7-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="3d8d7-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="3d8d7-124">Int64</span><span class="sxs-lookup"><span data-stu-id="3d8d7-124">Int64</span></span>   |
| <span data-ttu-id="3d8d7-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3d8d7-125">reportPeriod</span></span>            | <span data-ttu-id="3d8d7-126">String</span><span class="sxs-lookup"><span data-stu-id="3d8d7-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="3d8d7-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d8d7-127">JSON representation</span></span>

<span data-ttu-id="3d8d7-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d8d7-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
