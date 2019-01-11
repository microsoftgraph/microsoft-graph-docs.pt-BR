---
title: tipo de recurso de siteUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 1f656feacdbba3418049bd9f3072270aa04af798
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879923"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="80154-103">tipo de recurso de siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="80154-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="80154-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80154-104">Properties</span></span>

| <span data-ttu-id="80154-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80154-105">Property</span></span>           | <span data-ttu-id="80154-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="80154-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="80154-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="80154-107">reportRefreshDate</span></span>  | <span data-ttu-id="80154-108">Data</span><span class="sxs-lookup"><span data-stu-id="80154-108">Date</span></span>   |
| <span data-ttu-id="80154-109">siteType</span><span class="sxs-lookup"><span data-stu-id="80154-109">siteType</span></span>           | <span data-ttu-id="80154-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80154-110">String</span></span> |
| <span data-ttu-id="80154-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="80154-111">storageUsedInBytes</span></span> | <span data-ttu-id="80154-112">Int64</span><span class="sxs-lookup"><span data-stu-id="80154-112">Int64</span></span>  |
| <span data-ttu-id="80154-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="80154-113">reportDate</span></span>         | <span data-ttu-id="80154-114">Data</span><span class="sxs-lookup"><span data-stu-id="80154-114">Date</span></span>   |
| <span data-ttu-id="80154-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="80154-115">reportPeriod</span></span>       | <span data-ttu-id="80154-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80154-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="80154-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80154-117">JSON representation</span></span>

<span data-ttu-id="80154-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80154-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
