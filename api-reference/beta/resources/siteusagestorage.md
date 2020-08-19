---
title: tipo de recurso siteUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 36ca6cc16ec4eeaf399bb8bd49db51c43a9dd8be
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807910"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="9df41-103">tipo de recurso siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="9df41-103">siteUsageStorage resource type</span></span>

<span data-ttu-id="9df41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9df41-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="9df41-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9df41-105">Properties</span></span>

| <span data-ttu-id="9df41-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9df41-106">Property</span></span>           | <span data-ttu-id="9df41-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9df41-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="9df41-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9df41-108">reportRefreshDate</span></span>  | <span data-ttu-id="9df41-109">Data</span><span class="sxs-lookup"><span data-stu-id="9df41-109">Date</span></span>   |
| <span data-ttu-id="9df41-110">sitetype</span><span class="sxs-lookup"><span data-stu-id="9df41-110">siteType</span></span>           | <span data-ttu-id="9df41-111">String</span><span class="sxs-lookup"><span data-stu-id="9df41-111">String</span></span> |
| <span data-ttu-id="9df41-112">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="9df41-112">storageUsedInBytes</span></span> | <span data-ttu-id="9df41-113">Int64</span><span class="sxs-lookup"><span data-stu-id="9df41-113">Int64</span></span>  |
| <span data-ttu-id="9df41-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="9df41-114">reportDate</span></span>         | <span data-ttu-id="9df41-115">Data</span><span class="sxs-lookup"><span data-stu-id="9df41-115">Date</span></span>   |
| <span data-ttu-id="9df41-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9df41-116">reportPeriod</span></span>       | <span data-ttu-id="9df41-117">String</span><span class="sxs-lookup"><span data-stu-id="9df41-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9df41-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9df41-118">JSON representation</span></span>

<span data-ttu-id="9df41-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9df41-119">The following is a JSON representation of the resource.</span></span>

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
