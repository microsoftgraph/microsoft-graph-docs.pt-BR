---
title: tipo de recurso workbookFilterCriteria
description: Representa os critérios de filtragem aplicados a uma coluna.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: d63e42f8efee5652edb48604e5d1831e436a4e01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519222"
---
# <a name="workbookfiltercriteria-resource-type"></a><span data-ttu-id="a0d18-103">tipo de recurso workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="a0d18-103">workbookFilterCriteria resource type</span></span>

<span data-ttu-id="a0d18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0d18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0d18-105">Representa os critérios de filtragem aplicados a uma coluna.</span><span class="sxs-lookup"><span data-stu-id="a0d18-105">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0d18-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0d18-106">JSON representation</span></span>

<span data-ttu-id="a0d18-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0d18-107">Here is a JSON representation of the resource.</span></span>

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
