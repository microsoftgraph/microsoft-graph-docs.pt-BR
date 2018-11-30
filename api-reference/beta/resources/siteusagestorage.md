---
title: tipo de recurso de siteUsageStorage
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 1fdfa6cb2690d6dbacf5e534792061b6e64025d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034384"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="8c4de-103">tipo de recurso de siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="8c4de-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8c4de-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c4de-104">Properties</span></span>

| <span data-ttu-id="8c4de-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c4de-105">Property</span></span>           | <span data-ttu-id="8c4de-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c4de-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="8c4de-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8c4de-107">reportRefreshDate</span></span>  | <span data-ttu-id="8c4de-108">Data</span><span class="sxs-lookup"><span data-stu-id="8c4de-108">Date</span></span>   |
| <span data-ttu-id="8c4de-109">siteType</span><span class="sxs-lookup"><span data-stu-id="8c4de-109">siteType</span></span>           | <span data-ttu-id="8c4de-110">String</span><span class="sxs-lookup"><span data-stu-id="8c4de-110">String</span></span> |
| <span data-ttu-id="8c4de-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="8c4de-111">storageUsedInBytes</span></span> | <span data-ttu-id="8c4de-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8c4de-112">Int64</span></span>  |
| <span data-ttu-id="8c4de-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="8c4de-113">reportDate</span></span>         | <span data-ttu-id="8c4de-114">Data</span><span class="sxs-lookup"><span data-stu-id="8c4de-114">Date</span></span>   |
| <span data-ttu-id="8c4de-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8c4de-115">reportPeriod</span></span>       | <span data-ttu-id="8c4de-116">String</span><span class="sxs-lookup"><span data-stu-id="8c4de-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8c4de-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c4de-117">JSON representation</span></span>

<span data-ttu-id="8c4de-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c4de-118">The following is a JSON representation of the resource.</span></span>

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
