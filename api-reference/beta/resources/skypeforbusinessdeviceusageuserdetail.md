---
title: tipo de recurso skypeForBusinessDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 36cd6aba954206b60317520534284cd17f8d42e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997526"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="e5182-103">tipo de recurso skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="e5182-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="e5182-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5182-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e5182-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5182-105">Properties</span></span>

| <span data-ttu-id="e5182-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5182-106">Property</span></span>          | <span data-ttu-id="e5182-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5182-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="e5182-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e5182-108">reportRefreshDate</span></span> | <span data-ttu-id="e5182-109">Data</span><span class="sxs-lookup"><span data-stu-id="e5182-109">Date</span></span>    |
| <span data-ttu-id="e5182-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e5182-110">userPrincipalName</span></span> | <span data-ttu-id="e5182-111">String</span><span class="sxs-lookup"><span data-stu-id="e5182-111">String</span></span>  |
| <span data-ttu-id="e5182-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e5182-112">lastActivityDate</span></span>  | <span data-ttu-id="e5182-113">Data</span><span class="sxs-lookup"><span data-stu-id="e5182-113">Date</span></span>    |
| <span data-ttu-id="e5182-114">usedWindows</span><span class="sxs-lookup"><span data-stu-id="e5182-114">usedWindows</span></span>       | <span data-ttu-id="e5182-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5182-115">Boolean</span></span> |
| <span data-ttu-id="e5182-116">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="e5182-116">usedWindowsPhone</span></span>  | <span data-ttu-id="e5182-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5182-117">Boolean</span></span> |
| <span data-ttu-id="e5182-118">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="e5182-118">usedAndroidPhone</span></span>  | <span data-ttu-id="e5182-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5182-119">Boolean</span></span> |
| <span data-ttu-id="e5182-120">usediPhone</span><span class="sxs-lookup"><span data-stu-id="e5182-120">usediPhone</span></span>        | <span data-ttu-id="e5182-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5182-121">Boolean</span></span> |
| <span data-ttu-id="e5182-122">usediPad</span><span class="sxs-lookup"><span data-stu-id="e5182-122">usediPad</span></span>          | <span data-ttu-id="e5182-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5182-123">Boolean</span></span> |
| <span data-ttu-id="e5182-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e5182-124">reportPeriod</span></span>      | <span data-ttu-id="e5182-125">String</span><span class="sxs-lookup"><span data-stu-id="e5182-125">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e5182-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5182-126">JSON representation</span></span>

<span data-ttu-id="e5182-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5182-127">The following is a JSON representation of the resource.</span></span>

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


