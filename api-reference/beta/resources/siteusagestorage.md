---
title: tipo de recurso siteUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 1ed15d4efb1c9a0fa81fdd79faeb9542d8093aab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008226"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="30e6a-103">tipo de recurso siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="30e6a-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="30e6a-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30e6a-104">Properties</span></span>

| <span data-ttu-id="30e6a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30e6a-105">Property</span></span>           | <span data-ttu-id="30e6a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="30e6a-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="30e6a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="30e6a-107">reportRefreshDate</span></span>  | <span data-ttu-id="30e6a-108">Data</span><span class="sxs-lookup"><span data-stu-id="30e6a-108">Date</span></span>   |
| <span data-ttu-id="30e6a-109">sitetype</span><span class="sxs-lookup"><span data-stu-id="30e6a-109">siteType</span></span>           | <span data-ttu-id="30e6a-110">String</span><span class="sxs-lookup"><span data-stu-id="30e6a-110">String</span></span> |
| <span data-ttu-id="30e6a-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="30e6a-111">storageUsedInBytes</span></span> | <span data-ttu-id="30e6a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="30e6a-112">Int64</span></span>  |
| <span data-ttu-id="30e6a-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="30e6a-113">reportDate</span></span>         | <span data-ttu-id="30e6a-114">Data</span><span class="sxs-lookup"><span data-stu-id="30e6a-114">Date</span></span>   |
| <span data-ttu-id="30e6a-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="30e6a-115">reportPeriod</span></span>       | <span data-ttu-id="30e6a-116">String</span><span class="sxs-lookup"><span data-stu-id="30e6a-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="30e6a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30e6a-117">JSON representation</span></span>

<span data-ttu-id="30e6a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="30e6a-118">The following is a JSON representation of the resource.</span></span>

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
