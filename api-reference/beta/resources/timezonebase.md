---
title: Tipo de recurso timeZoneBase
description: A representação básica de um fuso horário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a5ebe26cb7968e9a5cce3ab05821dfb81e1221ec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007561"
---
# <a name="timezonebase-resource-type"></a>Tipo de recurso timeZoneBase

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A representação básica de um fuso horário.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| name | string | O nome de um fuso horário. Pode ser o nome de um fuso horário padrão como "Hora Padrão do Havaí Aleuta" ou "Fuso Horário Personalizado" para um fuso horário personalizado. |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
