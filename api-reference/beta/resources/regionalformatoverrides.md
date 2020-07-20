---
title: tipo de recurso regionalFormatOverrides
description: Um recurso representando substituições regionais de formatação para calendários, datas e horas.
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: add353f539cac8eb6bb0bc7997c7aaaeea450835
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744199"
---
# <a name="regionalformatoverrides-resource-type"></a>tipo de recurso regionalFormatOverrides

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de cadeias de caracteres que representam substituições de formatação para calendários, datas e horas. 

## <a name="properties"></a>Propriedades

|Propriedade             |Tipo                 |Descrição                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|calendar             |String               |O calendário a ser usado, por exemplo, calendário gregoriano.<br><br>Retornado por padrão.|                   
|firstDayOfWeek       |String               |O primeiro dia da semana a ser usado, por exemplo, domingo.<br><br>Retornado por padrão.|
|shortDateFormat      |String               |O formato de data de curto prazo a ser usado para exibir datas.<br><br>Retornado por padrão.|
|longDateFormat       |String               |O formato de data e hora por extenso a ser usado para exibir datas.<br><br>Retornado por padrão.|
|shortTimeFormat      |String               |O formato de tempo curto a ser usado para exibir o tempo.<br><br>Retornado por padrão.|
|longTimeFormat       |String               |O formato de hora longa a ser usado para exibir o tempo.<br><br>Retornado por padrão.|
|timeZone             |Cadeia de caracteres               |O fuso horário a ser usado para exibir o tempo.<br><br>Retornado por padrão.|

## <a name="json-representation"></a>Representação JSON

A seguir está uma definição de JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "",
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
