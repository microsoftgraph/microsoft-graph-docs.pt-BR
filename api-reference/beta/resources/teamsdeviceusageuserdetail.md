---
title: tipo de recurso teamsDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ddfdef3e9d5500951fc24de5beb333e822c9bbda
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046451"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="e031b-103">tipo de recurso teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="e031b-103">teamsDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="e031b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e031b-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e031b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e031b-105">Properties</span></span>

| <span data-ttu-id="e031b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e031b-106">Property</span></span>          | <span data-ttu-id="e031b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e031b-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="e031b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e031b-108">reportRefreshDate</span></span> | <span data-ttu-id="e031b-109">Data</span><span class="sxs-lookup"><span data-stu-id="e031b-109">Date</span></span>    |
| <span data-ttu-id="e031b-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e031b-110">userPrincipalName</span></span> | <span data-ttu-id="e031b-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e031b-111">String</span></span>  |
| <span data-ttu-id="e031b-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e031b-112">lastActivityDate</span></span>  | <span data-ttu-id="e031b-113">Data</span><span class="sxs-lookup"><span data-stu-id="e031b-113">Date</span></span>    |
| <span data-ttu-id="e031b-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e031b-114">isDeleted</span></span>         | <span data-ttu-id="e031b-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="e031b-115">Boolean</span></span> |
| <span data-ttu-id="e031b-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="e031b-116">deletedDate</span></span>       | <span data-ttu-id="e031b-117">Data</span><span class="sxs-lookup"><span data-stu-id="e031b-117">Date</span></span>    |
| <span data-ttu-id="e031b-118">usedWeb</span><span class="sxs-lookup"><span data-stu-id="e031b-118">usedWeb</span></span>           | <span data-ttu-id="e031b-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="e031b-119">Boolean</span></span> |
| <span data-ttu-id="e031b-120">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="e031b-120">usedWindowsPhone</span></span>  | <span data-ttu-id="e031b-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="e031b-121">Boolean</span></span> |
| <span data-ttu-id="e031b-122">usediOS</span><span class="sxs-lookup"><span data-stu-id="e031b-122">usediOS</span></span>           | <span data-ttu-id="e031b-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="e031b-123">Boolean</span></span> |
| <span data-ttu-id="e031b-124">usedMac</span><span class="sxs-lookup"><span data-stu-id="e031b-124">usedMac</span></span>           | <span data-ttu-id="e031b-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="e031b-125">Boolean</span></span> |
| <span data-ttu-id="e031b-126">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="e031b-126">usedAndroidPhone</span></span>  | <span data-ttu-id="e031b-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="e031b-127">Boolean</span></span> |
| <span data-ttu-id="e031b-128">usedWindows</span><span class="sxs-lookup"><span data-stu-id="e031b-128">usedWindows</span></span>       | <span data-ttu-id="e031b-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="e031b-129">Boolean</span></span> |
| <span data-ttu-id="e031b-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e031b-130">reportPeriod</span></span>      | <span data-ttu-id="e031b-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e031b-131">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e031b-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e031b-132">JSON representation</span></span>

<span data-ttu-id="e031b-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e031b-133">The following is a JSON representation of the resource.</span></span>

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


