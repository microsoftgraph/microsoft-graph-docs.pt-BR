---
title: tipo de recurso de oneDriveUsageAccountDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 92695f509302ede4b3ce64320e8f4ed42418f7e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842606"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="9b702-103">tipo de recurso de oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="9b702-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9b702-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b702-104">Properties</span></span>

| <span data-ttu-id="9b702-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b702-105">Property</span></span>                | <span data-ttu-id="9b702-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b702-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="9b702-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9b702-107">reportRefreshDate</span></span>       | <span data-ttu-id="9b702-108">Data</span><span class="sxs-lookup"><span data-stu-id="9b702-108">Date</span></span>    |
| <span data-ttu-id="9b702-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="9b702-109">siteUrl</span></span>                 | <span data-ttu-id="9b702-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b702-110">String</span></span>  |
| <span data-ttu-id="9b702-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="9b702-111">ownerDisplayName</span></span>        | <span data-ttu-id="9b702-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b702-112">String</span></span>  |
| <span data-ttu-id="9b702-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="9b702-113">isDeleted</span></span>               | <span data-ttu-id="9b702-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="9b702-114">Boolean</span></span> |
| <span data-ttu-id="9b702-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="9b702-115">lastActivityDate</span></span>        | <span data-ttu-id="9b702-116">Data</span><span class="sxs-lookup"><span data-stu-id="9b702-116">Date</span></span>    |
| <span data-ttu-id="9b702-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="9b702-117">fileCount</span></span>               | <span data-ttu-id="9b702-118">Int64</span><span class="sxs-lookup"><span data-stu-id="9b702-118">Int64</span></span>   |
| <span data-ttu-id="9b702-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="9b702-119">activeFileCount</span></span>         | <span data-ttu-id="9b702-120">Int64</span><span class="sxs-lookup"><span data-stu-id="9b702-120">Int64</span></span>   |
| <span data-ttu-id="9b702-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="9b702-121">storageUsedInBytes</span></span>      | <span data-ttu-id="9b702-122">Int64</span><span class="sxs-lookup"><span data-stu-id="9b702-122">Int64</span></span>   |
| <span data-ttu-id="9b702-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="9b702-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="9b702-124">Int64</span><span class="sxs-lookup"><span data-stu-id="9b702-124">Int64</span></span>   |
| <span data-ttu-id="9b702-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9b702-125">reportPeriod</span></span>            | <span data-ttu-id="9b702-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b702-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9b702-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b702-127">JSON representation</span></span>

<span data-ttu-id="9b702-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b702-128">The following is a JSON representation of the resource.</span></span>

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
