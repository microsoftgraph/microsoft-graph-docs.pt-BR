---
title: tipo de recurso oneDriveUsageAccountDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 594339072c683b053ddeb637b6f401bae2aed322
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812068"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="5a686-103">tipo de recurso oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="5a686-103">oneDriveUsageAccountDetail resource type</span></span>

<span data-ttu-id="5a686-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a686-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="5a686-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a686-105">Properties</span></span>

| <span data-ttu-id="5a686-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a686-106">Property</span></span>                | <span data-ttu-id="5a686-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a686-107">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="5a686-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5a686-108">reportRefreshDate</span></span>       | <span data-ttu-id="5a686-109">Data</span><span class="sxs-lookup"><span data-stu-id="5a686-109">Date</span></span>    |
| <span data-ttu-id="5a686-110">siteUrl</span><span class="sxs-lookup"><span data-stu-id="5a686-110">siteUrl</span></span>                 | <span data-ttu-id="5a686-111">String</span><span class="sxs-lookup"><span data-stu-id="5a686-111">String</span></span>  |
| <span data-ttu-id="5a686-112">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="5a686-112">ownerDisplayName</span></span>        | <span data-ttu-id="5a686-113">String</span><span class="sxs-lookup"><span data-stu-id="5a686-113">String</span></span>  |
| <span data-ttu-id="5a686-114">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5a686-114">ownerPrincipalName</span></span>      | <span data-ttu-id="5a686-115">String</span><span class="sxs-lookup"><span data-stu-id="5a686-115">String</span></span>  |
| <span data-ttu-id="5a686-116">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5a686-116">isDeleted</span></span>               | <span data-ttu-id="5a686-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a686-117">Boolean</span></span> |
| <span data-ttu-id="5a686-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="5a686-118">lastActivityDate</span></span>        | <span data-ttu-id="5a686-119">Data</span><span class="sxs-lookup"><span data-stu-id="5a686-119">Date</span></span>    |
| <span data-ttu-id="5a686-120">Contagem de FileCount</span><span class="sxs-lookup"><span data-stu-id="5a686-120">fileCount</span></span>               | <span data-ttu-id="5a686-121">Int64</span><span class="sxs-lookup"><span data-stu-id="5a686-121">Int64</span></span>   |
| <span data-ttu-id="5a686-122">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="5a686-122">activeFileCount</span></span>         | <span data-ttu-id="5a686-123">Int64</span><span class="sxs-lookup"><span data-stu-id="5a686-123">Int64</span></span>   |
| <span data-ttu-id="5a686-124">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="5a686-124">storageUsedInBytes</span></span>      | <span data-ttu-id="5a686-125">Int64</span><span class="sxs-lookup"><span data-stu-id="5a686-125">Int64</span></span>   |
| <span data-ttu-id="5a686-126">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="5a686-126">storageAllocatedInBytes</span></span> | <span data-ttu-id="5a686-127">Int64</span><span class="sxs-lookup"><span data-stu-id="5a686-127">Int64</span></span>   |
| <span data-ttu-id="5a686-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5a686-128">reportPeriod</span></span>            | <span data-ttu-id="5a686-129">String</span><span class="sxs-lookup"><span data-stu-id="5a686-129">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5a686-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a686-130">JSON representation</span></span>

<span data-ttu-id="5a686-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a686-131">The following is a JSON representation of the resource.</span></span>

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
