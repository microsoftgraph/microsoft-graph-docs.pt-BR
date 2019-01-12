---
title: tipo de recurso de emailActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b871bf5dbaedd961fad09bf97be868f46e7430a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938304"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="5f8c1-103">tipo de recurso de emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="5f8c1-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5f8c1-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f8c1-104">Properties</span></span>

| <span data-ttu-id="5f8c1-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f8c1-105">Property</span></span>          | <span data-ttu-id="5f8c1-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f8c1-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="5f8c1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5f8c1-107">reportRefreshDate</span></span> | <span data-ttu-id="5f8c1-108">Data</span><span class="sxs-lookup"><span data-stu-id="5f8c1-108">Date</span></span>              |
| <span data-ttu-id="5f8c1-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5f8c1-109">userPrincipalName</span></span> | <span data-ttu-id="5f8c1-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f8c1-110">String</span></span>            |
| <span data-ttu-id="5f8c1-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5f8c1-111">displayName</span></span>       | <span data-ttu-id="5f8c1-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f8c1-112">String</span></span>            |
| <span data-ttu-id="5f8c1-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5f8c1-113">isDeleted</span></span>         | <span data-ttu-id="5f8c1-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="5f8c1-114">Boolean</span></span>           |
| <span data-ttu-id="5f8c1-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="5f8c1-115">deletedDate</span></span>       | <span data-ttu-id="5f8c1-116">Data</span><span class="sxs-lookup"><span data-stu-id="5f8c1-116">Date</span></span>              |
| <span data-ttu-id="5f8c1-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="5f8c1-117">lastActivityDate</span></span>  | <span data-ttu-id="5f8c1-118">Data</span><span class="sxs-lookup"><span data-stu-id="5f8c1-118">Date</span></span>              |
| <span data-ttu-id="5f8c1-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="5f8c1-119">sendCount</span></span>         | <span data-ttu-id="5f8c1-120">Int64</span><span class="sxs-lookup"><span data-stu-id="5f8c1-120">Int64</span></span>             |
| <span data-ttu-id="5f8c1-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="5f8c1-121">receiveCount</span></span>      | <span data-ttu-id="5f8c1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="5f8c1-122">Int64</span></span>             |
| <span data-ttu-id="5f8c1-123">readCount</span><span class="sxs-lookup"><span data-stu-id="5f8c1-123">readCount</span></span>         | <span data-ttu-id="5f8c1-124">Int64</span><span class="sxs-lookup"><span data-stu-id="5f8c1-124">Int64</span></span>             |
| <span data-ttu-id="5f8c1-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="5f8c1-125">assignedProducts</span></span>  | <span data-ttu-id="5f8c1-126">String collection</span><span class="sxs-lookup"><span data-stu-id="5f8c1-126">String collection</span></span> |
| <span data-ttu-id="5f8c1-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5f8c1-127">reportPeriod</span></span>      | <span data-ttu-id="5f8c1-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f8c1-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="5f8c1-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f8c1-129">JSON representation</span></span>

<span data-ttu-id="5f8c1-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f8c1-130">The following is a JSON representation of the resource.</span></span>

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
