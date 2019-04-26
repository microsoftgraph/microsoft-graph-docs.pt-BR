---
title: Tipo de recurso timeZoneBase
description: A representação básica de um fuso horário.
localization_priority: Normal
ms.openlocfilehash: 8d968b8177da942c1b8940618c8ba965c362c914
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341866"
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
