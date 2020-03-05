---
title: tipo de recurso yammerGroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 9363bd711900cc6211e995c112581d3a91e08a04
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518984"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="2a322-103">tipo de recurso yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="2a322-103">yammerGroupsActivityDetail resource type</span></span>

<span data-ttu-id="2a322-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2a322-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="2a322-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a322-105">Properties</span></span>

| <span data-ttu-id="2a322-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a322-106">Property</span></span>           | <span data-ttu-id="2a322-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a322-107">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="2a322-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2a322-108">reportRefreshDate</span></span>  | <span data-ttu-id="2a322-109">Data</span><span class="sxs-lookup"><span data-stu-id="2a322-109">Date</span></span>    |
| <span data-ttu-id="2a322-110">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="2a322-110">groupDisplayName</span></span>   | <span data-ttu-id="2a322-111">String</span><span class="sxs-lookup"><span data-stu-id="2a322-111">String</span></span>  |
| <span data-ttu-id="2a322-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="2a322-112">isDeleted</span></span>          | <span data-ttu-id="2a322-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a322-113">Boolean</span></span> |
| <span data-ttu-id="2a322-114">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2a322-114">ownerPrincipalName</span></span> | <span data-ttu-id="2a322-115">String</span><span class="sxs-lookup"><span data-stu-id="2a322-115">String</span></span>  |
| <span data-ttu-id="2a322-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="2a322-116">lastActivityDate</span></span>   | <span data-ttu-id="2a322-117">Data</span><span class="sxs-lookup"><span data-stu-id="2a322-117">Date</span></span>    |
| <span data-ttu-id="2a322-118">groupType</span><span class="sxs-lookup"><span data-stu-id="2a322-118">groupType</span></span>          | <span data-ttu-id="2a322-119">String</span><span class="sxs-lookup"><span data-stu-id="2a322-119">String</span></span>  |
| <span data-ttu-id="2a322-120">office365Connected</span><span class="sxs-lookup"><span data-stu-id="2a322-120">office365Connected</span></span> | <span data-ttu-id="2a322-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a322-121">Boolean</span></span> |
| <span data-ttu-id="2a322-122">memberCount</span><span class="sxs-lookup"><span data-stu-id="2a322-122">memberCount</span></span>        | <span data-ttu-id="2a322-123">Int64</span><span class="sxs-lookup"><span data-stu-id="2a322-123">Int64</span></span>   |
| <span data-ttu-id="2a322-124">postedCount</span><span class="sxs-lookup"><span data-stu-id="2a322-124">postedCount</span></span>        | <span data-ttu-id="2a322-125">Int64</span><span class="sxs-lookup"><span data-stu-id="2a322-125">Int64</span></span>   |
| <span data-ttu-id="2a322-126">readCount</span><span class="sxs-lookup"><span data-stu-id="2a322-126">readCount</span></span>          | <span data-ttu-id="2a322-127">Int64</span><span class="sxs-lookup"><span data-stu-id="2a322-127">Int64</span></span>   |
| <span data-ttu-id="2a322-128">likedCount</span><span class="sxs-lookup"><span data-stu-id="2a322-128">likedCount</span></span>         | <span data-ttu-id="2a322-129">Int64</span><span class="sxs-lookup"><span data-stu-id="2a322-129">Int64</span></span>   |
| <span data-ttu-id="2a322-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2a322-130">reportPeriod</span></span>       | <span data-ttu-id="2a322-131">String</span><span class="sxs-lookup"><span data-stu-id="2a322-131">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="2a322-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a322-132">JSON representation</span></span>

<span data-ttu-id="2a322-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2a322-133">The following is a JSON representation of the resource.</span></span>

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
