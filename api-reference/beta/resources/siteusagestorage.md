---
title: tipo de recurso siteUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 84b46861196e8893655fc5abc69ad1d4809cfd03
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033510"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="62589-103">tipo de recurso siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="62589-103">siteUsageStorage resource type</span></span>

<span data-ttu-id="62589-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62589-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="62589-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62589-105">Properties</span></span>

| <span data-ttu-id="62589-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62589-106">Property</span></span>           | <span data-ttu-id="62589-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="62589-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="62589-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="62589-108">reportRefreshDate</span></span>  | <span data-ttu-id="62589-109">Data</span><span class="sxs-lookup"><span data-stu-id="62589-109">Date</span></span>   |
| <span data-ttu-id="62589-110">sitetype</span><span class="sxs-lookup"><span data-stu-id="62589-110">siteType</span></span>           | <span data-ttu-id="62589-111">String</span><span class="sxs-lookup"><span data-stu-id="62589-111">String</span></span> |
| <span data-ttu-id="62589-112">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="62589-112">storageUsedInBytes</span></span> | <span data-ttu-id="62589-113">Int64</span><span class="sxs-lookup"><span data-stu-id="62589-113">Int64</span></span>  |
| <span data-ttu-id="62589-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="62589-114">reportDate</span></span>         | <span data-ttu-id="62589-115">Data</span><span class="sxs-lookup"><span data-stu-id="62589-115">Date</span></span>   |
| <span data-ttu-id="62589-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="62589-116">reportPeriod</span></span>       | <span data-ttu-id="62589-117">String</span><span class="sxs-lookup"><span data-stu-id="62589-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="62589-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62589-118">JSON representation</span></span>

<span data-ttu-id="62589-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62589-119">The following is a JSON representation of the resource.</span></span>

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


