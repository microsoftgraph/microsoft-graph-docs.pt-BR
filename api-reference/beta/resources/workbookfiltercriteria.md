---
title: tipo de recurso workbookFilterCriteria
description: Representa os critérios de filtragem aplicados a uma coluna.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: 6e0b2b09ab464c0a04bf97ed666f3fd3a687e912
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964014"
---
# <a name="workbookfiltercriteria-resource-type"></a>tipo de recurso workbookFilterCriteria

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os critérios de filtragem aplicados a uma coluna.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
