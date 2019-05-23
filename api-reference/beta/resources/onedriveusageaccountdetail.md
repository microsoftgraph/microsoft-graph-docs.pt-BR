---
title: tipo de recurso oneDriveUsageAccountDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bcf75fad8c39a543e69fc378546a2621f24eaeab
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344924"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="c1255-103">tipo de recurso oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="c1255-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c1255-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1255-104">Properties</span></span>

| <span data-ttu-id="c1255-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1255-105">Property</span></span>                | <span data-ttu-id="c1255-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1255-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="c1255-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c1255-107">reportRefreshDate</span></span>       | <span data-ttu-id="c1255-108">Data</span><span class="sxs-lookup"><span data-stu-id="c1255-108">Date</span></span>    |
| <span data-ttu-id="c1255-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="c1255-109">siteUrl</span></span>                 | <span data-ttu-id="c1255-110">String</span><span class="sxs-lookup"><span data-stu-id="c1255-110">String</span></span>  |
| <span data-ttu-id="c1255-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="c1255-111">ownerDisplayName</span></span>        | <span data-ttu-id="c1255-112">String</span><span class="sxs-lookup"><span data-stu-id="c1255-112">String</span></span>  |
| <span data-ttu-id="c1255-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c1255-113">ownerPrincipalName</span></span>      | <span data-ttu-id="c1255-114">String</span><span class="sxs-lookup"><span data-stu-id="c1255-114">String</span></span>  |
| <span data-ttu-id="c1255-115">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c1255-115">isDeleted</span></span>               | <span data-ttu-id="c1255-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="c1255-116">Boolean</span></span> |
| <span data-ttu-id="c1255-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c1255-117">lastActivityDate</span></span>        | <span data-ttu-id="c1255-118">Data</span><span class="sxs-lookup"><span data-stu-id="c1255-118">Date</span></span>    |
| <span data-ttu-id="c1255-119">Contagem de FileCount</span><span class="sxs-lookup"><span data-stu-id="c1255-119">fileCount</span></span>               | <span data-ttu-id="c1255-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c1255-120">Int64</span></span>   |
| <span data-ttu-id="c1255-121">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="c1255-121">activeFileCount</span></span>         | <span data-ttu-id="c1255-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c1255-122">Int64</span></span>   |
| <span data-ttu-id="c1255-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="c1255-123">storageUsedInBytes</span></span>      | <span data-ttu-id="c1255-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c1255-124">Int64</span></span>   |
| <span data-ttu-id="c1255-125">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="c1255-125">storageAllocatedInBytes</span></span> | <span data-ttu-id="c1255-126">Int64</span><span class="sxs-lookup"><span data-stu-id="c1255-126">Int64</span></span>   |
| <span data-ttu-id="c1255-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c1255-127">reportPeriod</span></span>            | <span data-ttu-id="c1255-128">String</span><span class="sxs-lookup"><span data-stu-id="c1255-128">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c1255-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1255-129">JSON representation</span></span>

<span data-ttu-id="c1255-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1255-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "ownerPrincipalName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
