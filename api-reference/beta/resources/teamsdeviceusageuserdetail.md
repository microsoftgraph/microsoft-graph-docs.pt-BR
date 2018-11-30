---
title: tipo de recurso de teamsDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 4eeec5f07a0a604249617ac87a62ea12b4052395
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040428"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="a97f6-103">tipo de recurso de teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="a97f6-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a97f6-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a97f6-104">Properties</span></span>

| <span data-ttu-id="a97f6-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a97f6-105">Property</span></span>          | <span data-ttu-id="a97f6-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a97f6-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="a97f6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a97f6-107">reportRefreshDate</span></span> | <span data-ttu-id="a97f6-108">Data</span><span class="sxs-lookup"><span data-stu-id="a97f6-108">Date</span></span>    |
| <span data-ttu-id="a97f6-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a97f6-109">userPrincipalName</span></span> | <span data-ttu-id="a97f6-110">String</span><span class="sxs-lookup"><span data-stu-id="a97f6-110">String</span></span>  |
| <span data-ttu-id="a97f6-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a97f6-111">lastActivityDate</span></span>  | <span data-ttu-id="a97f6-112">Data</span><span class="sxs-lookup"><span data-stu-id="a97f6-112">Date</span></span>    |
| <span data-ttu-id="a97f6-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a97f6-113">isDeleted</span></span>         | <span data-ttu-id="a97f6-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="a97f6-114">Boolean</span></span> |
| <span data-ttu-id="a97f6-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="a97f6-115">deletedDate</span></span>       | <span data-ttu-id="a97f6-116">Data</span><span class="sxs-lookup"><span data-stu-id="a97f6-116">Date</span></span>    |
| <span data-ttu-id="a97f6-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="a97f6-117">usedWeb</span></span>           | <span data-ttu-id="a97f6-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="a97f6-118">Boolean</span></span> |
| <span data-ttu-id="a97f6-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="a97f6-119">usedWindowsPhone</span></span>  | <span data-ttu-id="a97f6-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="a97f6-120">Boolean</span></span> |
| <span data-ttu-id="a97f6-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="a97f6-121">usediOS</span></span>           | <span data-ttu-id="a97f6-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="a97f6-122">Boolean</span></span> |
| <span data-ttu-id="a97f6-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="a97f6-123">usedMac</span></span>           | <span data-ttu-id="a97f6-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="a97f6-124">Boolean</span></span> |
| <span data-ttu-id="a97f6-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="a97f6-125">usedAndroidPhone</span></span>  | <span data-ttu-id="a97f6-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="a97f6-126">Boolean</span></span> |
| <span data-ttu-id="a97f6-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="a97f6-127">usedWindows</span></span>       | <span data-ttu-id="a97f6-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="a97f6-128">Boolean</span></span> |
| <span data-ttu-id="a97f6-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a97f6-129">reportPeriod</span></span>      | <span data-ttu-id="a97f6-130">String</span><span class="sxs-lookup"><span data-stu-id="a97f6-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a97f6-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a97f6-131">JSON representation</span></span>

<span data-ttu-id="a97f6-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a97f6-132">The following is a JSON representation of the resource.</span></span>

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
