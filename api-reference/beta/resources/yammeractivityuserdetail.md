---
title: tipo de recurso de yammerActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: a1ca33efe8327b1c1e52de25714df9c0bd45ee05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039130"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="58f0a-103">tipo de recurso de yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="58f0a-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="58f0a-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58f0a-104">Properties</span></span>

| <span data-ttu-id="58f0a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58f0a-105">Property</span></span>          | <span data-ttu-id="58f0a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="58f0a-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="58f0a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="58f0a-107">reportRefreshDate</span></span> | <span data-ttu-id="58f0a-108">Data</span><span class="sxs-lookup"><span data-stu-id="58f0a-108">Date</span></span>              |
| <span data-ttu-id="58f0a-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="58f0a-109">userPrincipalName</span></span> | <span data-ttu-id="58f0a-110">String</span><span class="sxs-lookup"><span data-stu-id="58f0a-110">String</span></span>            |
| <span data-ttu-id="58f0a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="58f0a-111">displayName</span></span>       | <span data-ttu-id="58f0a-112">String</span><span class="sxs-lookup"><span data-stu-id="58f0a-112">String</span></span>            |
| <span data-ttu-id="58f0a-113">userState</span><span class="sxs-lookup"><span data-stu-id="58f0a-113">userState</span></span>         | <span data-ttu-id="58f0a-114">String</span><span class="sxs-lookup"><span data-stu-id="58f0a-114">String</span></span>            |
| <span data-ttu-id="58f0a-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="58f0a-115">stateChangeDate</span></span>   | <span data-ttu-id="58f0a-116">Data</span><span class="sxs-lookup"><span data-stu-id="58f0a-116">Date</span></span>              |
| <span data-ttu-id="58f0a-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="58f0a-117">lastActivityDate</span></span>  | <span data-ttu-id="58f0a-118">Data</span><span class="sxs-lookup"><span data-stu-id="58f0a-118">Date</span></span>              |
| <span data-ttu-id="58f0a-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="58f0a-119">postedCount</span></span>       | <span data-ttu-id="58f0a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="58f0a-120">Int64</span></span>             |
| <span data-ttu-id="58f0a-121">readCount</span><span class="sxs-lookup"><span data-stu-id="58f0a-121">readCount</span></span>         | <span data-ttu-id="58f0a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="58f0a-122">Int64</span></span>             |
| <span data-ttu-id="58f0a-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="58f0a-123">likedCount</span></span>        | <span data-ttu-id="58f0a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="58f0a-124">Int64</span></span>             |
| <span data-ttu-id="58f0a-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="58f0a-125">assignedProducts</span></span>  | <span data-ttu-id="58f0a-126">String collection</span><span class="sxs-lookup"><span data-stu-id="58f0a-126">String collection</span></span> |
| <span data-ttu-id="58f0a-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="58f0a-127">reportPeriod</span></span>      | <span data-ttu-id="58f0a-128">String</span><span class="sxs-lookup"><span data-stu-id="58f0a-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="58f0a-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58f0a-129">JSON representation</span></span>

<span data-ttu-id="58f0a-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58f0a-130">The following is a JSON representation of the resource.</span></span>

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
