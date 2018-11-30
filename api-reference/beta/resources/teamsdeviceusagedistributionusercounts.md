---
title: tipo de recurso de teamsDeviceUsageDistributionUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: b039320e389e1a61832089991b2368b27e51c475
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033400"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="4b416-103">tipo de recurso de teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="4b416-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4b416-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b416-104">Properties</span></span>

| <span data-ttu-id="4b416-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b416-105">Property</span></span>          | <span data-ttu-id="4b416-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b416-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4b416-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4b416-107">reportRefreshDate</span></span> | <span data-ttu-id="4b416-108">Data</span><span class="sxs-lookup"><span data-stu-id="4b416-108">Date</span></span>   |
| <span data-ttu-id="4b416-109">web</span><span class="sxs-lookup"><span data-stu-id="4b416-109">web</span></span>               | <span data-ttu-id="4b416-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4b416-110">Int64</span></span>  |
| <span data-ttu-id="4b416-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="4b416-111">windowsPhone</span></span>      | <span data-ttu-id="4b416-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4b416-112">Int64</span></span>  |
| <span data-ttu-id="4b416-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="4b416-113">androidPhone</span></span>      | <span data-ttu-id="4b416-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4b416-114">Int64</span></span>  |
| <span data-ttu-id="4b416-115">IOS</span><span class="sxs-lookup"><span data-stu-id="4b416-115">ios</span></span>               | <span data-ttu-id="4b416-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4b416-116">Int64</span></span>  |
| <span data-ttu-id="4b416-117">mac</span><span class="sxs-lookup"><span data-stu-id="4b416-117">mac</span></span>               | <span data-ttu-id="4b416-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4b416-118">Int64</span></span>  |
| <span data-ttu-id="4b416-119">Windows</span><span class="sxs-lookup"><span data-stu-id="4b416-119">windows</span></span>           | <span data-ttu-id="4b416-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4b416-120">Int64</span></span>  |
| <span data-ttu-id="4b416-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4b416-121">reportPeriod</span></span>      | <span data-ttu-id="4b416-122">String</span><span class="sxs-lookup"><span data-stu-id="4b416-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4b416-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b416-123">JSON representation</span></span>

<span data-ttu-id="4b416-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b416-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportPeriod": "String"
}
```
