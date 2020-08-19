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
# <a name="workbookfiltercriteria-resource-type"></a>tipo de recurso workbookFilterCriteria

Namespace: microsoft.graph

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
