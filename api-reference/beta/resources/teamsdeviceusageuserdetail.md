---
title: tipo de recurso teamsDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5bd7443e775a8a9de0dbbc27cf8843331f8f8cb7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007622"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="ec309-103">tipo de recurso teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="ec309-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ec309-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec309-104">Properties</span></span>

| <span data-ttu-id="ec309-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec309-105">Property</span></span>          | <span data-ttu-id="ec309-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec309-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="ec309-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ec309-107">reportRefreshDate</span></span> | <span data-ttu-id="ec309-108">Data</span><span class="sxs-lookup"><span data-stu-id="ec309-108">Date</span></span>    |
| <span data-ttu-id="ec309-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ec309-109">userPrincipalName</span></span> | <span data-ttu-id="ec309-110">String</span><span class="sxs-lookup"><span data-stu-id="ec309-110">String</span></span>  |
| <span data-ttu-id="ec309-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ec309-111">lastActivityDate</span></span>  | <span data-ttu-id="ec309-112">Data</span><span class="sxs-lookup"><span data-stu-id="ec309-112">Date</span></span>    |
| <span data-ttu-id="ec309-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ec309-113">isDeleted</span></span>         | <span data-ttu-id="ec309-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec309-114">Boolean</span></span> |
| <span data-ttu-id="ec309-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="ec309-115">deletedDate</span></span>       | <span data-ttu-id="ec309-116">Data</span><span class="sxs-lookup"><span data-stu-id="ec309-116">Date</span></span>    |
| <span data-ttu-id="ec309-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="ec309-117">usedWeb</span></span>           | <span data-ttu-id="ec309-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec309-118">Boolean</span></span> |
| <span data-ttu-id="ec309-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="ec309-119">usedWindowsPhone</span></span>  | <span data-ttu-id="ec309-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec309-120">Boolean</span></span> |
| <span data-ttu-id="ec309-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="ec309-121">usediOS</span></span>           | <span data-ttu-id="ec309-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec309-122">Boolean</span></span> |
| <span data-ttu-id="ec309-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="ec309-123">usedMac</span></span>           | <span data-ttu-id="ec309-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec309-124">Boolean</span></span> |
| <span data-ttu-id="ec309-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="ec309-125">usedAndroidPhone</span></span>  | <span data-ttu-id="ec309-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec309-126">Boolean</span></span> |
| <span data-ttu-id="ec309-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="ec309-127">usedWindows</span></span>       | <span data-ttu-id="ec309-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec309-128">Boolean</span></span> |
| <span data-ttu-id="ec309-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ec309-129">reportPeriod</span></span>      | <span data-ttu-id="ec309-130">String</span><span class="sxs-lookup"><span data-stu-id="ec309-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ec309-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec309-131">JSON representation</span></span>

<span data-ttu-id="ec309-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec309-132">The following is a JSON representation of the resource.</span></span>

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
