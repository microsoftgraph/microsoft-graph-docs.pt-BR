---
title: tipo de recurso skypeForBusinessDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b84cf9c7654354446fb7c6a5005befe3d17a0fa4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964911"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="e514f-103">tipo de recurso skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="e514f-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e514f-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e514f-104">Properties</span></span>

| <span data-ttu-id="e514f-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e514f-105">Property</span></span>          | <span data-ttu-id="e514f-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e514f-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="e514f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e514f-107">reportRefreshDate</span></span> | <span data-ttu-id="e514f-108">Data</span><span class="sxs-lookup"><span data-stu-id="e514f-108">Date</span></span>    |
| <span data-ttu-id="e514f-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e514f-109">userPrincipalName</span></span> | <span data-ttu-id="e514f-110">String</span><span class="sxs-lookup"><span data-stu-id="e514f-110">String</span></span>  |
| <span data-ttu-id="e514f-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e514f-111">lastActivityDate</span></span>  | <span data-ttu-id="e514f-112">Data</span><span class="sxs-lookup"><span data-stu-id="e514f-112">Date</span></span>    |
| <span data-ttu-id="e514f-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="e514f-113">usedWindows</span></span>       | <span data-ttu-id="e514f-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="e514f-114">Boolean</span></span> |
| <span data-ttu-id="e514f-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="e514f-115">usedWindowsPhone</span></span>  | <span data-ttu-id="e514f-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="e514f-116">Boolean</span></span> |
| <span data-ttu-id="e514f-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="e514f-117">usedAndroidPhone</span></span>  | <span data-ttu-id="e514f-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="e514f-118">Boolean</span></span> |
| <span data-ttu-id="e514f-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="e514f-119">usediPhone</span></span>        | <span data-ttu-id="e514f-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="e514f-120">Boolean</span></span> |
| <span data-ttu-id="e514f-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="e514f-121">usediPad</span></span>          | <span data-ttu-id="e514f-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="e514f-122">Boolean</span></span> |
| <span data-ttu-id="e514f-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e514f-123">reportPeriod</span></span>      | <span data-ttu-id="e514f-124">String</span><span class="sxs-lookup"><span data-stu-id="e514f-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e514f-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e514f-125">JSON representation</span></span>

<span data-ttu-id="e514f-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e514f-126">The following is a JSON representation of the resource.</span></span>

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
