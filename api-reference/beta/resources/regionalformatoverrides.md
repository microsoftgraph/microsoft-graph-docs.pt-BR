---
title: Tipo de recurso regionalFormatOverrides
description: Um recurso que representa substituições de formatação regional para calendários, datas e horários.
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 2b4046ad8ec6b2d646d1dc2d93cbe7bed205cbad
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516063"
---
# <a name="regionalformatoverrides-resource-type"></a>Tipo de recurso regionalFormatOverrides

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de cadeias de caracteres que representa substituições de formatação para calendários, datas e horários. 

## <a name="properties"></a>Propriedades

|Propriedade             |Tipo                     |Descrição                                                    |
|---------------------|-------------------------|---------------------------------------------------------------|
|calendar             |String                   |O calendário a ser usado, por exemplo, Calendário Gregoriano.<br><br>Retornado por padrão.|                   
|firstDayOfWeek       |microsoft.graph.dayOfWeek|O primeiro dia da semana a ser usado, por exemplo, domingo.<br><br>Retornado por padrão.|
|shortDateFormat      |String                   |O formato de tempo curto a ser usado para exibição de datas.<br><br>Retornado por padrão.|
|longDateFormat       |String                   |O formato de data longa a ser usado para exibição de datas.<br><br>Retornado por padrão.|
|shortTimeFormat      |String                   |O formato de tempo curto a ser usado para exibição de tempo.<br><br>Retornado por padrão.|
|longTimeFormat       |String                   |O formato de longo tempo a ser usado para exibição de tempo.<br><br>Retornado por padrão.|
|timeZone             |Cadeia de caracteres                   |O timezone a ser usado para exibição de tempo.<br><br>Retornado por padrão.|

## <a name="json-representation"></a>Representação JSON

A seguir está uma definição JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.regionalFormatOverrides"
}-->

```json
{
    "calendar": "string",
    "firstDayOfWeek": "string",
    "shortDateFormat": "string",
    "longDateFormat": "string",
    "shortTimeFormat": "string",
    "longTimeFormat": "string",
    "timeZone": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalFormatOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


