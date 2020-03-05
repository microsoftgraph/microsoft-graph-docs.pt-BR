---
title: tipo de recurso skypeForBusinessDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 582c3483d4292f634385461508bf579834dfd12e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520405"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="899b3-103">tipo de recurso skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="899b3-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="899b3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="899b3-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="899b3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="899b3-105">Properties</span></span>

| <span data-ttu-id="899b3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="899b3-106">Property</span></span>          | <span data-ttu-id="899b3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="899b3-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="899b3-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="899b3-108">reportRefreshDate</span></span> | <span data-ttu-id="899b3-109">Data</span><span class="sxs-lookup"><span data-stu-id="899b3-109">Date</span></span>    |
| <span data-ttu-id="899b3-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="899b3-110">userPrincipalName</span></span> | <span data-ttu-id="899b3-111">String</span><span class="sxs-lookup"><span data-stu-id="899b3-111">String</span></span>  |
| <span data-ttu-id="899b3-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="899b3-112">lastActivityDate</span></span>  | <span data-ttu-id="899b3-113">Data</span><span class="sxs-lookup"><span data-stu-id="899b3-113">Date</span></span>    |
| <span data-ttu-id="899b3-114">usedWindows</span><span class="sxs-lookup"><span data-stu-id="899b3-114">usedWindows</span></span>       | <span data-ttu-id="899b3-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="899b3-115">Boolean</span></span> |
| <span data-ttu-id="899b3-116">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="899b3-116">usedWindowsPhone</span></span>  | <span data-ttu-id="899b3-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="899b3-117">Boolean</span></span> |
| <span data-ttu-id="899b3-118">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="899b3-118">usedAndroidPhone</span></span>  | <span data-ttu-id="899b3-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="899b3-119">Boolean</span></span> |
| <span data-ttu-id="899b3-120">usediPhone</span><span class="sxs-lookup"><span data-stu-id="899b3-120">usediPhone</span></span>        | <span data-ttu-id="899b3-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="899b3-121">Boolean</span></span> |
| <span data-ttu-id="899b3-122">usediPad</span><span class="sxs-lookup"><span data-stu-id="899b3-122">usediPad</span></span>          | <span data-ttu-id="899b3-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="899b3-123">Boolean</span></span> |
| <span data-ttu-id="899b3-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="899b3-124">reportPeriod</span></span>      | <span data-ttu-id="899b3-125">String</span><span class="sxs-lookup"><span data-stu-id="899b3-125">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="899b3-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="899b3-126">JSON representation</span></span>

<span data-ttu-id="899b3-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="899b3-127">The following is a JSON representation of the resource.</span></span>

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
