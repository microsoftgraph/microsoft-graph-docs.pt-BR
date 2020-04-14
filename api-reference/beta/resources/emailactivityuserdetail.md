---
title: tipo de recurso emailActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 54efe4d3a24a0409e8daa2ebde6d4aff4b729118
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440566"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="d7abb-103">tipo de recurso emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d7abb-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="d7abb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7abb-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d7abb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7abb-105">Properties</span></span>

| <span data-ttu-id="d7abb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7abb-106">Property</span></span>          | <span data-ttu-id="d7abb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7abb-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="d7abb-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d7abb-108">reportRefreshDate</span></span> | <span data-ttu-id="d7abb-109">Data</span><span class="sxs-lookup"><span data-stu-id="d7abb-109">Date</span></span>              |
| <span data-ttu-id="d7abb-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d7abb-110">userPrincipalName</span></span> | <span data-ttu-id="d7abb-111">String</span><span class="sxs-lookup"><span data-stu-id="d7abb-111">String</span></span>            |
| <span data-ttu-id="d7abb-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d7abb-112">displayName</span></span>       | <span data-ttu-id="d7abb-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7abb-113">String</span></span>            |
| <span data-ttu-id="d7abb-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d7abb-114">isDeleted</span></span>         | <span data-ttu-id="d7abb-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7abb-115">Boolean</span></span>           |
| <span data-ttu-id="d7abb-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="d7abb-116">deletedDate</span></span>       | <span data-ttu-id="d7abb-117">Data</span><span class="sxs-lookup"><span data-stu-id="d7abb-117">Date</span></span>              |
| <span data-ttu-id="d7abb-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d7abb-118">lastActivityDate</span></span>  | <span data-ttu-id="d7abb-119">Data</span><span class="sxs-lookup"><span data-stu-id="d7abb-119">Date</span></span>              |
| <span data-ttu-id="d7abb-120">sendCount</span><span class="sxs-lookup"><span data-stu-id="d7abb-120">sendCount</span></span>         | <span data-ttu-id="d7abb-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d7abb-121">Int64</span></span>             |
| <span data-ttu-id="d7abb-122">receiveCount</span><span class="sxs-lookup"><span data-stu-id="d7abb-122">receiveCount</span></span>      | <span data-ttu-id="d7abb-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d7abb-123">Int64</span></span>             |
| <span data-ttu-id="d7abb-124">readCount</span><span class="sxs-lookup"><span data-stu-id="d7abb-124">readCount</span></span>         | <span data-ttu-id="d7abb-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d7abb-125">Int64</span></span>             |
| <span data-ttu-id="d7abb-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="d7abb-126">assignedProducts</span></span>  | <span data-ttu-id="d7abb-127">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d7abb-127">String collection</span></span> |
| <span data-ttu-id="d7abb-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d7abb-128">reportPeriod</span></span>      | <span data-ttu-id="d7abb-129">String</span><span class="sxs-lookup"><span data-stu-id="d7abb-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="d7abb-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7abb-130">JSON representation</span></span>

<span data-ttu-id="d7abb-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7abb-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
