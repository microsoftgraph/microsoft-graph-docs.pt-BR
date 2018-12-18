---
title: tipo de recurso de teamsDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
ms.openlocfilehash: 1947b66a59190945e5a6b823b47ef8df7d02683a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328998"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="69a76-103">tipo de recurso de teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="69a76-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="69a76-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69a76-104">Properties</span></span>

| <span data-ttu-id="69a76-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69a76-105">Property</span></span>          | <span data-ttu-id="69a76-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="69a76-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="69a76-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="69a76-107">reportRefreshDate</span></span> | <span data-ttu-id="69a76-108">Data</span><span class="sxs-lookup"><span data-stu-id="69a76-108">Date</span></span>    |
| <span data-ttu-id="69a76-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="69a76-109">userPrincipalName</span></span> | <span data-ttu-id="69a76-110">String</span><span class="sxs-lookup"><span data-stu-id="69a76-110">String</span></span>  |
| <span data-ttu-id="69a76-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="69a76-111">lastActivityDate</span></span>  | <span data-ttu-id="69a76-112">Data</span><span class="sxs-lookup"><span data-stu-id="69a76-112">Date</span></span>    |
| <span data-ttu-id="69a76-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="69a76-113">isDeleted</span></span>         | <span data-ttu-id="69a76-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="69a76-114">Boolean</span></span> |
| <span data-ttu-id="69a76-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="69a76-115">deletedDate</span></span>       | <span data-ttu-id="69a76-116">Data</span><span class="sxs-lookup"><span data-stu-id="69a76-116">Date</span></span>    |
| <span data-ttu-id="69a76-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="69a76-117">usedWeb</span></span>           | <span data-ttu-id="69a76-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="69a76-118">Boolean</span></span> |
| <span data-ttu-id="69a76-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="69a76-119">usedWindowsPhone</span></span>  | <span data-ttu-id="69a76-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="69a76-120">Boolean</span></span> |
| <span data-ttu-id="69a76-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="69a76-121">usediOS</span></span>           | <span data-ttu-id="69a76-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="69a76-122">Boolean</span></span> |
| <span data-ttu-id="69a76-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="69a76-123">usedMac</span></span>           | <span data-ttu-id="69a76-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="69a76-124">Boolean</span></span> |
| <span data-ttu-id="69a76-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="69a76-125">usedAndroidPhone</span></span>  | <span data-ttu-id="69a76-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="69a76-126">Boolean</span></span> |
| <span data-ttu-id="69a76-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="69a76-127">usedWindows</span></span>       | <span data-ttu-id="69a76-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="69a76-128">Boolean</span></span> |
| <span data-ttu-id="69a76-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="69a76-129">reportPeriod</span></span>      | <span data-ttu-id="69a76-130">String</span><span class="sxs-lookup"><span data-stu-id="69a76-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="69a76-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69a76-131">JSON representation</span></span>

<span data-ttu-id="69a76-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69a76-132">The following is a JSON representation of the resource.</span></span>

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
