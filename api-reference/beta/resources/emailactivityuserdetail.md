---
title: tipo de recurso de emailActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 16512c3a8a4dab62d4a71406d6c33d52a5a9bc08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817995"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="85516-103">tipo de recurso de emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="85516-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="85516-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85516-104">Properties</span></span>

| <span data-ttu-id="85516-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85516-105">Property</span></span>          | <span data-ttu-id="85516-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="85516-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="85516-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="85516-107">reportRefreshDate</span></span> | <span data-ttu-id="85516-108">Data</span><span class="sxs-lookup"><span data-stu-id="85516-108">Date</span></span>              |
| <span data-ttu-id="85516-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="85516-109">userPrincipalName</span></span> | <span data-ttu-id="85516-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85516-110">String</span></span>            |
| <span data-ttu-id="85516-111">displayName</span><span class="sxs-lookup"><span data-stu-id="85516-111">displayName</span></span>       | <span data-ttu-id="85516-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85516-112">String</span></span>            |
| <span data-ttu-id="85516-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="85516-113">isDeleted</span></span>         | <span data-ttu-id="85516-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="85516-114">Boolean</span></span>           |
| <span data-ttu-id="85516-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="85516-115">deletedDate</span></span>       | <span data-ttu-id="85516-116">Data</span><span class="sxs-lookup"><span data-stu-id="85516-116">Date</span></span>              |
| <span data-ttu-id="85516-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="85516-117">lastActivityDate</span></span>  | <span data-ttu-id="85516-118">Data</span><span class="sxs-lookup"><span data-stu-id="85516-118">Date</span></span>              |
| <span data-ttu-id="85516-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="85516-119">sendCount</span></span>         | <span data-ttu-id="85516-120">Int64</span><span class="sxs-lookup"><span data-stu-id="85516-120">Int64</span></span>             |
| <span data-ttu-id="85516-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="85516-121">receiveCount</span></span>      | <span data-ttu-id="85516-122">Int64</span><span class="sxs-lookup"><span data-stu-id="85516-122">Int64</span></span>             |
| <span data-ttu-id="85516-123">readCount</span><span class="sxs-lookup"><span data-stu-id="85516-123">readCount</span></span>         | <span data-ttu-id="85516-124">Int64</span><span class="sxs-lookup"><span data-stu-id="85516-124">Int64</span></span>             |
| <span data-ttu-id="85516-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="85516-125">assignedProducts</span></span>  | <span data-ttu-id="85516-126">String collection</span><span class="sxs-lookup"><span data-stu-id="85516-126">String collection</span></span> |
| <span data-ttu-id="85516-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="85516-127">reportPeriod</span></span>      | <span data-ttu-id="85516-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85516-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="85516-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85516-129">JSON representation</span></span>

<span data-ttu-id="85516-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85516-130">The following is a JSON representation of the resource.</span></span>

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
