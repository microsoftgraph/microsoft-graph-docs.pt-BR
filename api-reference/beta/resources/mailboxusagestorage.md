---
title: tipo de recurso de mailboxUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: dcabfab0e8a64f2d74442f7d7464708501a59b95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840737"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="326f3-103">tipo de recurso de mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="326f3-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="326f3-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="326f3-104">Properties</span></span>

| <span data-ttu-id="326f3-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="326f3-105">Property</span></span>           | <span data-ttu-id="326f3-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="326f3-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="326f3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="326f3-107">reportRefreshDate</span></span>  | <span data-ttu-id="326f3-108">Data</span><span class="sxs-lookup"><span data-stu-id="326f3-108">Date</span></span>   |
| <span data-ttu-id="326f3-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="326f3-109">storageUsedInBytes</span></span> | <span data-ttu-id="326f3-110">Int64</span><span class="sxs-lookup"><span data-stu-id="326f3-110">Int64</span></span>  |
| <span data-ttu-id="326f3-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="326f3-111">reportDate</span></span>         | <span data-ttu-id="326f3-112">Data</span><span class="sxs-lookup"><span data-stu-id="326f3-112">Date</span></span>   |
| <span data-ttu-id="326f3-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="326f3-113">reportPeriod</span></span>       | <span data-ttu-id="326f3-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="326f3-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="326f3-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="326f3-115">JSON representation</span></span>

<span data-ttu-id="326f3-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="326f3-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
