---
title: tipo de recurso de teamsUserActivityUserDetail
description: A seguir está uma representaion JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913426"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="99e0c-103">tipo de recurso de teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="99e0c-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="99e0c-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99e0c-104">Properties</span></span>

| <span data-ttu-id="99e0c-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99e0c-105">Property</span></span>                | <span data-ttu-id="99e0c-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="99e0c-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="99e0c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="99e0c-107">reportRefreshDate</span></span>       | <span data-ttu-id="99e0c-108">Data</span><span class="sxs-lookup"><span data-stu-id="99e0c-108">Date</span></span>              |
| <span data-ttu-id="99e0c-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="99e0c-109">userPrincipalName</span></span>       | <span data-ttu-id="99e0c-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99e0c-110">String</span></span>            |
| <span data-ttu-id="99e0c-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="99e0c-111">lastActivityDate</span></span>        | <span data-ttu-id="99e0c-112">Data</span><span class="sxs-lookup"><span data-stu-id="99e0c-112">Date</span></span>              |
| <span data-ttu-id="99e0c-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="99e0c-113">isDeleted</span></span>               | <span data-ttu-id="99e0c-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="99e0c-114">Boolean</span></span>           |
| <span data-ttu-id="99e0c-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="99e0c-115">deletedDate</span></span>             | <span data-ttu-id="99e0c-116">Data</span><span class="sxs-lookup"><span data-stu-id="99e0c-116">Date</span></span>              |
| <span data-ttu-id="99e0c-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="99e0c-117">assignedProducts</span></span>        | <span data-ttu-id="99e0c-118">String collection</span><span class="sxs-lookup"><span data-stu-id="99e0c-118">String collection</span></span> |
| <span data-ttu-id="99e0c-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="99e0c-119">teamChatMessageCount</span></span>    | <span data-ttu-id="99e0c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="99e0c-120">Int64</span></span>             |
| <span data-ttu-id="99e0c-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="99e0c-121">privateChatMessageCount</span></span> | <span data-ttu-id="99e0c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="99e0c-122">Int64</span></span>             |
| <span data-ttu-id="99e0c-123">callCount</span><span class="sxs-lookup"><span data-stu-id="99e0c-123">callCount</span></span>               | <span data-ttu-id="99e0c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="99e0c-124">Int64</span></span>             |
| <span data-ttu-id="99e0c-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="99e0c-125">meetingCount</span></span>            | <span data-ttu-id="99e0c-126">Int64</span><span class="sxs-lookup"><span data-stu-id="99e0c-126">Int64</span></span>             |
| <span data-ttu-id="99e0c-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="99e0c-127">hasOtherAction</span></span>          | <span data-ttu-id="99e0c-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="99e0c-128">Boolean</span></span>           |
| <span data-ttu-id="99e0c-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="99e0c-129">reportPeriod</span></span>            | <span data-ttu-id="99e0c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99e0c-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="99e0c-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99e0c-131">JSON representation</span></span>

<span data-ttu-id="99e0c-132">A seguir está uma representaion JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99e0c-132">The following is a JSON representaion of the resource.</span></span>

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
