---
title: Tipo de recurso emailActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 73e743bc6409f762a7898ec8037633c7bc3f00e4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981848"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="1e4ff-103">Tipo de recurso emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="1e4ff-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="1e4ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e4ff-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="1e4ff-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e4ff-105">Properties</span></span>

| <span data-ttu-id="1e4ff-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e4ff-106">Property</span></span>          | <span data-ttu-id="1e4ff-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e4ff-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="1e4ff-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1e4ff-108">reportRefreshDate</span></span> | <span data-ttu-id="1e4ff-109">Data</span><span class="sxs-lookup"><span data-stu-id="1e4ff-109">Date</span></span>              |
| <span data-ttu-id="1e4ff-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1e4ff-110">userPrincipalName</span></span> | <span data-ttu-id="1e4ff-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e4ff-111">String</span></span>            |
| <span data-ttu-id="1e4ff-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1e4ff-112">displayName</span></span>       | <span data-ttu-id="1e4ff-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e4ff-113">String</span></span>            |
| <span data-ttu-id="1e4ff-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1e4ff-114">isDeleted</span></span>         | <span data-ttu-id="1e4ff-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e4ff-115">Boolean</span></span>           |
| <span data-ttu-id="1e4ff-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="1e4ff-116">deletedDate</span></span>       | <span data-ttu-id="1e4ff-117">Data</span><span class="sxs-lookup"><span data-stu-id="1e4ff-117">Date</span></span>              |
| <span data-ttu-id="1e4ff-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="1e4ff-118">lastActivityDate</span></span>  | <span data-ttu-id="1e4ff-119">Data</span><span class="sxs-lookup"><span data-stu-id="1e4ff-119">Date</span></span>              |
| <span data-ttu-id="1e4ff-120">sendCount</span><span class="sxs-lookup"><span data-stu-id="1e4ff-120">sendCount</span></span>         | <span data-ttu-id="1e4ff-121">Int64</span><span class="sxs-lookup"><span data-stu-id="1e4ff-121">Int64</span></span>             |
| <span data-ttu-id="1e4ff-122">receiveCount</span><span class="sxs-lookup"><span data-stu-id="1e4ff-122">receiveCount</span></span>      | <span data-ttu-id="1e4ff-123">Int64</span><span class="sxs-lookup"><span data-stu-id="1e4ff-123">Int64</span></span>             |
| <span data-ttu-id="1e4ff-124">readCount</span><span class="sxs-lookup"><span data-stu-id="1e4ff-124">readCount</span></span>         | <span data-ttu-id="1e4ff-125">Int64</span><span class="sxs-lookup"><span data-stu-id="1e4ff-125">Int64</span></span>             |
| <span data-ttu-id="1e4ff-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="1e4ff-126">assignedProducts</span></span>  | <span data-ttu-id="1e4ff-127">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1e4ff-127">String collection</span></span> |
| <span data-ttu-id="1e4ff-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1e4ff-128">reportPeriod</span></span>      | <span data-ttu-id="1e4ff-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e4ff-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="1e4ff-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e4ff-130">JSON representation</span></span>

<span data-ttu-id="1e4ff-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e4ff-131">The following is a JSON representation of the resource.</span></span>

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


