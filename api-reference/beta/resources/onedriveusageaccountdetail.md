---
title: tipo de recurso oneDriveUsageAccountDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563541"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="394d8-103">tipo de recurso oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="394d8-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="394d8-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="394d8-104">Properties</span></span>

| <span data-ttu-id="394d8-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="394d8-105">Property</span></span>                | <span data-ttu-id="394d8-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="394d8-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="394d8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="394d8-107">reportRefreshDate</span></span>       | <span data-ttu-id="394d8-108">Data</span><span class="sxs-lookup"><span data-stu-id="394d8-108">Date</span></span>    |
| <span data-ttu-id="394d8-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="394d8-109">siteUrl</span></span>                 | <span data-ttu-id="394d8-110">String</span><span class="sxs-lookup"><span data-stu-id="394d8-110">String</span></span>  |
| <span data-ttu-id="394d8-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="394d8-111">ownerDisplayName</span></span>        | <span data-ttu-id="394d8-112">String</span><span class="sxs-lookup"><span data-stu-id="394d8-112">String</span></span>  |
| <span data-ttu-id="394d8-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="394d8-113">isDeleted</span></span>               | <span data-ttu-id="394d8-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="394d8-114">Boolean</span></span> |
| <span data-ttu-id="394d8-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="394d8-115">lastActivityDate</span></span>        | <span data-ttu-id="394d8-116">Data</span><span class="sxs-lookup"><span data-stu-id="394d8-116">Date</span></span>    |
| <span data-ttu-id="394d8-117">Contagem de FileCount</span><span class="sxs-lookup"><span data-stu-id="394d8-117">fileCount</span></span>               | <span data-ttu-id="394d8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="394d8-118">Int64</span></span>   |
| <span data-ttu-id="394d8-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="394d8-119">activeFileCount</span></span>         | <span data-ttu-id="394d8-120">Int64</span><span class="sxs-lookup"><span data-stu-id="394d8-120">Int64</span></span>   |
| <span data-ttu-id="394d8-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="394d8-121">storageUsedInBytes</span></span>      | <span data-ttu-id="394d8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="394d8-122">Int64</span></span>   |
| <span data-ttu-id="394d8-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="394d8-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="394d8-124">Int64</span><span class="sxs-lookup"><span data-stu-id="394d8-124">Int64</span></span>   |
| <span data-ttu-id="394d8-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="394d8-125">reportPeriod</span></span>            | <span data-ttu-id="394d8-126">String</span><span class="sxs-lookup"><span data-stu-id="394d8-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="394d8-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="394d8-127">JSON representation</span></span>

<span data-ttu-id="394d8-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="394d8-128">The following is a JSON representation of the resource.</span></span>

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
