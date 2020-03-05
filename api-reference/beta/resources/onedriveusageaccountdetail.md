---
title: tipo de recurso oneDriveUsageAccountDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 21bc509fd2364365e29d1e35bcbe78d67fdc40c8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522376"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="d6d85-103">tipo de recurso oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="d6d85-103">oneDriveUsageAccountDetail resource type</span></span>

<span data-ttu-id="d6d85-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d6d85-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d6d85-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6d85-105">Properties</span></span>

| <span data-ttu-id="d6d85-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6d85-106">Property</span></span>                | <span data-ttu-id="d6d85-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6d85-107">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="d6d85-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d6d85-108">reportRefreshDate</span></span>       | <span data-ttu-id="d6d85-109">Data</span><span class="sxs-lookup"><span data-stu-id="d6d85-109">Date</span></span>    |
| <span data-ttu-id="d6d85-110">siteUrl</span><span class="sxs-lookup"><span data-stu-id="d6d85-110">siteUrl</span></span>                 | <span data-ttu-id="d6d85-111">String</span><span class="sxs-lookup"><span data-stu-id="d6d85-111">String</span></span>  |
| <span data-ttu-id="d6d85-112">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="d6d85-112">ownerDisplayName</span></span>        | <span data-ttu-id="d6d85-113">String</span><span class="sxs-lookup"><span data-stu-id="d6d85-113">String</span></span>  |
| <span data-ttu-id="d6d85-114">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d6d85-114">ownerPrincipalName</span></span>      | <span data-ttu-id="d6d85-115">String</span><span class="sxs-lookup"><span data-stu-id="d6d85-115">String</span></span>  |
| <span data-ttu-id="d6d85-116">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d6d85-116">isDeleted</span></span>               | <span data-ttu-id="d6d85-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6d85-117">Boolean</span></span> |
| <span data-ttu-id="d6d85-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d6d85-118">lastActivityDate</span></span>        | <span data-ttu-id="d6d85-119">Data</span><span class="sxs-lookup"><span data-stu-id="d6d85-119">Date</span></span>    |
| <span data-ttu-id="d6d85-120">Contagem de FileCount</span><span class="sxs-lookup"><span data-stu-id="d6d85-120">fileCount</span></span>               | <span data-ttu-id="d6d85-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d6d85-121">Int64</span></span>   |
| <span data-ttu-id="d6d85-122">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="d6d85-122">activeFileCount</span></span>         | <span data-ttu-id="d6d85-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d6d85-123">Int64</span></span>   |
| <span data-ttu-id="d6d85-124">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="d6d85-124">storageUsedInBytes</span></span>      | <span data-ttu-id="d6d85-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d6d85-125">Int64</span></span>   |
| <span data-ttu-id="d6d85-126">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="d6d85-126">storageAllocatedInBytes</span></span> | <span data-ttu-id="d6d85-127">Int64</span><span class="sxs-lookup"><span data-stu-id="d6d85-127">Int64</span></span>   |
| <span data-ttu-id="d6d85-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d6d85-128">reportPeriod</span></span>            | <span data-ttu-id="d6d85-129">String</span><span class="sxs-lookup"><span data-stu-id="d6d85-129">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d6d85-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6d85-130">JSON representation</span></span>

<span data-ttu-id="d6d85-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6d85-131">The following is a JSON representation of the resource.</span></span>

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
