---
title: tipo de recurso oneDriveUsageAccountDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 6e355e1f71d493b30ffb2fe41816208dfe4816e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039283"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="6b46c-103">tipo de recurso oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="6b46c-103">oneDriveUsageAccountDetail resource type</span></span>

<span data-ttu-id="6b46c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b46c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="6b46c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b46c-105">Properties</span></span>

| <span data-ttu-id="6b46c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b46c-106">Property</span></span>                | <span data-ttu-id="6b46c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b46c-107">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="6b46c-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6b46c-108">reportRefreshDate</span></span>       | <span data-ttu-id="6b46c-109">Data</span><span class="sxs-lookup"><span data-stu-id="6b46c-109">Date</span></span>    |
| <span data-ttu-id="6b46c-110">siteUrl</span><span class="sxs-lookup"><span data-stu-id="6b46c-110">siteUrl</span></span>                 | <span data-ttu-id="6b46c-111">String</span><span class="sxs-lookup"><span data-stu-id="6b46c-111">String</span></span>  |
| <span data-ttu-id="6b46c-112">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="6b46c-112">ownerDisplayName</span></span>        | <span data-ttu-id="6b46c-113">String</span><span class="sxs-lookup"><span data-stu-id="6b46c-113">String</span></span>  |
| <span data-ttu-id="6b46c-114">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6b46c-114">ownerPrincipalName</span></span>      | <span data-ttu-id="6b46c-115">String</span><span class="sxs-lookup"><span data-stu-id="6b46c-115">String</span></span>  |
| <span data-ttu-id="6b46c-116">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6b46c-116">isDeleted</span></span>               | <span data-ttu-id="6b46c-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="6b46c-117">Boolean</span></span> |
| <span data-ttu-id="6b46c-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="6b46c-118">lastActivityDate</span></span>        | <span data-ttu-id="6b46c-119">Data</span><span class="sxs-lookup"><span data-stu-id="6b46c-119">Date</span></span>    |
| <span data-ttu-id="6b46c-120">Contagem de FileCount</span><span class="sxs-lookup"><span data-stu-id="6b46c-120">fileCount</span></span>               | <span data-ttu-id="6b46c-121">Int64</span><span class="sxs-lookup"><span data-stu-id="6b46c-121">Int64</span></span>   |
| <span data-ttu-id="6b46c-122">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="6b46c-122">activeFileCount</span></span>         | <span data-ttu-id="6b46c-123">Int64</span><span class="sxs-lookup"><span data-stu-id="6b46c-123">Int64</span></span>   |
| <span data-ttu-id="6b46c-124">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="6b46c-124">storageUsedInBytes</span></span>      | <span data-ttu-id="6b46c-125">Int64</span><span class="sxs-lookup"><span data-stu-id="6b46c-125">Int64</span></span>   |
| <span data-ttu-id="6b46c-126">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="6b46c-126">storageAllocatedInBytes</span></span> | <span data-ttu-id="6b46c-127">Int64</span><span class="sxs-lookup"><span data-stu-id="6b46c-127">Int64</span></span>   |
| <span data-ttu-id="6b46c-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6b46c-128">reportPeriod</span></span>            | <span data-ttu-id="6b46c-129">String</span><span class="sxs-lookup"><span data-stu-id="6b46c-129">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6b46c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b46c-130">JSON representation</span></span>

<span data-ttu-id="6b46c-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b46c-131">The following is a JSON representation of the resource.</span></span>

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


