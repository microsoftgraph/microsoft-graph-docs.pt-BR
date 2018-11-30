---
title: tipo de recurso de yammerGroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 9a4bb00aecb2ae1d14b68a5388e0dedc7c41b1cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034108"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="e045e-103">tipo de recurso de yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="e045e-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e045e-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e045e-104">Properties</span></span>

| <span data-ttu-id="e045e-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e045e-105">Property</span></span>           | <span data-ttu-id="e045e-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e045e-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="e045e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e045e-107">reportRefreshDate</span></span>  | <span data-ttu-id="e045e-108">Data</span><span class="sxs-lookup"><span data-stu-id="e045e-108">Date</span></span>    |
| <span data-ttu-id="e045e-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="e045e-109">groupDisplayName</span></span>   | <span data-ttu-id="e045e-110">String</span><span class="sxs-lookup"><span data-stu-id="e045e-110">String</span></span>  |
| <span data-ttu-id="e045e-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e045e-111">isDeleted</span></span>          | <span data-ttu-id="e045e-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="e045e-112">Boolean</span></span> |
| <span data-ttu-id="e045e-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e045e-113">ownerPrincipalName</span></span> | <span data-ttu-id="e045e-114">String</span><span class="sxs-lookup"><span data-stu-id="e045e-114">String</span></span>  |
| <span data-ttu-id="e045e-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e045e-115">lastActivityDate</span></span>   | <span data-ttu-id="e045e-116">Data</span><span class="sxs-lookup"><span data-stu-id="e045e-116">Date</span></span>    |
| <span data-ttu-id="e045e-117">groupType</span><span class="sxs-lookup"><span data-stu-id="e045e-117">groupType</span></span>          | <span data-ttu-id="e045e-118">String</span><span class="sxs-lookup"><span data-stu-id="e045e-118">String</span></span>  |
| <span data-ttu-id="e045e-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="e045e-119">office365Connected</span></span> | <span data-ttu-id="e045e-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="e045e-120">Boolean</span></span> |
| <span data-ttu-id="e045e-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="e045e-121">memberCount</span></span>        | <span data-ttu-id="e045e-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e045e-122">Int64</span></span>   |
| <span data-ttu-id="e045e-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="e045e-123">postedCount</span></span>        | <span data-ttu-id="e045e-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e045e-124">Int64</span></span>   |
| <span data-ttu-id="e045e-125">readCount</span><span class="sxs-lookup"><span data-stu-id="e045e-125">readCount</span></span>          | <span data-ttu-id="e045e-126">Int64</span><span class="sxs-lookup"><span data-stu-id="e045e-126">Int64</span></span>   |
| <span data-ttu-id="e045e-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="e045e-127">likedCount</span></span>         | <span data-ttu-id="e045e-128">Int64</span><span class="sxs-lookup"><span data-stu-id="e045e-128">Int64</span></span>   |
| <span data-ttu-id="e045e-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e045e-129">reportPeriod</span></span>       | <span data-ttu-id="e045e-130">String</span><span class="sxs-lookup"><span data-stu-id="e045e-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e045e-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e045e-131">JSON representation</span></span>

<span data-ttu-id="e045e-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e045e-132">The following is a JSON representation of the resource.</span></span>

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
