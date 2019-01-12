---
title: tipo de recurso de oneDriveUsageAccountDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957393"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="1a18e-103">tipo de recurso de oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="1a18e-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1a18e-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a18e-104">Properties</span></span>

| <span data-ttu-id="1a18e-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a18e-105">Property</span></span>                | <span data-ttu-id="1a18e-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a18e-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="1a18e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1a18e-107">reportRefreshDate</span></span>       | <span data-ttu-id="1a18e-108">Data</span><span class="sxs-lookup"><span data-stu-id="1a18e-108">Date</span></span>    |
| <span data-ttu-id="1a18e-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="1a18e-109">siteUrl</span></span>                 | <span data-ttu-id="1a18e-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a18e-110">String</span></span>  |
| <span data-ttu-id="1a18e-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="1a18e-111">ownerDisplayName</span></span>        | <span data-ttu-id="1a18e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a18e-112">String</span></span>  |
| <span data-ttu-id="1a18e-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1a18e-113">isDeleted</span></span>               | <span data-ttu-id="1a18e-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a18e-114">Boolean</span></span> |
| <span data-ttu-id="1a18e-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="1a18e-115">lastActivityDate</span></span>        | <span data-ttu-id="1a18e-116">Data</span><span class="sxs-lookup"><span data-stu-id="1a18e-116">Date</span></span>    |
| <span data-ttu-id="1a18e-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="1a18e-117">fileCount</span></span>               | <span data-ttu-id="1a18e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1a18e-118">Int64</span></span>   |
| <span data-ttu-id="1a18e-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="1a18e-119">activeFileCount</span></span>         | <span data-ttu-id="1a18e-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1a18e-120">Int64</span></span>   |
| <span data-ttu-id="1a18e-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="1a18e-121">storageUsedInBytes</span></span>      | <span data-ttu-id="1a18e-122">Int64</span><span class="sxs-lookup"><span data-stu-id="1a18e-122">Int64</span></span>   |
| <span data-ttu-id="1a18e-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="1a18e-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="1a18e-124">Int64</span><span class="sxs-lookup"><span data-stu-id="1a18e-124">Int64</span></span>   |
| <span data-ttu-id="1a18e-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1a18e-125">reportPeriod</span></span>            | <span data-ttu-id="1a18e-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a18e-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1a18e-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a18e-127">JSON representation</span></span>

<span data-ttu-id="1a18e-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a18e-128">The following is a JSON representation of the resource.</span></span>

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
