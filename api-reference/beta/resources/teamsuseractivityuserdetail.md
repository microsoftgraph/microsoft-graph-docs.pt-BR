---
title: tipo de recurso teamsUserActivityUserDetail
description: Veja a seguir uma representaion JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582903"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="83aee-103">tipo de recurso teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="83aee-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="83aee-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83aee-104">Properties</span></span>

| <span data-ttu-id="83aee-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83aee-105">Property</span></span>                | <span data-ttu-id="83aee-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="83aee-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="83aee-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="83aee-107">reportRefreshDate</span></span>       | <span data-ttu-id="83aee-108">Data</span><span class="sxs-lookup"><span data-stu-id="83aee-108">Date</span></span>              |
| <span data-ttu-id="83aee-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="83aee-109">userPrincipalName</span></span>       | <span data-ttu-id="83aee-110">String</span><span class="sxs-lookup"><span data-stu-id="83aee-110">String</span></span>            |
| <span data-ttu-id="83aee-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="83aee-111">lastActivityDate</span></span>        | <span data-ttu-id="83aee-112">Data</span><span class="sxs-lookup"><span data-stu-id="83aee-112">Date</span></span>              |
| <span data-ttu-id="83aee-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="83aee-113">isDeleted</span></span>               | <span data-ttu-id="83aee-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="83aee-114">Boolean</span></span>           |
| <span data-ttu-id="83aee-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="83aee-115">deletedDate</span></span>             | <span data-ttu-id="83aee-116">Data</span><span class="sxs-lookup"><span data-stu-id="83aee-116">Date</span></span>              |
| <span data-ttu-id="83aee-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="83aee-117">assignedProducts</span></span>        | <span data-ttu-id="83aee-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="83aee-118">String collection</span></span> |
| <span data-ttu-id="83aee-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="83aee-119">teamChatMessageCount</span></span>    | <span data-ttu-id="83aee-120">Int64</span><span class="sxs-lookup"><span data-stu-id="83aee-120">Int64</span></span>             |
| <span data-ttu-id="83aee-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="83aee-121">privateChatMessageCount</span></span> | <span data-ttu-id="83aee-122">Int64</span><span class="sxs-lookup"><span data-stu-id="83aee-122">Int64</span></span>             |
| <span data-ttu-id="83aee-123">callCount</span><span class="sxs-lookup"><span data-stu-id="83aee-123">callCount</span></span>               | <span data-ttu-id="83aee-124">Int64</span><span class="sxs-lookup"><span data-stu-id="83aee-124">Int64</span></span>             |
| <span data-ttu-id="83aee-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="83aee-125">meetingCount</span></span>            | <span data-ttu-id="83aee-126">Int64</span><span class="sxs-lookup"><span data-stu-id="83aee-126">Int64</span></span>             |
| <span data-ttu-id="83aee-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="83aee-127">hasOtherAction</span></span>          | <span data-ttu-id="83aee-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="83aee-128">Boolean</span></span>           |
| <span data-ttu-id="83aee-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="83aee-129">reportPeriod</span></span>            | <span data-ttu-id="83aee-130">String</span><span class="sxs-lookup"><span data-stu-id="83aee-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="83aee-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83aee-131">JSON representation</span></span>

<span data-ttu-id="83aee-132">Veja a seguir uma representaion JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83aee-132">The following is a JSON representaion of the resource.</span></span>

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
