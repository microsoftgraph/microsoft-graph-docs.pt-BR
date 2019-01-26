---
title: tipo de recurso de yammerGroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c5b580f643686c27497fd24a6fe00c7750a6a938
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573260"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="e6100-103">tipo de recurso de yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="e6100-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e6100-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6100-104">Properties</span></span>

| <span data-ttu-id="e6100-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6100-105">Property</span></span>           | <span data-ttu-id="e6100-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6100-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="e6100-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e6100-107">reportRefreshDate</span></span>  | <span data-ttu-id="e6100-108">Data</span><span class="sxs-lookup"><span data-stu-id="e6100-108">Date</span></span>    |
| <span data-ttu-id="e6100-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="e6100-109">groupDisplayName</span></span>   | <span data-ttu-id="e6100-110">String</span><span class="sxs-lookup"><span data-stu-id="e6100-110">String</span></span>  |
| <span data-ttu-id="e6100-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e6100-111">isDeleted</span></span>          | <span data-ttu-id="e6100-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6100-112">Boolean</span></span> |
| <span data-ttu-id="e6100-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e6100-113">ownerPrincipalName</span></span> | <span data-ttu-id="e6100-114">String</span><span class="sxs-lookup"><span data-stu-id="e6100-114">String</span></span>  |
| <span data-ttu-id="e6100-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e6100-115">lastActivityDate</span></span>   | <span data-ttu-id="e6100-116">Data</span><span class="sxs-lookup"><span data-stu-id="e6100-116">Date</span></span>    |
| <span data-ttu-id="e6100-117">groupType</span><span class="sxs-lookup"><span data-stu-id="e6100-117">groupType</span></span>          | <span data-ttu-id="e6100-118">String</span><span class="sxs-lookup"><span data-stu-id="e6100-118">String</span></span>  |
| <span data-ttu-id="e6100-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="e6100-119">office365Connected</span></span> | <span data-ttu-id="e6100-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6100-120">Boolean</span></span> |
| <span data-ttu-id="e6100-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="e6100-121">memberCount</span></span>        | <span data-ttu-id="e6100-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e6100-122">Int64</span></span>   |
| <span data-ttu-id="e6100-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="e6100-123">postedCount</span></span>        | <span data-ttu-id="e6100-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e6100-124">Int64</span></span>   |
| <span data-ttu-id="e6100-125">readCount</span><span class="sxs-lookup"><span data-stu-id="e6100-125">readCount</span></span>          | <span data-ttu-id="e6100-126">Int64</span><span class="sxs-lookup"><span data-stu-id="e6100-126">Int64</span></span>   |
| <span data-ttu-id="e6100-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="e6100-127">likedCount</span></span>         | <span data-ttu-id="e6100-128">Int64</span><span class="sxs-lookup"><span data-stu-id="e6100-128">Int64</span></span>   |
| <span data-ttu-id="e6100-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e6100-129">reportPeriod</span></span>       | <span data-ttu-id="e6100-130">String</span><span class="sxs-lookup"><span data-stu-id="e6100-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e6100-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6100-131">JSON representation</span></span>

<span data-ttu-id="e6100-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6100-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "office365Connected": true, 
  "memberCount": 1024, 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "reportPeriod": "String"
}
```
