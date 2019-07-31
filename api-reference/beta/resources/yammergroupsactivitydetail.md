---
title: tipo de recurso yammerGroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: f16eda3f28556a18c47c68d532ace4244edfad19
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963749"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="97e24-103">tipo de recurso yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="97e24-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="97e24-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97e24-104">Properties</span></span>

| <span data-ttu-id="97e24-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97e24-105">Property</span></span>           | <span data-ttu-id="97e24-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="97e24-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="97e24-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="97e24-107">reportRefreshDate</span></span>  | <span data-ttu-id="97e24-108">Data</span><span class="sxs-lookup"><span data-stu-id="97e24-108">Date</span></span>    |
| <span data-ttu-id="97e24-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="97e24-109">groupDisplayName</span></span>   | <span data-ttu-id="97e24-110">String</span><span class="sxs-lookup"><span data-stu-id="97e24-110">String</span></span>  |
| <span data-ttu-id="97e24-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="97e24-111">isDeleted</span></span>          | <span data-ttu-id="97e24-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="97e24-112">Boolean</span></span> |
| <span data-ttu-id="97e24-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="97e24-113">ownerPrincipalName</span></span> | <span data-ttu-id="97e24-114">String</span><span class="sxs-lookup"><span data-stu-id="97e24-114">String</span></span>  |
| <span data-ttu-id="97e24-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="97e24-115">lastActivityDate</span></span>   | <span data-ttu-id="97e24-116">Data</span><span class="sxs-lookup"><span data-stu-id="97e24-116">Date</span></span>    |
| <span data-ttu-id="97e24-117">groupType</span><span class="sxs-lookup"><span data-stu-id="97e24-117">groupType</span></span>          | <span data-ttu-id="97e24-118">String</span><span class="sxs-lookup"><span data-stu-id="97e24-118">String</span></span>  |
| <span data-ttu-id="97e24-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="97e24-119">office365Connected</span></span> | <span data-ttu-id="97e24-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="97e24-120">Boolean</span></span> |
| <span data-ttu-id="97e24-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="97e24-121">memberCount</span></span>        | <span data-ttu-id="97e24-122">Int64</span><span class="sxs-lookup"><span data-stu-id="97e24-122">Int64</span></span>   |
| <span data-ttu-id="97e24-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="97e24-123">postedCount</span></span>        | <span data-ttu-id="97e24-124">Int64</span><span class="sxs-lookup"><span data-stu-id="97e24-124">Int64</span></span>   |
| <span data-ttu-id="97e24-125">readCount</span><span class="sxs-lookup"><span data-stu-id="97e24-125">readCount</span></span>          | <span data-ttu-id="97e24-126">Int64</span><span class="sxs-lookup"><span data-stu-id="97e24-126">Int64</span></span>   |
| <span data-ttu-id="97e24-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="97e24-127">likedCount</span></span>         | <span data-ttu-id="97e24-128">Int64</span><span class="sxs-lookup"><span data-stu-id="97e24-128">Int64</span></span>   |
| <span data-ttu-id="97e24-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="97e24-129">reportPeriod</span></span>       | <span data-ttu-id="97e24-130">String</span><span class="sxs-lookup"><span data-stu-id="97e24-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="97e24-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97e24-131">JSON representation</span></span>

<span data-ttu-id="97e24-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97e24-132">The following is a JSON representation of the resource.</span></span>

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
