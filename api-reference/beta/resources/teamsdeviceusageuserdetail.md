---
title: tipo de recurso teamsDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c5c3815b2418f414aa552f211bbeed5f643eb0d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519859"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="47e06-103">tipo de recurso teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="47e06-103">teamsDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="47e06-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="47e06-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="47e06-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47e06-105">Properties</span></span>

| <span data-ttu-id="47e06-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47e06-106">Property</span></span>          | <span data-ttu-id="47e06-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="47e06-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="47e06-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="47e06-108">reportRefreshDate</span></span> | <span data-ttu-id="47e06-109">Data</span><span class="sxs-lookup"><span data-stu-id="47e06-109">Date</span></span>    |
| <span data-ttu-id="47e06-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="47e06-110">userPrincipalName</span></span> | <span data-ttu-id="47e06-111">String</span><span class="sxs-lookup"><span data-stu-id="47e06-111">String</span></span>  |
| <span data-ttu-id="47e06-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="47e06-112">lastActivityDate</span></span>  | <span data-ttu-id="47e06-113">Data</span><span class="sxs-lookup"><span data-stu-id="47e06-113">Date</span></span>    |
| <span data-ttu-id="47e06-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="47e06-114">isDeleted</span></span>         | <span data-ttu-id="47e06-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="47e06-115">Boolean</span></span> |
| <span data-ttu-id="47e06-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="47e06-116">deletedDate</span></span>       | <span data-ttu-id="47e06-117">Data</span><span class="sxs-lookup"><span data-stu-id="47e06-117">Date</span></span>    |
| <span data-ttu-id="47e06-118">usedWeb</span><span class="sxs-lookup"><span data-stu-id="47e06-118">usedWeb</span></span>           | <span data-ttu-id="47e06-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="47e06-119">Boolean</span></span> |
| <span data-ttu-id="47e06-120">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="47e06-120">usedWindowsPhone</span></span>  | <span data-ttu-id="47e06-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="47e06-121">Boolean</span></span> |
| <span data-ttu-id="47e06-122">usediOS</span><span class="sxs-lookup"><span data-stu-id="47e06-122">usediOS</span></span>           | <span data-ttu-id="47e06-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="47e06-123">Boolean</span></span> |
| <span data-ttu-id="47e06-124">usedMac</span><span class="sxs-lookup"><span data-stu-id="47e06-124">usedMac</span></span>           | <span data-ttu-id="47e06-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="47e06-125">Boolean</span></span> |
| <span data-ttu-id="47e06-126">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="47e06-126">usedAndroidPhone</span></span>  | <span data-ttu-id="47e06-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="47e06-127">Boolean</span></span> |
| <span data-ttu-id="47e06-128">usedWindows</span><span class="sxs-lookup"><span data-stu-id="47e06-128">usedWindows</span></span>       | <span data-ttu-id="47e06-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="47e06-129">Boolean</span></span> |
| <span data-ttu-id="47e06-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="47e06-130">reportPeriod</span></span>      | <span data-ttu-id="47e06-131">String</span><span class="sxs-lookup"><span data-stu-id="47e06-131">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="47e06-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47e06-132">JSON representation</span></span>

<span data-ttu-id="47e06-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47e06-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```
