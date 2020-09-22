---
title: tipo de recurso yammerActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: eb17035f0d062d55a3607dd30f31459b79b8400c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971367"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="fc9ff-103">tipo de recurso yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="fc9ff-103">yammerActivityUserDetail resource type</span></span>

<span data-ttu-id="fc9ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc9ff-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="fc9ff-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc9ff-105">Properties</span></span>

| <span data-ttu-id="fc9ff-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc9ff-106">Property</span></span>          | <span data-ttu-id="fc9ff-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc9ff-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="fc9ff-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fc9ff-108">reportRefreshDate</span></span> | <span data-ttu-id="fc9ff-109">Data</span><span class="sxs-lookup"><span data-stu-id="fc9ff-109">Date</span></span>              |
| <span data-ttu-id="fc9ff-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fc9ff-110">userPrincipalName</span></span> | <span data-ttu-id="fc9ff-111">String</span><span class="sxs-lookup"><span data-stu-id="fc9ff-111">String</span></span>            |
| <span data-ttu-id="fc9ff-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fc9ff-112">displayName</span></span>       | <span data-ttu-id="fc9ff-113">String</span><span class="sxs-lookup"><span data-stu-id="fc9ff-113">String</span></span>            |
| <span data-ttu-id="fc9ff-114">userState</span><span class="sxs-lookup"><span data-stu-id="fc9ff-114">userState</span></span>         | <span data-ttu-id="fc9ff-115">String</span><span class="sxs-lookup"><span data-stu-id="fc9ff-115">String</span></span>            |
| <span data-ttu-id="fc9ff-116">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="fc9ff-116">stateChangeDate</span></span>   | <span data-ttu-id="fc9ff-117">Data</span><span class="sxs-lookup"><span data-stu-id="fc9ff-117">Date</span></span>              |
| <span data-ttu-id="fc9ff-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="fc9ff-118">lastActivityDate</span></span>  | <span data-ttu-id="fc9ff-119">Data</span><span class="sxs-lookup"><span data-stu-id="fc9ff-119">Date</span></span>              |
| <span data-ttu-id="fc9ff-120">postedCount</span><span class="sxs-lookup"><span data-stu-id="fc9ff-120">postedCount</span></span>       | <span data-ttu-id="fc9ff-121">Int64</span><span class="sxs-lookup"><span data-stu-id="fc9ff-121">Int64</span></span>             |
| <span data-ttu-id="fc9ff-122">readCount</span><span class="sxs-lookup"><span data-stu-id="fc9ff-122">readCount</span></span>         | <span data-ttu-id="fc9ff-123">Int64</span><span class="sxs-lookup"><span data-stu-id="fc9ff-123">Int64</span></span>             |
| <span data-ttu-id="fc9ff-124">likedCount</span><span class="sxs-lookup"><span data-stu-id="fc9ff-124">likedCount</span></span>        | <span data-ttu-id="fc9ff-125">Int64</span><span class="sxs-lookup"><span data-stu-id="fc9ff-125">Int64</span></span>             |
| <span data-ttu-id="fc9ff-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="fc9ff-126">assignedProducts</span></span>  | <span data-ttu-id="fc9ff-127">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc9ff-127">String collection</span></span> |
| <span data-ttu-id="fc9ff-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fc9ff-128">reportPeriod</span></span>      | <span data-ttu-id="fc9ff-129">String</span><span class="sxs-lookup"><span data-stu-id="fc9ff-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="fc9ff-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc9ff-130">JSON representation</span></span>

<span data-ttu-id="fc9ff-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc9ff-131">The following is a JSON representation of the resource.</span></span>

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


