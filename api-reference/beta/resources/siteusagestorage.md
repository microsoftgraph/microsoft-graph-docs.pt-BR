---
title: tipo de recurso siteUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 33d78540a6dd5b3c15cb6d8fce80496be19f0711
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520517"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="6f440-103">tipo de recurso siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="6f440-103">siteUsageStorage resource type</span></span>

<span data-ttu-id="6f440-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6f440-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="6f440-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f440-105">Properties</span></span>

| <span data-ttu-id="6f440-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f440-106">Property</span></span>           | <span data-ttu-id="6f440-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f440-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="6f440-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6f440-108">reportRefreshDate</span></span>  | <span data-ttu-id="6f440-109">Data</span><span class="sxs-lookup"><span data-stu-id="6f440-109">Date</span></span>   |
| <span data-ttu-id="6f440-110">sitetype</span><span class="sxs-lookup"><span data-stu-id="6f440-110">siteType</span></span>           | <span data-ttu-id="6f440-111">String</span><span class="sxs-lookup"><span data-stu-id="6f440-111">String</span></span> |
| <span data-ttu-id="6f440-112">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="6f440-112">storageUsedInBytes</span></span> | <span data-ttu-id="6f440-113">Int64</span><span class="sxs-lookup"><span data-stu-id="6f440-113">Int64</span></span>  |
| <span data-ttu-id="6f440-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="6f440-114">reportDate</span></span>         | <span data-ttu-id="6f440-115">Data</span><span class="sxs-lookup"><span data-stu-id="6f440-115">Date</span></span>   |
| <span data-ttu-id="6f440-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6f440-116">reportPeriod</span></span>       | <span data-ttu-id="6f440-117">String</span><span class="sxs-lookup"><span data-stu-id="6f440-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f440-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f440-118">JSON representation</span></span>

<span data-ttu-id="6f440-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f440-119">The following is a JSON representation of the resource.</span></span>

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
