---
title: tipo de recurso skypeForBusinessDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 50f37fdfd3441c256241b76ebcc6b144eb1486d7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811045"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="39d89-103">tipo de recurso skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="39d89-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="39d89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39d89-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="39d89-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39d89-105">Properties</span></span>

| <span data-ttu-id="39d89-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39d89-106">Property</span></span>          | <span data-ttu-id="39d89-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="39d89-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="39d89-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="39d89-108">reportRefreshDate</span></span> | <span data-ttu-id="39d89-109">Data</span><span class="sxs-lookup"><span data-stu-id="39d89-109">Date</span></span>    |
| <span data-ttu-id="39d89-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="39d89-110">userPrincipalName</span></span> | <span data-ttu-id="39d89-111">String</span><span class="sxs-lookup"><span data-stu-id="39d89-111">String</span></span>  |
| <span data-ttu-id="39d89-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="39d89-112">lastActivityDate</span></span>  | <span data-ttu-id="39d89-113">Data</span><span class="sxs-lookup"><span data-stu-id="39d89-113">Date</span></span>    |
| <span data-ttu-id="39d89-114">usedWindows</span><span class="sxs-lookup"><span data-stu-id="39d89-114">usedWindows</span></span>       | <span data-ttu-id="39d89-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="39d89-115">Boolean</span></span> |
| <span data-ttu-id="39d89-116">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="39d89-116">usedWindowsPhone</span></span>  | <span data-ttu-id="39d89-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="39d89-117">Boolean</span></span> |
| <span data-ttu-id="39d89-118">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="39d89-118">usedAndroidPhone</span></span>  | <span data-ttu-id="39d89-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="39d89-119">Boolean</span></span> |
| <span data-ttu-id="39d89-120">usediPhone</span><span class="sxs-lookup"><span data-stu-id="39d89-120">usediPhone</span></span>        | <span data-ttu-id="39d89-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="39d89-121">Boolean</span></span> |
| <span data-ttu-id="39d89-122">usediPad</span><span class="sxs-lookup"><span data-stu-id="39d89-122">usediPad</span></span>          | <span data-ttu-id="39d89-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="39d89-123">Boolean</span></span> |
| <span data-ttu-id="39d89-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="39d89-124">reportPeriod</span></span>      | <span data-ttu-id="39d89-125">String</span><span class="sxs-lookup"><span data-stu-id="39d89-125">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="39d89-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39d89-126">JSON representation</span></span>

<span data-ttu-id="39d89-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39d89-127">The following is a JSON representation of the resource.</span></span>

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
