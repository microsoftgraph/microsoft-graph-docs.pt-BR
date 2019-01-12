---
title: tipo de recurso de teamsDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8cdd2fe1a212bb1d36846b80fc1b558c576deb47
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953782"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="116d8-103">tipo de recurso de teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="116d8-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="116d8-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="116d8-104">Properties</span></span>

| <span data-ttu-id="116d8-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="116d8-105">Property</span></span>          | <span data-ttu-id="116d8-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="116d8-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="116d8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="116d8-107">reportRefreshDate</span></span> | <span data-ttu-id="116d8-108">Data</span><span class="sxs-lookup"><span data-stu-id="116d8-108">Date</span></span>    |
| <span data-ttu-id="116d8-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="116d8-109">userPrincipalName</span></span> | <span data-ttu-id="116d8-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="116d8-110">String</span></span>  |
| <span data-ttu-id="116d8-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="116d8-111">lastActivityDate</span></span>  | <span data-ttu-id="116d8-112">Data</span><span class="sxs-lookup"><span data-stu-id="116d8-112">Date</span></span>    |
| <span data-ttu-id="116d8-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="116d8-113">isDeleted</span></span>         | <span data-ttu-id="116d8-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="116d8-114">Boolean</span></span> |
| <span data-ttu-id="116d8-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="116d8-115">deletedDate</span></span>       | <span data-ttu-id="116d8-116">Data</span><span class="sxs-lookup"><span data-stu-id="116d8-116">Date</span></span>    |
| <span data-ttu-id="116d8-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="116d8-117">usedWeb</span></span>           | <span data-ttu-id="116d8-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="116d8-118">Boolean</span></span> |
| <span data-ttu-id="116d8-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="116d8-119">usedWindowsPhone</span></span>  | <span data-ttu-id="116d8-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="116d8-120">Boolean</span></span> |
| <span data-ttu-id="116d8-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="116d8-121">usediOS</span></span>           | <span data-ttu-id="116d8-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="116d8-122">Boolean</span></span> |
| <span data-ttu-id="116d8-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="116d8-123">usedMac</span></span>           | <span data-ttu-id="116d8-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="116d8-124">Boolean</span></span> |
| <span data-ttu-id="116d8-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="116d8-125">usedAndroidPhone</span></span>  | <span data-ttu-id="116d8-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="116d8-126">Boolean</span></span> |
| <span data-ttu-id="116d8-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="116d8-127">usedWindows</span></span>       | <span data-ttu-id="116d8-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="116d8-128">Boolean</span></span> |
| <span data-ttu-id="116d8-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="116d8-129">reportPeriod</span></span>      | <span data-ttu-id="116d8-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="116d8-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="116d8-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="116d8-131">JSON representation</span></span>

<span data-ttu-id="116d8-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="116d8-132">The following is a JSON representation of the resource.</span></span>

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
