---
title: tipo de recurso teamsUserActivityUserDetail
description: Veja a seguir uma representaion JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cbe6297388907f28f8841e0a1dcb2ec3ae788844
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964351"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="24c38-103">tipo de recurso teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="24c38-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="24c38-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24c38-104">Properties</span></span>

| <span data-ttu-id="24c38-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24c38-105">Property</span></span>                | <span data-ttu-id="24c38-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="24c38-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="24c38-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="24c38-107">reportRefreshDate</span></span>       | <span data-ttu-id="24c38-108">Data</span><span class="sxs-lookup"><span data-stu-id="24c38-108">Date</span></span>              |
| <span data-ttu-id="24c38-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="24c38-109">userPrincipalName</span></span>       | <span data-ttu-id="24c38-110">String</span><span class="sxs-lookup"><span data-stu-id="24c38-110">String</span></span>            |
| <span data-ttu-id="24c38-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="24c38-111">lastActivityDate</span></span>        | <span data-ttu-id="24c38-112">Data</span><span class="sxs-lookup"><span data-stu-id="24c38-112">Date</span></span>              |
| <span data-ttu-id="24c38-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="24c38-113">isDeleted</span></span>               | <span data-ttu-id="24c38-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="24c38-114">Boolean</span></span>           |
| <span data-ttu-id="24c38-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="24c38-115">deletedDate</span></span>             | <span data-ttu-id="24c38-116">Data</span><span class="sxs-lookup"><span data-stu-id="24c38-116">Date</span></span>              |
| <span data-ttu-id="24c38-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="24c38-117">assignedProducts</span></span>        | <span data-ttu-id="24c38-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="24c38-118">String collection</span></span> |
| <span data-ttu-id="24c38-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="24c38-119">teamChatMessageCount</span></span>    | <span data-ttu-id="24c38-120">Int64</span><span class="sxs-lookup"><span data-stu-id="24c38-120">Int64</span></span>             |
| <span data-ttu-id="24c38-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="24c38-121">privateChatMessageCount</span></span> | <span data-ttu-id="24c38-122">Int64</span><span class="sxs-lookup"><span data-stu-id="24c38-122">Int64</span></span>             |
| <span data-ttu-id="24c38-123">callCount</span><span class="sxs-lookup"><span data-stu-id="24c38-123">callCount</span></span>               | <span data-ttu-id="24c38-124">Int64</span><span class="sxs-lookup"><span data-stu-id="24c38-124">Int64</span></span>             |
| <span data-ttu-id="24c38-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="24c38-125">meetingCount</span></span>            | <span data-ttu-id="24c38-126">Int64</span><span class="sxs-lookup"><span data-stu-id="24c38-126">Int64</span></span>             |
| <span data-ttu-id="24c38-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="24c38-127">hasOtherAction</span></span>          | <span data-ttu-id="24c38-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="24c38-128">Boolean</span></span>           |
| <span data-ttu-id="24c38-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="24c38-129">reportPeriod</span></span>            | <span data-ttu-id="24c38-130">String</span><span class="sxs-lookup"><span data-stu-id="24c38-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="24c38-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24c38-131">JSON representation</span></span>

<span data-ttu-id="24c38-132">Veja a seguir uma representaion JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="24c38-132">The following is a JSON representaion of the resource.</span></span>

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
