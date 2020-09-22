---
title: tipo de recurso teamsUserActivityUserDetail
description: Veja a seguir uma representaion JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 73208044be5d3612303774f92dfced2302939de8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046353"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="413e2-103">tipo de recurso teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="413e2-103">teamsUserActivityUserDetail resource type</span></span>

<span data-ttu-id="413e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="413e2-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="413e2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="413e2-105">Properties</span></span>

| <span data-ttu-id="413e2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="413e2-106">Property</span></span>                | <span data-ttu-id="413e2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="413e2-107">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="413e2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="413e2-108">reportRefreshDate</span></span>       | <span data-ttu-id="413e2-109">Data</span><span class="sxs-lookup"><span data-stu-id="413e2-109">Date</span></span>              |
| <span data-ttu-id="413e2-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="413e2-110">userPrincipalName</span></span>       | <span data-ttu-id="413e2-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="413e2-111">String</span></span>            |
| <span data-ttu-id="413e2-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="413e2-112">lastActivityDate</span></span>        | <span data-ttu-id="413e2-113">Data</span><span class="sxs-lookup"><span data-stu-id="413e2-113">Date</span></span>              |
| <span data-ttu-id="413e2-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="413e2-114">isDeleted</span></span>               | <span data-ttu-id="413e2-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="413e2-115">Boolean</span></span>           |
| <span data-ttu-id="413e2-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="413e2-116">deletedDate</span></span>             | <span data-ttu-id="413e2-117">Data</span><span class="sxs-lookup"><span data-stu-id="413e2-117">Date</span></span>              |
| <span data-ttu-id="413e2-118">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="413e2-118">assignedProducts</span></span>        | <span data-ttu-id="413e2-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="413e2-119">String collection</span></span> |
| <span data-ttu-id="413e2-120">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="413e2-120">teamChatMessageCount</span></span>    | <span data-ttu-id="413e2-121">Int64</span><span class="sxs-lookup"><span data-stu-id="413e2-121">Int64</span></span>             |
| <span data-ttu-id="413e2-122">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="413e2-122">privateChatMessageCount</span></span> | <span data-ttu-id="413e2-123">Int64</span><span class="sxs-lookup"><span data-stu-id="413e2-123">Int64</span></span>             |
| <span data-ttu-id="413e2-124">callCount</span><span class="sxs-lookup"><span data-stu-id="413e2-124">callCount</span></span>               | <span data-ttu-id="413e2-125">Int64</span><span class="sxs-lookup"><span data-stu-id="413e2-125">Int64</span></span>             |
| <span data-ttu-id="413e2-126">meetingCount</span><span class="sxs-lookup"><span data-stu-id="413e2-126">meetingCount</span></span>            | <span data-ttu-id="413e2-127">Int64</span><span class="sxs-lookup"><span data-stu-id="413e2-127">Int64</span></span>             |
| <span data-ttu-id="413e2-128">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="413e2-128">hasOtherAction</span></span>          | <span data-ttu-id="413e2-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="413e2-129">Boolean</span></span>           |
| <span data-ttu-id="413e2-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="413e2-130">reportPeriod</span></span>            | <span data-ttu-id="413e2-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="413e2-131">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="413e2-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="413e2-132">JSON representation</span></span>

<span data-ttu-id="413e2-133">Veja a seguir uma representaion JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="413e2-133">The following is a JSON representaion of the resource.</span></span>

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


