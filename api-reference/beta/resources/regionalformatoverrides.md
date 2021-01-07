---
title: tipo de recurso regionalFormatOverrides
description: Um recurso representando substituições regionais de formatação para calendários, datas e horas.
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 437b67f6a99017bb20096dbd20451b7662145cbd
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777593"
---
# <a name="regionalformatoverrides-resource-type"></a>tipo de recurso regionalFormatOverrides

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de cadeias de caracteres que representam substituições de formatação para calendários, datas e horas. 

## <a name="properties"></a>Propriedades

|Propriedade             |Tipo                 |Descrição                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|calendar             |Cadeia de caracteres               |O calendário a ser usado, por exemplo, calendário gregoriano.<br><br>Retornado por padrão.|                   
|firstDayOfWeek       |String               |O primeiro dia da semana a ser usado, por exemplo, domingo.<br><br>Retornado por padrão.|
|shortDateFormat      |Cadeia de caracteres               |O formato de data de curto prazo a ser usado para exibir datas.<br><br>Retornado por padrão.|
|longDateFormat       |Cadeia de caracteres               |O formato de data e hora por extenso a ser usado para exibir datas.<br><br>Retornado por padrão.|
|shortTimeFormat      |Cadeia de caracteres               |O formato de tempo curto a ser usado para exibir o tempo.<br><br>Retornado por padrão.|
|longTimeFormat       |Cadeia de caracteres               |O formato de hora longa a ser usado para exibir o tempo.<br><br>Retornado por padrão.|
|timeZone             |Cadeia de caracteres               |O fuso horário a ser usado para exibir o tempo.<br><br>Retornado por padrão.|

## <a name="json-representation"></a>Representação JSON

A seguir está uma definição de JSON do recurso.

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


