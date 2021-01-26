---
title: Tipo de recurso yammerGroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: cb4f04b04d59a5b14185e82d47c5366f3e2890e4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982338"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="748df-103">Tipo de recurso yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="748df-103">yammerGroupsActivityDetail resource type</span></span>

<span data-ttu-id="748df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="748df-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="748df-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="748df-105">Properties</span></span>

| <span data-ttu-id="748df-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="748df-106">Property</span></span>           | <span data-ttu-id="748df-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="748df-107">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="748df-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="748df-108">reportRefreshDate</span></span>  | <span data-ttu-id="748df-109">Data</span><span class="sxs-lookup"><span data-stu-id="748df-109">Date</span></span>    |
| <span data-ttu-id="748df-110">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="748df-110">groupDisplayName</span></span>   | <span data-ttu-id="748df-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="748df-111">String</span></span>  |
| <span data-ttu-id="748df-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="748df-112">isDeleted</span></span>          | <span data-ttu-id="748df-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="748df-113">Boolean</span></span> |
| <span data-ttu-id="748df-114">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="748df-114">ownerPrincipalName</span></span> | <span data-ttu-id="748df-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="748df-115">String</span></span>  |
| <span data-ttu-id="748df-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="748df-116">lastActivityDate</span></span>   | <span data-ttu-id="748df-117">Data</span><span class="sxs-lookup"><span data-stu-id="748df-117">Date</span></span>    |
| <span data-ttu-id="748df-118">groupType</span><span class="sxs-lookup"><span data-stu-id="748df-118">groupType</span></span>          | <span data-ttu-id="748df-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="748df-119">String</span></span>  |
| <span data-ttu-id="748df-120">office365Connected</span><span class="sxs-lookup"><span data-stu-id="748df-120">office365Connected</span></span> | <span data-ttu-id="748df-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="748df-121">Boolean</span></span> |
| <span data-ttu-id="748df-122">memberCount</span><span class="sxs-lookup"><span data-stu-id="748df-122">memberCount</span></span>        | <span data-ttu-id="748df-123">Int64</span><span class="sxs-lookup"><span data-stu-id="748df-123">Int64</span></span>   |
| <span data-ttu-id="748df-124">postedCount</span><span class="sxs-lookup"><span data-stu-id="748df-124">postedCount</span></span>        | <span data-ttu-id="748df-125">Int64</span><span class="sxs-lookup"><span data-stu-id="748df-125">Int64</span></span>   |
| <span data-ttu-id="748df-126">readCount</span><span class="sxs-lookup"><span data-stu-id="748df-126">readCount</span></span>          | <span data-ttu-id="748df-127">Int64</span><span class="sxs-lookup"><span data-stu-id="748df-127">Int64</span></span>   |
| <span data-ttu-id="748df-128">likedCount</span><span class="sxs-lookup"><span data-stu-id="748df-128">likedCount</span></span>         | <span data-ttu-id="748df-129">Int64</span><span class="sxs-lookup"><span data-stu-id="748df-129">Int64</span></span>   |
| <span data-ttu-id="748df-130">networkDisplayName</span><span class="sxs-lookup"><span data-stu-id="748df-130">networkDisplayName</span></span> | <span data-ttu-id="748df-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="748df-131">String</span></span>  |
| <span data-ttu-id="748df-132">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="748df-132">reportPeriod</span></span>       | <span data-ttu-id="748df-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="748df-133">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="748df-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="748df-134">JSON representation</span></span>

<span data-ttu-id="748df-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="748df-135">The following is a JSON representation of the resource.</span></span>

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
  "networkDisplayName": "String",
  "reportPeriod": "String"
}
```


