---
title: Tipo de recurso timeCardEntry
description: Representa uma entrada de cartão de ponto específica.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d09b324b4d43765f05de789129021e2eb1f24789
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786369"
---
# <a name="timecardentry-resource-type"></a>Tipo de recurso timeCardEntry

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma entrada de cartão de ponto [específica.](timecard.md)

## <a name="properties"></a>Propriedades
|Propriedade               |Tipo           |Descrição                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| clockInEvent       |[timeCardEvent](timecardevent.md)    | O evento de clock-in do **timeCard**.|
| clockOutEvent                 |[timeCardEvent](timecardevent.md)  |O evento de saída do **timeCard**. |
| quebras    |[Coleção timeCardBreak](timecardbreak.md)    |A lista de quebras associada ao **timeCard**.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEntry"
}-->
```json
{
   "clockInEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "clockOutEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "breaks":[
      {
         "breakId":"string",
         "notes":{
             "content": "string",
             "contentType": "text"
          },
         "start":{
            "dateTime":"String (timestamp)",
            "atApprovedLocation":true,
            "notes":{
                 "content": "string",
                 "contentType": "text"
            },
         },
         "end":null
      }
   ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timecardentry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
