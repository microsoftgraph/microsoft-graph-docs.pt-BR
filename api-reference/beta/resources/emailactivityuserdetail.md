---
title: tipo de recurso emailActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: cd78b80d97a6dfcaa4c7b97085e89daa4f8a8523
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972198"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="94f4f-103">tipo de recurso emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="94f4f-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="94f4f-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94f4f-104">Properties</span></span>

| <span data-ttu-id="94f4f-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94f4f-105">Property</span></span>          | <span data-ttu-id="94f4f-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="94f4f-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="94f4f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="94f4f-107">reportRefreshDate</span></span> | <span data-ttu-id="94f4f-108">Data</span><span class="sxs-lookup"><span data-stu-id="94f4f-108">Date</span></span>              |
| <span data-ttu-id="94f4f-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="94f4f-109">userPrincipalName</span></span> | <span data-ttu-id="94f4f-110">String</span><span class="sxs-lookup"><span data-stu-id="94f4f-110">String</span></span>            |
| <span data-ttu-id="94f4f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="94f4f-111">displayName</span></span>       | <span data-ttu-id="94f4f-112">String</span><span class="sxs-lookup"><span data-stu-id="94f4f-112">String</span></span>            |
| <span data-ttu-id="94f4f-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="94f4f-113">isDeleted</span></span>         | <span data-ttu-id="94f4f-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="94f4f-114">Boolean</span></span>           |
| <span data-ttu-id="94f4f-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="94f4f-115">deletedDate</span></span>       | <span data-ttu-id="94f4f-116">Data</span><span class="sxs-lookup"><span data-stu-id="94f4f-116">Date</span></span>              |
| <span data-ttu-id="94f4f-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="94f4f-117">lastActivityDate</span></span>  | <span data-ttu-id="94f4f-118">Data</span><span class="sxs-lookup"><span data-stu-id="94f4f-118">Date</span></span>              |
| <span data-ttu-id="94f4f-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="94f4f-119">sendCount</span></span>         | <span data-ttu-id="94f4f-120">Int64</span><span class="sxs-lookup"><span data-stu-id="94f4f-120">Int64</span></span>             |
| <span data-ttu-id="94f4f-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="94f4f-121">receiveCount</span></span>      | <span data-ttu-id="94f4f-122">Int64</span><span class="sxs-lookup"><span data-stu-id="94f4f-122">Int64</span></span>             |
| <span data-ttu-id="94f4f-123">readCount</span><span class="sxs-lookup"><span data-stu-id="94f4f-123">readCount</span></span>         | <span data-ttu-id="94f4f-124">Int64</span><span class="sxs-lookup"><span data-stu-id="94f4f-124">Int64</span></span>             |
| <span data-ttu-id="94f4f-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="94f4f-125">assignedProducts</span></span>  | <span data-ttu-id="94f4f-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="94f4f-126">String collection</span></span> |
| <span data-ttu-id="94f4f-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="94f4f-127">reportPeriod</span></span>      | <span data-ttu-id="94f4f-128">String</span><span class="sxs-lookup"><span data-stu-id="94f4f-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="94f4f-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94f4f-129">JSON representation</span></span>

<span data-ttu-id="94f4f-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94f4f-130">The following is a JSON representation of the resource.</span></span>

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
