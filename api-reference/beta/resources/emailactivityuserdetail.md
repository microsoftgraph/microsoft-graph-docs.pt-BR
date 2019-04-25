---
title: tipo de recurso emailActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b871bf5dbaedd961fad09bf97be868f46e7430a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542829"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="f9410-103">tipo de recurso emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="f9410-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f9410-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9410-104">Properties</span></span>

| <span data-ttu-id="f9410-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9410-105">Property</span></span>          | <span data-ttu-id="f9410-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9410-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="f9410-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f9410-107">reportRefreshDate</span></span> | <span data-ttu-id="f9410-108">Data</span><span class="sxs-lookup"><span data-stu-id="f9410-108">Date</span></span>              |
| <span data-ttu-id="f9410-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f9410-109">userPrincipalName</span></span> | <span data-ttu-id="f9410-110">String</span><span class="sxs-lookup"><span data-stu-id="f9410-110">String</span></span>            |
| <span data-ttu-id="f9410-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f9410-111">displayName</span></span>       | <span data-ttu-id="f9410-112">String</span><span class="sxs-lookup"><span data-stu-id="f9410-112">String</span></span>            |
| <span data-ttu-id="f9410-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f9410-113">isDeleted</span></span>         | <span data-ttu-id="f9410-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9410-114">Boolean</span></span>           |
| <span data-ttu-id="f9410-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="f9410-115">deletedDate</span></span>       | <span data-ttu-id="f9410-116">Data</span><span class="sxs-lookup"><span data-stu-id="f9410-116">Date</span></span>              |
| <span data-ttu-id="f9410-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f9410-117">lastActivityDate</span></span>  | <span data-ttu-id="f9410-118">Data</span><span class="sxs-lookup"><span data-stu-id="f9410-118">Date</span></span>              |
| <span data-ttu-id="f9410-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="f9410-119">sendCount</span></span>         | <span data-ttu-id="f9410-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f9410-120">Int64</span></span>             |
| <span data-ttu-id="f9410-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="f9410-121">receiveCount</span></span>      | <span data-ttu-id="f9410-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f9410-122">Int64</span></span>             |
| <span data-ttu-id="f9410-123">readCount</span><span class="sxs-lookup"><span data-stu-id="f9410-123">readCount</span></span>         | <span data-ttu-id="f9410-124">Int64</span><span class="sxs-lookup"><span data-stu-id="f9410-124">Int64</span></span>             |
| <span data-ttu-id="f9410-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="f9410-125">assignedProducts</span></span>  | <span data-ttu-id="f9410-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9410-126">String collection</span></span> |
| <span data-ttu-id="f9410-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f9410-127">reportPeriod</span></span>      | <span data-ttu-id="f9410-128">String</span><span class="sxs-lookup"><span data-stu-id="f9410-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="f9410-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9410-129">JSON representation</span></span>

<span data-ttu-id="f9410-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9410-130">The following is a JSON representation of the resource.</span></span>

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
