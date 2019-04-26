---
title: tipo de recurso yammerGroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c5b580f643686c27497fd24a6fe00c7750a6a938
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551418"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="f47e5-103">tipo de recurso yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="f47e5-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f47e5-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f47e5-104">Properties</span></span>

| <span data-ttu-id="f47e5-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f47e5-105">Property</span></span>           | <span data-ttu-id="f47e5-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="f47e5-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="f47e5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f47e5-107">reportRefreshDate</span></span>  | <span data-ttu-id="f47e5-108">Data</span><span class="sxs-lookup"><span data-stu-id="f47e5-108">Date</span></span>    |
| <span data-ttu-id="f47e5-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="f47e5-109">groupDisplayName</span></span>   | <span data-ttu-id="f47e5-110">String</span><span class="sxs-lookup"><span data-stu-id="f47e5-110">String</span></span>  |
| <span data-ttu-id="f47e5-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f47e5-111">isDeleted</span></span>          | <span data-ttu-id="f47e5-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="f47e5-112">Boolean</span></span> |
| <span data-ttu-id="f47e5-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f47e5-113">ownerPrincipalName</span></span> | <span data-ttu-id="f47e5-114">String</span><span class="sxs-lookup"><span data-stu-id="f47e5-114">String</span></span>  |
| <span data-ttu-id="f47e5-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f47e5-115">lastActivityDate</span></span>   | <span data-ttu-id="f47e5-116">Data</span><span class="sxs-lookup"><span data-stu-id="f47e5-116">Date</span></span>    |
| <span data-ttu-id="f47e5-117">groupType</span><span class="sxs-lookup"><span data-stu-id="f47e5-117">groupType</span></span>          | <span data-ttu-id="f47e5-118">String</span><span class="sxs-lookup"><span data-stu-id="f47e5-118">String</span></span>  |
| <span data-ttu-id="f47e5-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="f47e5-119">office365Connected</span></span> | <span data-ttu-id="f47e5-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="f47e5-120">Boolean</span></span> |
| <span data-ttu-id="f47e5-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="f47e5-121">memberCount</span></span>        | <span data-ttu-id="f47e5-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f47e5-122">Int64</span></span>   |
| <span data-ttu-id="f47e5-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="f47e5-123">postedCount</span></span>        | <span data-ttu-id="f47e5-124">Int64</span><span class="sxs-lookup"><span data-stu-id="f47e5-124">Int64</span></span>   |
| <span data-ttu-id="f47e5-125">readCount</span><span class="sxs-lookup"><span data-stu-id="f47e5-125">readCount</span></span>          | <span data-ttu-id="f47e5-126">Int64</span><span class="sxs-lookup"><span data-stu-id="f47e5-126">Int64</span></span>   |
| <span data-ttu-id="f47e5-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="f47e5-127">likedCount</span></span>         | <span data-ttu-id="f47e5-128">Int64</span><span class="sxs-lookup"><span data-stu-id="f47e5-128">Int64</span></span>   |
| <span data-ttu-id="f47e5-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f47e5-129">reportPeriod</span></span>       | <span data-ttu-id="f47e5-130">String</span><span class="sxs-lookup"><span data-stu-id="f47e5-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f47e5-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f47e5-131">JSON representation</span></span>

<span data-ttu-id="f47e5-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f47e5-132">The following is a JSON representation of the resource.</span></span>

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
