---
title: tipo de recurso de oneDriveUsageFileCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 98e387b97687a4aab55e8d94e72fdbfa585a0e84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034048"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="eeb80-103">tipo de recurso de oneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="eeb80-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="eeb80-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eeb80-104">Properties</span></span>

| <span data-ttu-id="eeb80-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eeb80-105">Property</span></span>          | <span data-ttu-id="eeb80-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeb80-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="eeb80-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="eeb80-107">reportRefreshDate</span></span> | <span data-ttu-id="eeb80-108">Data</span><span class="sxs-lookup"><span data-stu-id="eeb80-108">Date</span></span>   |
| <span data-ttu-id="eeb80-109">siteType</span><span class="sxs-lookup"><span data-stu-id="eeb80-109">siteType</span></span>          | <span data-ttu-id="eeb80-110">String</span><span class="sxs-lookup"><span data-stu-id="eeb80-110">String</span></span> |
| <span data-ttu-id="eeb80-111">total</span><span class="sxs-lookup"><span data-stu-id="eeb80-111">total</span></span>             | <span data-ttu-id="eeb80-112">Int64</span><span class="sxs-lookup"><span data-stu-id="eeb80-112">Int64</span></span>  |
| <span data-ttu-id="eeb80-113">ativo</span><span class="sxs-lookup"><span data-stu-id="eeb80-113">active</span></span>            | <span data-ttu-id="eeb80-114">Int64</span><span class="sxs-lookup"><span data-stu-id="eeb80-114">Int64</span></span>  |
| <span data-ttu-id="eeb80-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="eeb80-115">reportDate</span></span>        | <span data-ttu-id="eeb80-116">Data</span><span class="sxs-lookup"><span data-stu-id="eeb80-116">Date</span></span>   |
| <span data-ttu-id="eeb80-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="eeb80-117">reportPeriod</span></span>      | <span data-ttu-id="eeb80-118">String</span><span class="sxs-lookup"><span data-stu-id="eeb80-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eeb80-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eeb80-119">JSON representation</span></span>

<span data-ttu-id="eeb80-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eeb80-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
