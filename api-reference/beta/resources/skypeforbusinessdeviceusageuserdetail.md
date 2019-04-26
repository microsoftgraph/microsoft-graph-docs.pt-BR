---
title: tipo de recurso skypeForBusinessDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555931"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="7bbec-103">tipo de recurso skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="7bbec-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7bbec-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bbec-104">Properties</span></span>

| <span data-ttu-id="7bbec-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bbec-105">Property</span></span>          | <span data-ttu-id="7bbec-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bbec-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="7bbec-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7bbec-107">reportRefreshDate</span></span> | <span data-ttu-id="7bbec-108">Data</span><span class="sxs-lookup"><span data-stu-id="7bbec-108">Date</span></span>    |
| <span data-ttu-id="7bbec-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7bbec-109">userPrincipalName</span></span> | <span data-ttu-id="7bbec-110">String</span><span class="sxs-lookup"><span data-stu-id="7bbec-110">String</span></span>  |
| <span data-ttu-id="7bbec-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7bbec-111">lastActivityDate</span></span>  | <span data-ttu-id="7bbec-112">Data</span><span class="sxs-lookup"><span data-stu-id="7bbec-112">Date</span></span>    |
| <span data-ttu-id="7bbec-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="7bbec-113">usedWindows</span></span>       | <span data-ttu-id="7bbec-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="7bbec-114">Boolean</span></span> |
| <span data-ttu-id="7bbec-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="7bbec-115">usedWindowsPhone</span></span>  | <span data-ttu-id="7bbec-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="7bbec-116">Boolean</span></span> |
| <span data-ttu-id="7bbec-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="7bbec-117">usedAndroidPhone</span></span>  | <span data-ttu-id="7bbec-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="7bbec-118">Boolean</span></span> |
| <span data-ttu-id="7bbec-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="7bbec-119">usediPhone</span></span>        | <span data-ttu-id="7bbec-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="7bbec-120">Boolean</span></span> |
| <span data-ttu-id="7bbec-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="7bbec-121">usediPad</span></span>          | <span data-ttu-id="7bbec-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="7bbec-122">Boolean</span></span> |
| <span data-ttu-id="7bbec-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7bbec-123">reportPeriod</span></span>      | <span data-ttu-id="7bbec-124">String</span><span class="sxs-lookup"><span data-stu-id="7bbec-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="7bbec-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bbec-125">JSON representation</span></span>

<span data-ttu-id="7bbec-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bbec-126">The following is a JSON representation of the resource.</span></span>

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
