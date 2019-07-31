---
title: tipo de recurso oneDriveUsageAccountDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: cc80110a2f8f755ef984b2f993ea660798a86743
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966465"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="4d2a9-103">tipo de recurso oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="4d2a9-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4d2a9-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d2a9-104">Properties</span></span>

| <span data-ttu-id="4d2a9-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d2a9-105">Property</span></span>                | <span data-ttu-id="4d2a9-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d2a9-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="4d2a9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4d2a9-107">reportRefreshDate</span></span>       | <span data-ttu-id="4d2a9-108">Data</span><span class="sxs-lookup"><span data-stu-id="4d2a9-108">Date</span></span>    |
| <span data-ttu-id="4d2a9-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="4d2a9-109">siteUrl</span></span>                 | <span data-ttu-id="4d2a9-110">String</span><span class="sxs-lookup"><span data-stu-id="4d2a9-110">String</span></span>  |
| <span data-ttu-id="4d2a9-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="4d2a9-111">ownerDisplayName</span></span>        | <span data-ttu-id="4d2a9-112">String</span><span class="sxs-lookup"><span data-stu-id="4d2a9-112">String</span></span>  |
| <span data-ttu-id="4d2a9-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4d2a9-113">ownerPrincipalName</span></span>      | <span data-ttu-id="4d2a9-114">String</span><span class="sxs-lookup"><span data-stu-id="4d2a9-114">String</span></span>  |
| <span data-ttu-id="4d2a9-115">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4d2a9-115">isDeleted</span></span>               | <span data-ttu-id="4d2a9-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d2a9-116">Boolean</span></span> |
| <span data-ttu-id="4d2a9-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="4d2a9-117">lastActivityDate</span></span>        | <span data-ttu-id="4d2a9-118">Data</span><span class="sxs-lookup"><span data-stu-id="4d2a9-118">Date</span></span>    |
| <span data-ttu-id="4d2a9-119">Contagem de FileCount</span><span class="sxs-lookup"><span data-stu-id="4d2a9-119">fileCount</span></span>               | <span data-ttu-id="4d2a9-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4d2a9-120">Int64</span></span>   |
| <span data-ttu-id="4d2a9-121">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="4d2a9-121">activeFileCount</span></span>         | <span data-ttu-id="4d2a9-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4d2a9-122">Int64</span></span>   |
| <span data-ttu-id="4d2a9-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="4d2a9-123">storageUsedInBytes</span></span>      | <span data-ttu-id="4d2a9-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4d2a9-124">Int64</span></span>   |
| <span data-ttu-id="4d2a9-125">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="4d2a9-125">storageAllocatedInBytes</span></span> | <span data-ttu-id="4d2a9-126">Int64</span><span class="sxs-lookup"><span data-stu-id="4d2a9-126">Int64</span></span>   |
| <span data-ttu-id="4d2a9-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4d2a9-127">reportPeriod</span></span>            | <span data-ttu-id="4d2a9-128">String</span><span class="sxs-lookup"><span data-stu-id="4d2a9-128">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="4d2a9-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d2a9-129">JSON representation</span></span>

<span data-ttu-id="4d2a9-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d2a9-130">The following is a JSON representation of the resource.</span></span>

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
