---
title: tipo de recurso de skypeForBusinessDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858377"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="cc844-103">tipo de recurso de skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="cc844-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="cc844-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc844-104">Properties</span></span>

| <span data-ttu-id="cc844-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc844-105">Property</span></span>          | <span data-ttu-id="cc844-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc844-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="cc844-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cc844-107">reportRefreshDate</span></span> | <span data-ttu-id="cc844-108">Data</span><span class="sxs-lookup"><span data-stu-id="cc844-108">Date</span></span>    |
| <span data-ttu-id="cc844-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cc844-109">userPrincipalName</span></span> | <span data-ttu-id="cc844-110">String</span><span class="sxs-lookup"><span data-stu-id="cc844-110">String</span></span>  |
| <span data-ttu-id="cc844-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="cc844-111">lastActivityDate</span></span>  | <span data-ttu-id="cc844-112">Data</span><span class="sxs-lookup"><span data-stu-id="cc844-112">Date</span></span>    |
| <span data-ttu-id="cc844-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="cc844-113">usedWindows</span></span>       | <span data-ttu-id="cc844-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc844-114">Boolean</span></span> |
| <span data-ttu-id="cc844-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="cc844-115">usedWindowsPhone</span></span>  | <span data-ttu-id="cc844-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc844-116">Boolean</span></span> |
| <span data-ttu-id="cc844-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="cc844-117">usedAndroidPhone</span></span>  | <span data-ttu-id="cc844-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc844-118">Boolean</span></span> |
| <span data-ttu-id="cc844-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="cc844-119">usediPhone</span></span>        | <span data-ttu-id="cc844-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc844-120">Boolean</span></span> |
| <span data-ttu-id="cc844-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="cc844-121">usediPad</span></span>          | <span data-ttu-id="cc844-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc844-122">Boolean</span></span> |
| <span data-ttu-id="cc844-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cc844-123">reportPeriod</span></span>      | <span data-ttu-id="cc844-124">String</span><span class="sxs-lookup"><span data-stu-id="cc844-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="cc844-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc844-125">JSON representation</span></span>

<span data-ttu-id="cc844-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc844-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
