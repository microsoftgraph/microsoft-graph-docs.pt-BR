---
title: tipo de recurso de skypeForBusinessDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: b62920d124fd52e0f653c128eeb0956cdfe0c680
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034712"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="ccd31-103">tipo de recurso de skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="ccd31-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ccd31-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccd31-104">Properties</span></span>

| <span data-ttu-id="ccd31-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccd31-105">Property</span></span>          | <span data-ttu-id="ccd31-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccd31-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="ccd31-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ccd31-107">reportRefreshDate</span></span> | <span data-ttu-id="ccd31-108">Data</span><span class="sxs-lookup"><span data-stu-id="ccd31-108">Date</span></span>    |
| <span data-ttu-id="ccd31-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ccd31-109">userPrincipalName</span></span> | <span data-ttu-id="ccd31-110">String</span><span class="sxs-lookup"><span data-stu-id="ccd31-110">String</span></span>  |
| <span data-ttu-id="ccd31-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ccd31-111">lastActivityDate</span></span>  | <span data-ttu-id="ccd31-112">Data</span><span class="sxs-lookup"><span data-stu-id="ccd31-112">Date</span></span>    |
| <span data-ttu-id="ccd31-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="ccd31-113">usedWindows</span></span>       | <span data-ttu-id="ccd31-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccd31-114">Boolean</span></span> |
| <span data-ttu-id="ccd31-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="ccd31-115">usedWindowsPhone</span></span>  | <span data-ttu-id="ccd31-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccd31-116">Boolean</span></span> |
| <span data-ttu-id="ccd31-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="ccd31-117">usedAndroidPhone</span></span>  | <span data-ttu-id="ccd31-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccd31-118">Boolean</span></span> |
| <span data-ttu-id="ccd31-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="ccd31-119">usediPhone</span></span>        | <span data-ttu-id="ccd31-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccd31-120">Boolean</span></span> |
| <span data-ttu-id="ccd31-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="ccd31-121">usediPad</span></span>          | <span data-ttu-id="ccd31-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccd31-122">Boolean</span></span> |
| <span data-ttu-id="ccd31-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ccd31-123">reportPeriod</span></span>      | <span data-ttu-id="ccd31-124">String</span><span class="sxs-lookup"><span data-stu-id="ccd31-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ccd31-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccd31-125">JSON representation</span></span>

<span data-ttu-id="ccd31-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccd31-126">The following is a JSON representation of the resource.</span></span>

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
