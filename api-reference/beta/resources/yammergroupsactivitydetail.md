---
title: tipo de recurso de yammerGroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 79ce924fff5d1ce9ca861c3d48589a0ecad149dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939165"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="bb1ff-103">tipo de recurso de yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="bb1ff-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bb1ff-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb1ff-104">Properties</span></span>

| <span data-ttu-id="bb1ff-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb1ff-105">Property</span></span>           | <span data-ttu-id="bb1ff-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb1ff-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="bb1ff-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bb1ff-107">reportRefreshDate</span></span>  | <span data-ttu-id="bb1ff-108">Data</span><span class="sxs-lookup"><span data-stu-id="bb1ff-108">Date</span></span>    |
| <span data-ttu-id="bb1ff-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb1ff-109">groupDisplayName</span></span>   | <span data-ttu-id="bb1ff-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb1ff-110">String</span></span>  |
| <span data-ttu-id="bb1ff-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="bb1ff-111">isDeleted</span></span>          | <span data-ttu-id="bb1ff-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb1ff-112">Boolean</span></span> |
| <span data-ttu-id="bb1ff-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb1ff-113">ownerPrincipalName</span></span> | <span data-ttu-id="bb1ff-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb1ff-114">String</span></span>  |
| <span data-ttu-id="bb1ff-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="bb1ff-115">lastActivityDate</span></span>   | <span data-ttu-id="bb1ff-116">Data</span><span class="sxs-lookup"><span data-stu-id="bb1ff-116">Date</span></span>    |
| <span data-ttu-id="bb1ff-117">groupType</span><span class="sxs-lookup"><span data-stu-id="bb1ff-117">groupType</span></span>          | <span data-ttu-id="bb1ff-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb1ff-118">String</span></span>  |
| <span data-ttu-id="bb1ff-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="bb1ff-119">office365Connected</span></span> | <span data-ttu-id="bb1ff-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb1ff-120">Boolean</span></span> |
| <span data-ttu-id="bb1ff-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="bb1ff-121">memberCount</span></span>        | <span data-ttu-id="bb1ff-122">Int64</span><span class="sxs-lookup"><span data-stu-id="bb1ff-122">Int64</span></span>   |
| <span data-ttu-id="bb1ff-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="bb1ff-123">postedCount</span></span>        | <span data-ttu-id="bb1ff-124">Int64</span><span class="sxs-lookup"><span data-stu-id="bb1ff-124">Int64</span></span>   |
| <span data-ttu-id="bb1ff-125">readCount</span><span class="sxs-lookup"><span data-stu-id="bb1ff-125">readCount</span></span>          | <span data-ttu-id="bb1ff-126">Int64</span><span class="sxs-lookup"><span data-stu-id="bb1ff-126">Int64</span></span>   |
| <span data-ttu-id="bb1ff-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="bb1ff-127">likedCount</span></span>         | <span data-ttu-id="bb1ff-128">Int64</span><span class="sxs-lookup"><span data-stu-id="bb1ff-128">Int64</span></span>   |
| <span data-ttu-id="bb1ff-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bb1ff-129">reportPeriod</span></span>       | <span data-ttu-id="bb1ff-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb1ff-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="bb1ff-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb1ff-131">JSON representation</span></span>

<span data-ttu-id="bb1ff-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb1ff-132">The following is a JSON representation of the resource.</span></span>

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
