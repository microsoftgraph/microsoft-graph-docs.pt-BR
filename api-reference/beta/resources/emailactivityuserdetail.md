---
title: tipo de recurso de emailActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 4f74b4af41c44e41b07bae1a8421011bc5188efc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033135"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="a6be8-103">tipo de recurso de emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="a6be8-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a6be8-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6be8-104">Properties</span></span>

| <span data-ttu-id="a6be8-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6be8-105">Property</span></span>          | <span data-ttu-id="a6be8-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6be8-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="a6be8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a6be8-107">reportRefreshDate</span></span> | <span data-ttu-id="a6be8-108">Data</span><span class="sxs-lookup"><span data-stu-id="a6be8-108">Date</span></span>              |
| <span data-ttu-id="a6be8-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a6be8-109">userPrincipalName</span></span> | <span data-ttu-id="a6be8-110">String</span><span class="sxs-lookup"><span data-stu-id="a6be8-110">String</span></span>            |
| <span data-ttu-id="a6be8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a6be8-111">displayName</span></span>       | <span data-ttu-id="a6be8-112">String</span><span class="sxs-lookup"><span data-stu-id="a6be8-112">String</span></span>            |
| <span data-ttu-id="a6be8-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a6be8-113">isDeleted</span></span>         | <span data-ttu-id="a6be8-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6be8-114">Boolean</span></span>           |
| <span data-ttu-id="a6be8-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="a6be8-115">deletedDate</span></span>       | <span data-ttu-id="a6be8-116">Data</span><span class="sxs-lookup"><span data-stu-id="a6be8-116">Date</span></span>              |
| <span data-ttu-id="a6be8-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a6be8-117">lastActivityDate</span></span>  | <span data-ttu-id="a6be8-118">Data</span><span class="sxs-lookup"><span data-stu-id="a6be8-118">Date</span></span>              |
| <span data-ttu-id="a6be8-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="a6be8-119">sendCount</span></span>         | <span data-ttu-id="a6be8-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a6be8-120">Int64</span></span>             |
| <span data-ttu-id="a6be8-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="a6be8-121">receiveCount</span></span>      | <span data-ttu-id="a6be8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a6be8-122">Int64</span></span>             |
| <span data-ttu-id="a6be8-123">readCount</span><span class="sxs-lookup"><span data-stu-id="a6be8-123">readCount</span></span>         | <span data-ttu-id="a6be8-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a6be8-124">Int64</span></span>             |
| <span data-ttu-id="a6be8-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="a6be8-125">assignedProducts</span></span>  | <span data-ttu-id="a6be8-126">String collection</span><span class="sxs-lookup"><span data-stu-id="a6be8-126">String collection</span></span> |
| <span data-ttu-id="a6be8-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a6be8-127">reportPeriod</span></span>      | <span data-ttu-id="a6be8-128">String</span><span class="sxs-lookup"><span data-stu-id="a6be8-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="a6be8-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6be8-129">JSON representation</span></span>

<span data-ttu-id="a6be8-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6be8-130">The following is a JSON representation of the resource.</span></span>

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
