---
title: tipo de recurso de teamsUserActivityUserDetail
description: A seguir está uma representaion JSON do recurso.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 2e3f64c7065343712f6a9d9c6a114bf95f24c171
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823650"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="f8859-103">tipo de recurso de teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="f8859-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f8859-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8859-104">Properties</span></span>

| <span data-ttu-id="f8859-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8859-105">Property</span></span>                | <span data-ttu-id="f8859-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8859-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="f8859-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f8859-107">reportRefreshDate</span></span>       | <span data-ttu-id="f8859-108">Data</span><span class="sxs-lookup"><span data-stu-id="f8859-108">Date</span></span>              |
| <span data-ttu-id="f8859-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8859-109">userPrincipalName</span></span>       | <span data-ttu-id="f8859-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8859-110">String</span></span>            |
| <span data-ttu-id="f8859-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f8859-111">lastActivityDate</span></span>        | <span data-ttu-id="f8859-112">Data</span><span class="sxs-lookup"><span data-stu-id="f8859-112">Date</span></span>              |
| <span data-ttu-id="f8859-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f8859-113">isDeleted</span></span>               | <span data-ttu-id="f8859-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="f8859-114">Boolean</span></span>           |
| <span data-ttu-id="f8859-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="f8859-115">deletedDate</span></span>             | <span data-ttu-id="f8859-116">Data</span><span class="sxs-lookup"><span data-stu-id="f8859-116">Date</span></span>              |
| <span data-ttu-id="f8859-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="f8859-117">assignedProducts</span></span>        | <span data-ttu-id="f8859-118">String collection</span><span class="sxs-lookup"><span data-stu-id="f8859-118">String collection</span></span> |
| <span data-ttu-id="f8859-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="f8859-119">teamChatMessageCount</span></span>    | <span data-ttu-id="f8859-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f8859-120">Int64</span></span>             |
| <span data-ttu-id="f8859-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="f8859-121">privateChatMessageCount</span></span> | <span data-ttu-id="f8859-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f8859-122">Int64</span></span>             |
| <span data-ttu-id="f8859-123">callCount</span><span class="sxs-lookup"><span data-stu-id="f8859-123">callCount</span></span>               | <span data-ttu-id="f8859-124">Int64</span><span class="sxs-lookup"><span data-stu-id="f8859-124">Int64</span></span>             |
| <span data-ttu-id="f8859-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="f8859-125">meetingCount</span></span>            | <span data-ttu-id="f8859-126">Int64</span><span class="sxs-lookup"><span data-stu-id="f8859-126">Int64</span></span>             |
| <span data-ttu-id="f8859-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="f8859-127">hasOtherAction</span></span>          | <span data-ttu-id="f8859-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="f8859-128">Boolean</span></span>           |
| <span data-ttu-id="f8859-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f8859-129">reportPeriod</span></span>            | <span data-ttu-id="f8859-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8859-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="f8859-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8859-131">JSON representation</span></span>

<span data-ttu-id="f8859-132">A seguir está uma representaion JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8859-132">The following is a JSON representaion of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```
