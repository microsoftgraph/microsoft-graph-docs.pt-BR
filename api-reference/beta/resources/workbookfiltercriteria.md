---
title: tipo de recurso workbookFilterCriteria
description: Representa os critérios de filtragem aplicados a uma coluna.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: 6bd7906d458cf3573fe0d7d3f61cc5c8684e1c03
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808484"
---
# <a name="workbookfiltercriteria-resource-type"></a><span data-ttu-id="04a9d-103">tipo de recurso workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="04a9d-103">workbookFilterCriteria resource type</span></span>

<span data-ttu-id="04a9d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04a9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04a9d-105">Representa os critérios de filtragem aplicados a uma coluna.</span><span class="sxs-lookup"><span data-stu-id="04a9d-105">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04a9d-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04a9d-106">JSON representation</span></span>

<span data-ttu-id="04a9d-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04a9d-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "values": {"@odata.type":"microsoft.graph.Json"},
  "icon":{"@odata.type": "microsoft.graph.workbookIcon"},
  "operator":"string"
}
```
