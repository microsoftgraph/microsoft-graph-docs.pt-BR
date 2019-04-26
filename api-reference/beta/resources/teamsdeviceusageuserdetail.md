---
title: tipo de recurso teamsDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8cdd2fe1a212bb1d36846b80fc1b558c576deb47
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553600"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="7941a-103">tipo de recurso teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="7941a-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7941a-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7941a-104">Properties</span></span>

| <span data-ttu-id="7941a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7941a-105">Property</span></span>          | <span data-ttu-id="7941a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="7941a-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="7941a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7941a-107">reportRefreshDate</span></span> | <span data-ttu-id="7941a-108">Data</span><span class="sxs-lookup"><span data-stu-id="7941a-108">Date</span></span>    |
| <span data-ttu-id="7941a-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7941a-109">userPrincipalName</span></span> | <span data-ttu-id="7941a-110">String</span><span class="sxs-lookup"><span data-stu-id="7941a-110">String</span></span>  |
| <span data-ttu-id="7941a-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7941a-111">lastActivityDate</span></span>  | <span data-ttu-id="7941a-112">Data</span><span class="sxs-lookup"><span data-stu-id="7941a-112">Date</span></span>    |
| <span data-ttu-id="7941a-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="7941a-113">isDeleted</span></span>         | <span data-ttu-id="7941a-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="7941a-114">Boolean</span></span> |
| <span data-ttu-id="7941a-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="7941a-115">deletedDate</span></span>       | <span data-ttu-id="7941a-116">Data</span><span class="sxs-lookup"><span data-stu-id="7941a-116">Date</span></span>    |
| <span data-ttu-id="7941a-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="7941a-117">usedWeb</span></span>           | <span data-ttu-id="7941a-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="7941a-118">Boolean</span></span> |
| <span data-ttu-id="7941a-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="7941a-119">usedWindowsPhone</span></span>  | <span data-ttu-id="7941a-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="7941a-120">Boolean</span></span> |
| <span data-ttu-id="7941a-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="7941a-121">usediOS</span></span>           | <span data-ttu-id="7941a-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="7941a-122">Boolean</span></span> |
| <span data-ttu-id="7941a-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="7941a-123">usedMac</span></span>           | <span data-ttu-id="7941a-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="7941a-124">Boolean</span></span> |
| <span data-ttu-id="7941a-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="7941a-125">usedAndroidPhone</span></span>  | <span data-ttu-id="7941a-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="7941a-126">Boolean</span></span> |
| <span data-ttu-id="7941a-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="7941a-127">usedWindows</span></span>       | <span data-ttu-id="7941a-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="7941a-128">Boolean</span></span> |
| <span data-ttu-id="7941a-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7941a-129">reportPeriod</span></span>      | <span data-ttu-id="7941a-130">String</span><span class="sxs-lookup"><span data-stu-id="7941a-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="7941a-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7941a-131">JSON representation</span></span>

<span data-ttu-id="7941a-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7941a-132">The following is a JSON representation of the resource.</span></span>

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
