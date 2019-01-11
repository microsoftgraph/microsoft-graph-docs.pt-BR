---
title: tipo de recurso de yammerActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: d7869869466dc785b92db23f8b574eb2e77dd786
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816398"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="c8bff-103">tipo de recurso de yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="c8bff-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c8bff-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8bff-104">Properties</span></span>

| <span data-ttu-id="c8bff-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8bff-105">Property</span></span>          | <span data-ttu-id="c8bff-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8bff-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="c8bff-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c8bff-107">reportRefreshDate</span></span> | <span data-ttu-id="c8bff-108">Data</span><span class="sxs-lookup"><span data-stu-id="c8bff-108">Date</span></span>              |
| <span data-ttu-id="c8bff-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c8bff-109">userPrincipalName</span></span> | <span data-ttu-id="c8bff-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8bff-110">String</span></span>            |
| <span data-ttu-id="c8bff-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c8bff-111">displayName</span></span>       | <span data-ttu-id="c8bff-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8bff-112">String</span></span>            |
| <span data-ttu-id="c8bff-113">userState</span><span class="sxs-lookup"><span data-stu-id="c8bff-113">userState</span></span>         | <span data-ttu-id="c8bff-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8bff-114">String</span></span>            |
| <span data-ttu-id="c8bff-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="c8bff-115">stateChangeDate</span></span>   | <span data-ttu-id="c8bff-116">Data</span><span class="sxs-lookup"><span data-stu-id="c8bff-116">Date</span></span>              |
| <span data-ttu-id="c8bff-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c8bff-117">lastActivityDate</span></span>  | <span data-ttu-id="c8bff-118">Data</span><span class="sxs-lookup"><span data-stu-id="c8bff-118">Date</span></span>              |
| <span data-ttu-id="c8bff-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="c8bff-119">postedCount</span></span>       | <span data-ttu-id="c8bff-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c8bff-120">Int64</span></span>             |
| <span data-ttu-id="c8bff-121">readCount</span><span class="sxs-lookup"><span data-stu-id="c8bff-121">readCount</span></span>         | <span data-ttu-id="c8bff-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c8bff-122">Int64</span></span>             |
| <span data-ttu-id="c8bff-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="c8bff-123">likedCount</span></span>        | <span data-ttu-id="c8bff-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c8bff-124">Int64</span></span>             |
| <span data-ttu-id="c8bff-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="c8bff-125">assignedProducts</span></span>  | <span data-ttu-id="c8bff-126">String collection</span><span class="sxs-lookup"><span data-stu-id="c8bff-126">String collection</span></span> |
| <span data-ttu-id="c8bff-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c8bff-127">reportPeriod</span></span>      | <span data-ttu-id="c8bff-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8bff-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="c8bff-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8bff-129">JSON representation</span></span>

<span data-ttu-id="c8bff-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8bff-130">The following is a JSON representation of the resource.</span></span>

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
