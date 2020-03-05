---
title: tipo de recurso yammerActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 922ebf14f59d60a988fe77ee36ce04d9c76befec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519026"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="672a4-103">tipo de recurso yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="672a4-103">yammerActivityUserDetail resource type</span></span>

<span data-ttu-id="672a4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="672a4-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="672a4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="672a4-105">Properties</span></span>

| <span data-ttu-id="672a4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="672a4-106">Property</span></span>          | <span data-ttu-id="672a4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="672a4-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="672a4-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="672a4-108">reportRefreshDate</span></span> | <span data-ttu-id="672a4-109">Data</span><span class="sxs-lookup"><span data-stu-id="672a4-109">Date</span></span>              |
| <span data-ttu-id="672a4-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="672a4-110">userPrincipalName</span></span> | <span data-ttu-id="672a4-111">String</span><span class="sxs-lookup"><span data-stu-id="672a4-111">String</span></span>            |
| <span data-ttu-id="672a4-112">displayName</span><span class="sxs-lookup"><span data-stu-id="672a4-112">displayName</span></span>       | <span data-ttu-id="672a4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="672a4-113">String</span></span>            |
| <span data-ttu-id="672a4-114">userState</span><span class="sxs-lookup"><span data-stu-id="672a4-114">userState</span></span>         | <span data-ttu-id="672a4-115">String</span><span class="sxs-lookup"><span data-stu-id="672a4-115">String</span></span>            |
| <span data-ttu-id="672a4-116">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="672a4-116">stateChangeDate</span></span>   | <span data-ttu-id="672a4-117">Data</span><span class="sxs-lookup"><span data-stu-id="672a4-117">Date</span></span>              |
| <span data-ttu-id="672a4-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="672a4-118">lastActivityDate</span></span>  | <span data-ttu-id="672a4-119">Data</span><span class="sxs-lookup"><span data-stu-id="672a4-119">Date</span></span>              |
| <span data-ttu-id="672a4-120">postedCount</span><span class="sxs-lookup"><span data-stu-id="672a4-120">postedCount</span></span>       | <span data-ttu-id="672a4-121">Int64</span><span class="sxs-lookup"><span data-stu-id="672a4-121">Int64</span></span>             |
| <span data-ttu-id="672a4-122">readCount</span><span class="sxs-lookup"><span data-stu-id="672a4-122">readCount</span></span>         | <span data-ttu-id="672a4-123">Int64</span><span class="sxs-lookup"><span data-stu-id="672a4-123">Int64</span></span>             |
| <span data-ttu-id="672a4-124">likedCount</span><span class="sxs-lookup"><span data-stu-id="672a4-124">likedCount</span></span>        | <span data-ttu-id="672a4-125">Int64</span><span class="sxs-lookup"><span data-stu-id="672a4-125">Int64</span></span>             |
| <span data-ttu-id="672a4-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="672a4-126">assignedProducts</span></span>  | <span data-ttu-id="672a4-127">String collection</span><span class="sxs-lookup"><span data-stu-id="672a4-127">String collection</span></span> |
| <span data-ttu-id="672a4-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="672a4-128">reportPeriod</span></span>      | <span data-ttu-id="672a4-129">String</span><span class="sxs-lookup"><span data-stu-id="672a4-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="672a4-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="672a4-130">JSON representation</span></span>

<span data-ttu-id="672a4-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="672a4-131">The following is a JSON representation of the resource.</span></span>

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
