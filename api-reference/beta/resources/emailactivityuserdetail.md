---
title: tipo de recurso emailActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c664cb4a381cf2ebe3de9bd9ca53719786b94405
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499565"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="84753-103">tipo de recurso emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="84753-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="84753-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="84753-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="84753-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84753-105">Properties</span></span>

| <span data-ttu-id="84753-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84753-106">Property</span></span>          | <span data-ttu-id="84753-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="84753-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="84753-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="84753-108">reportRefreshDate</span></span> | <span data-ttu-id="84753-109">Data</span><span class="sxs-lookup"><span data-stu-id="84753-109">Date</span></span>              |
| <span data-ttu-id="84753-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="84753-110">userPrincipalName</span></span> | <span data-ttu-id="84753-111">String</span><span class="sxs-lookup"><span data-stu-id="84753-111">String</span></span>            |
| <span data-ttu-id="84753-112">displayName</span><span class="sxs-lookup"><span data-stu-id="84753-112">displayName</span></span>       | <span data-ttu-id="84753-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84753-113">String</span></span>            |
| <span data-ttu-id="84753-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="84753-114">isDeleted</span></span>         | <span data-ttu-id="84753-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="84753-115">Boolean</span></span>           |
| <span data-ttu-id="84753-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="84753-116">deletedDate</span></span>       | <span data-ttu-id="84753-117">Data</span><span class="sxs-lookup"><span data-stu-id="84753-117">Date</span></span>              |
| <span data-ttu-id="84753-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="84753-118">lastActivityDate</span></span>  | <span data-ttu-id="84753-119">Data</span><span class="sxs-lookup"><span data-stu-id="84753-119">Date</span></span>              |
| <span data-ttu-id="84753-120">sendCount</span><span class="sxs-lookup"><span data-stu-id="84753-120">sendCount</span></span>         | <span data-ttu-id="84753-121">Int64</span><span class="sxs-lookup"><span data-stu-id="84753-121">Int64</span></span>             |
| <span data-ttu-id="84753-122">receiveCount</span><span class="sxs-lookup"><span data-stu-id="84753-122">receiveCount</span></span>      | <span data-ttu-id="84753-123">Int64</span><span class="sxs-lookup"><span data-stu-id="84753-123">Int64</span></span>             |
| <span data-ttu-id="84753-124">readCount</span><span class="sxs-lookup"><span data-stu-id="84753-124">readCount</span></span>         | <span data-ttu-id="84753-125">Int64</span><span class="sxs-lookup"><span data-stu-id="84753-125">Int64</span></span>             |
| <span data-ttu-id="84753-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="84753-126">assignedProducts</span></span>  | <span data-ttu-id="84753-127">String collection</span><span class="sxs-lookup"><span data-stu-id="84753-127">String collection</span></span> |
| <span data-ttu-id="84753-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="84753-128">reportPeriod</span></span>      | <span data-ttu-id="84753-129">String</span><span class="sxs-lookup"><span data-stu-id="84753-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="84753-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84753-130">JSON representation</span></span>

<span data-ttu-id="84753-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84753-131">The following is a JSON representation of the resource.</span></span>

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
