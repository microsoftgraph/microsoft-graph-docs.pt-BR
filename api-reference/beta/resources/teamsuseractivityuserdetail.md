---
title: tipo de recurso de teamsUserActivityUserDetail
description: A seguir está uma representaion JSON do recurso.
ms.openlocfilehash: 4e40ea4adf07450e6b51555df47579955a2a0286
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039809"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="09d57-103">tipo de recurso de teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="09d57-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="09d57-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09d57-104">Properties</span></span>

| <span data-ttu-id="09d57-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09d57-105">Property</span></span>                | <span data-ttu-id="09d57-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="09d57-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="09d57-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="09d57-107">reportRefreshDate</span></span>       | <span data-ttu-id="09d57-108">Data</span><span class="sxs-lookup"><span data-stu-id="09d57-108">Date</span></span>              |
| <span data-ttu-id="09d57-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="09d57-109">userPrincipalName</span></span>       | <span data-ttu-id="09d57-110">String</span><span class="sxs-lookup"><span data-stu-id="09d57-110">String</span></span>            |
| <span data-ttu-id="09d57-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="09d57-111">lastActivityDate</span></span>        | <span data-ttu-id="09d57-112">Data</span><span class="sxs-lookup"><span data-stu-id="09d57-112">Date</span></span>              |
| <span data-ttu-id="09d57-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="09d57-113">isDeleted</span></span>               | <span data-ttu-id="09d57-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="09d57-114">Boolean</span></span>           |
| <span data-ttu-id="09d57-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="09d57-115">deletedDate</span></span>             | <span data-ttu-id="09d57-116">Data</span><span class="sxs-lookup"><span data-stu-id="09d57-116">Date</span></span>              |
| <span data-ttu-id="09d57-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="09d57-117">assignedProducts</span></span>        | <span data-ttu-id="09d57-118">String collection</span><span class="sxs-lookup"><span data-stu-id="09d57-118">String collection</span></span> |
| <span data-ttu-id="09d57-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="09d57-119">teamChatMessageCount</span></span>    | <span data-ttu-id="09d57-120">Int64</span><span class="sxs-lookup"><span data-stu-id="09d57-120">Int64</span></span>             |
| <span data-ttu-id="09d57-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="09d57-121">privateChatMessageCount</span></span> | <span data-ttu-id="09d57-122">Int64</span><span class="sxs-lookup"><span data-stu-id="09d57-122">Int64</span></span>             |
| <span data-ttu-id="09d57-123">callCount</span><span class="sxs-lookup"><span data-stu-id="09d57-123">callCount</span></span>               | <span data-ttu-id="09d57-124">Int64</span><span class="sxs-lookup"><span data-stu-id="09d57-124">Int64</span></span>             |
| <span data-ttu-id="09d57-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="09d57-125">meetingCount</span></span>            | <span data-ttu-id="09d57-126">Int64</span><span class="sxs-lookup"><span data-stu-id="09d57-126">Int64</span></span>             |
| <span data-ttu-id="09d57-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="09d57-127">hasOtherAction</span></span>          | <span data-ttu-id="09d57-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="09d57-128">Boolean</span></span>           |
| <span data-ttu-id="09d57-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="09d57-129">reportPeriod</span></span>            | <span data-ttu-id="09d57-130">String</span><span class="sxs-lookup"><span data-stu-id="09d57-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="09d57-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09d57-131">JSON representation</span></span>

<span data-ttu-id="09d57-132">A seguir está uma representaion JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09d57-132">The following is a JSON representaion of the resource.</span></span>

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
