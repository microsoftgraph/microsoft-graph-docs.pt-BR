---
title: tipo de recurso de yammerGroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 9e4ac61f2af69b4229c2e9c3df7c653428cc2033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832029"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="c1058-103">tipo de recurso de yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="c1058-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c1058-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1058-104">Properties</span></span>

| <span data-ttu-id="c1058-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1058-105">Property</span></span>           | <span data-ttu-id="c1058-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1058-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="c1058-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c1058-107">reportRefreshDate</span></span>  | <span data-ttu-id="c1058-108">Data</span><span class="sxs-lookup"><span data-stu-id="c1058-108">Date</span></span>    |
| <span data-ttu-id="c1058-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="c1058-109">groupDisplayName</span></span>   | <span data-ttu-id="c1058-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1058-110">String</span></span>  |
| <span data-ttu-id="c1058-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c1058-111">isDeleted</span></span>          | <span data-ttu-id="c1058-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="c1058-112">Boolean</span></span> |
| <span data-ttu-id="c1058-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c1058-113">ownerPrincipalName</span></span> | <span data-ttu-id="c1058-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1058-114">String</span></span>  |
| <span data-ttu-id="c1058-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c1058-115">lastActivityDate</span></span>   | <span data-ttu-id="c1058-116">Data</span><span class="sxs-lookup"><span data-stu-id="c1058-116">Date</span></span>    |
| <span data-ttu-id="c1058-117">groupType</span><span class="sxs-lookup"><span data-stu-id="c1058-117">groupType</span></span>          | <span data-ttu-id="c1058-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1058-118">String</span></span>  |
| <span data-ttu-id="c1058-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="c1058-119">office365Connected</span></span> | <span data-ttu-id="c1058-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="c1058-120">Boolean</span></span> |
| <span data-ttu-id="c1058-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="c1058-121">memberCount</span></span>        | <span data-ttu-id="c1058-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c1058-122">Int64</span></span>   |
| <span data-ttu-id="c1058-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="c1058-123">postedCount</span></span>        | <span data-ttu-id="c1058-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c1058-124">Int64</span></span>   |
| <span data-ttu-id="c1058-125">readCount</span><span class="sxs-lookup"><span data-stu-id="c1058-125">readCount</span></span>          | <span data-ttu-id="c1058-126">Int64</span><span class="sxs-lookup"><span data-stu-id="c1058-126">Int64</span></span>   |
| <span data-ttu-id="c1058-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="c1058-127">likedCount</span></span>         | <span data-ttu-id="c1058-128">Int64</span><span class="sxs-lookup"><span data-stu-id="c1058-128">Int64</span></span>   |
| <span data-ttu-id="c1058-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c1058-129">reportPeriod</span></span>       | <span data-ttu-id="c1058-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1058-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c1058-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1058-131">JSON representation</span></span>

<span data-ttu-id="c1058-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1058-132">The following is a JSON representation of the resource.</span></span>

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
