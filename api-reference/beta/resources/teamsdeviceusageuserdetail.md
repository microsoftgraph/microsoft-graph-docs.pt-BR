---
title: tipo de recurso de teamsDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06e2cea1154c608b61642b07adbd96aae1710903
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807102"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="ab1a9-103">tipo de recurso de teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="ab1a9-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ab1a9-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab1a9-104">Properties</span></span>

| <span data-ttu-id="ab1a9-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab1a9-105">Property</span></span>          | <span data-ttu-id="ab1a9-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab1a9-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="ab1a9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ab1a9-107">reportRefreshDate</span></span> | <span data-ttu-id="ab1a9-108">Data</span><span class="sxs-lookup"><span data-stu-id="ab1a9-108">Date</span></span>    |
| <span data-ttu-id="ab1a9-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ab1a9-109">userPrincipalName</span></span> | <span data-ttu-id="ab1a9-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab1a9-110">String</span></span>  |
| <span data-ttu-id="ab1a9-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ab1a9-111">lastActivityDate</span></span>  | <span data-ttu-id="ab1a9-112">Data</span><span class="sxs-lookup"><span data-stu-id="ab1a9-112">Date</span></span>    |
| <span data-ttu-id="ab1a9-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ab1a9-113">isDeleted</span></span>         | <span data-ttu-id="ab1a9-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab1a9-114">Boolean</span></span> |
| <span data-ttu-id="ab1a9-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="ab1a9-115">deletedDate</span></span>       | <span data-ttu-id="ab1a9-116">Data</span><span class="sxs-lookup"><span data-stu-id="ab1a9-116">Date</span></span>    |
| <span data-ttu-id="ab1a9-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="ab1a9-117">usedWeb</span></span>           | <span data-ttu-id="ab1a9-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab1a9-118">Boolean</span></span> |
| <span data-ttu-id="ab1a9-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="ab1a9-119">usedWindowsPhone</span></span>  | <span data-ttu-id="ab1a9-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab1a9-120">Boolean</span></span> |
| <span data-ttu-id="ab1a9-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="ab1a9-121">usediOS</span></span>           | <span data-ttu-id="ab1a9-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab1a9-122">Boolean</span></span> |
| <span data-ttu-id="ab1a9-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="ab1a9-123">usedMac</span></span>           | <span data-ttu-id="ab1a9-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab1a9-124">Boolean</span></span> |
| <span data-ttu-id="ab1a9-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="ab1a9-125">usedAndroidPhone</span></span>  | <span data-ttu-id="ab1a9-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab1a9-126">Boolean</span></span> |
| <span data-ttu-id="ab1a9-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="ab1a9-127">usedWindows</span></span>       | <span data-ttu-id="ab1a9-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab1a9-128">Boolean</span></span> |
| <span data-ttu-id="ab1a9-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ab1a9-129">reportPeriod</span></span>      | <span data-ttu-id="ab1a9-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab1a9-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ab1a9-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab1a9-131">JSON representation</span></span>

<span data-ttu-id="ab1a9-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab1a9-132">The following is a JSON representation of the resource.</span></span>

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
