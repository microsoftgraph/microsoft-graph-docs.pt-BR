---
title: tipo de recurso emailActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 76ec180ceb239f79c420f26b48521e9bc7e81787
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979480"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="8e19e-103">tipo de recurso emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="8e19e-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="8e19e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e19e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="8e19e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e19e-105">Properties</span></span>

| <span data-ttu-id="8e19e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e19e-106">Property</span></span>          | <span data-ttu-id="8e19e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e19e-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="8e19e-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8e19e-108">reportRefreshDate</span></span> | <span data-ttu-id="8e19e-109">Data</span><span class="sxs-lookup"><span data-stu-id="8e19e-109">Date</span></span>              |
| <span data-ttu-id="8e19e-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8e19e-110">userPrincipalName</span></span> | <span data-ttu-id="8e19e-111">String</span><span class="sxs-lookup"><span data-stu-id="8e19e-111">String</span></span>            |
| <span data-ttu-id="8e19e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8e19e-112">displayName</span></span>       | <span data-ttu-id="8e19e-113">String</span><span class="sxs-lookup"><span data-stu-id="8e19e-113">String</span></span>            |
| <span data-ttu-id="8e19e-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8e19e-114">isDeleted</span></span>         | <span data-ttu-id="8e19e-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e19e-115">Boolean</span></span>           |
| <span data-ttu-id="8e19e-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="8e19e-116">deletedDate</span></span>       | <span data-ttu-id="8e19e-117">Data</span><span class="sxs-lookup"><span data-stu-id="8e19e-117">Date</span></span>              |
| <span data-ttu-id="8e19e-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8e19e-118">lastActivityDate</span></span>  | <span data-ttu-id="8e19e-119">Data</span><span class="sxs-lookup"><span data-stu-id="8e19e-119">Date</span></span>              |
| <span data-ttu-id="8e19e-120">sendCount</span><span class="sxs-lookup"><span data-stu-id="8e19e-120">sendCount</span></span>         | <span data-ttu-id="8e19e-121">Int64</span><span class="sxs-lookup"><span data-stu-id="8e19e-121">Int64</span></span>             |
| <span data-ttu-id="8e19e-122">receiveCount</span><span class="sxs-lookup"><span data-stu-id="8e19e-122">receiveCount</span></span>      | <span data-ttu-id="8e19e-123">Int64</span><span class="sxs-lookup"><span data-stu-id="8e19e-123">Int64</span></span>             |
| <span data-ttu-id="8e19e-124">readCount</span><span class="sxs-lookup"><span data-stu-id="8e19e-124">readCount</span></span>         | <span data-ttu-id="8e19e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="8e19e-125">Int64</span></span>             |
| <span data-ttu-id="8e19e-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="8e19e-126">assignedProducts</span></span>  | <span data-ttu-id="8e19e-127">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e19e-127">String collection</span></span> |
| <span data-ttu-id="8e19e-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8e19e-128">reportPeriod</span></span>      | <span data-ttu-id="8e19e-129">String</span><span class="sxs-lookup"><span data-stu-id="8e19e-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="8e19e-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e19e-130">JSON representation</span></span>

<span data-ttu-id="8e19e-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e19e-131">The following is a JSON representation of the resource.</span></span>

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


