---
title: tipo de recurso de yammerActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea520e6024bb050001461fb5ada5c90ea2b2125
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575825"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="4e664-103">tipo de recurso de yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="4e664-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4e664-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e664-104">Properties</span></span>

| <span data-ttu-id="4e664-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e664-105">Property</span></span>          | <span data-ttu-id="4e664-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e664-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="4e664-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4e664-107">reportRefreshDate</span></span> | <span data-ttu-id="4e664-108">Data</span><span class="sxs-lookup"><span data-stu-id="4e664-108">Date</span></span>              |
| <span data-ttu-id="4e664-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4e664-109">userPrincipalName</span></span> | <span data-ttu-id="4e664-110">String</span><span class="sxs-lookup"><span data-stu-id="4e664-110">String</span></span>            |
| <span data-ttu-id="4e664-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4e664-111">displayName</span></span>       | <span data-ttu-id="4e664-112">String</span><span class="sxs-lookup"><span data-stu-id="4e664-112">String</span></span>            |
| <span data-ttu-id="4e664-113">userState</span><span class="sxs-lookup"><span data-stu-id="4e664-113">userState</span></span>         | <span data-ttu-id="4e664-114">String</span><span class="sxs-lookup"><span data-stu-id="4e664-114">String</span></span>            |
| <span data-ttu-id="4e664-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="4e664-115">stateChangeDate</span></span>   | <span data-ttu-id="4e664-116">Data</span><span class="sxs-lookup"><span data-stu-id="4e664-116">Date</span></span>              |
| <span data-ttu-id="4e664-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="4e664-117">lastActivityDate</span></span>  | <span data-ttu-id="4e664-118">Data</span><span class="sxs-lookup"><span data-stu-id="4e664-118">Date</span></span>              |
| <span data-ttu-id="4e664-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="4e664-119">postedCount</span></span>       | <span data-ttu-id="4e664-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4e664-120">Int64</span></span>             |
| <span data-ttu-id="4e664-121">readCount</span><span class="sxs-lookup"><span data-stu-id="4e664-121">readCount</span></span>         | <span data-ttu-id="4e664-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4e664-122">Int64</span></span>             |
| <span data-ttu-id="4e664-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="4e664-123">likedCount</span></span>        | <span data-ttu-id="4e664-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4e664-124">Int64</span></span>             |
| <span data-ttu-id="4e664-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="4e664-125">assignedProducts</span></span>  | <span data-ttu-id="4e664-126">String collection</span><span class="sxs-lookup"><span data-stu-id="4e664-126">String collection</span></span> |
| <span data-ttu-id="4e664-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4e664-127">reportPeriod</span></span>      | <span data-ttu-id="4e664-128">String</span><span class="sxs-lookup"><span data-stu-id="4e664-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="4e664-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e664-129">JSON representation</span></span>

<span data-ttu-id="4e664-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e664-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
