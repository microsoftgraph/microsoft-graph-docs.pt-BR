---
title: tipo de recurso yammerDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 083ace4b10b24e8e5de5d287ddf418d93658c879
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006973"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="74020-103">tipo de recurso yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="74020-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="74020-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74020-104">Properties</span></span>

| <span data-ttu-id="74020-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74020-105">Property</span></span>          | <span data-ttu-id="74020-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="74020-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="74020-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="74020-107">reportRefreshDate</span></span> | <span data-ttu-id="74020-108">Data</span><span class="sxs-lookup"><span data-stu-id="74020-108">Date</span></span>    |
| <span data-ttu-id="74020-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74020-109">userPrincipalName</span></span> | <span data-ttu-id="74020-110">String</span><span class="sxs-lookup"><span data-stu-id="74020-110">String</span></span>  |
| <span data-ttu-id="74020-111">displayName</span><span class="sxs-lookup"><span data-stu-id="74020-111">displayName</span></span>       | <span data-ttu-id="74020-112">String</span><span class="sxs-lookup"><span data-stu-id="74020-112">String</span></span>  |
| <span data-ttu-id="74020-113">userState</span><span class="sxs-lookup"><span data-stu-id="74020-113">userState</span></span>         | <span data-ttu-id="74020-114">String</span><span class="sxs-lookup"><span data-stu-id="74020-114">String</span></span>  |
| <span data-ttu-id="74020-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="74020-115">stateChangeDate</span></span>   | <span data-ttu-id="74020-116">Data</span><span class="sxs-lookup"><span data-stu-id="74020-116">Date</span></span>    |
| <span data-ttu-id="74020-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="74020-117">lastActivityDate</span></span>  | <span data-ttu-id="74020-118">Data</span><span class="sxs-lookup"><span data-stu-id="74020-118">Date</span></span>    |
| <span data-ttu-id="74020-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="74020-119">usedWeb</span></span>           | <span data-ttu-id="74020-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="74020-120">Boolean</span></span> |
| <span data-ttu-id="74020-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="74020-121">usedWindowsPhone</span></span>  | <span data-ttu-id="74020-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="74020-122">Boolean</span></span> |
| <span data-ttu-id="74020-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="74020-123">usedAndroidPhone</span></span>  | <span data-ttu-id="74020-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="74020-124">Boolean</span></span> |
| <span data-ttu-id="74020-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="74020-125">usediPhone</span></span>        | <span data-ttu-id="74020-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="74020-126">Boolean</span></span> |
| <span data-ttu-id="74020-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="74020-127">usediPad</span></span>          | <span data-ttu-id="74020-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="74020-128">Boolean</span></span> |
| <span data-ttu-id="74020-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="74020-129">usedOthers</span></span>        | <span data-ttu-id="74020-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="74020-130">Boolean</span></span> |
| <span data-ttu-id="74020-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="74020-131">reportPeriod</span></span>      | <span data-ttu-id="74020-132">String</span><span class="sxs-lookup"><span data-stu-id="74020-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="74020-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74020-133">JSON representation</span></span>

<span data-ttu-id="74020-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74020-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "usedOthers": true, 
  "reportPeriod": "String"
}
```
