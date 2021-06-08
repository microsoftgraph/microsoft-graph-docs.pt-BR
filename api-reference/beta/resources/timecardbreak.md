---
title: Tipo de recurso timeCardBreak
description: Representa uma quebra de cartão de ponto específica.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 509667ec1fad41f956ee5ee6d6a4371b8d17fc2e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786360"
---
# <a name="timecardbreak-resource-type"></a>Tipo de recurso timeCardBreak

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma quebra de cartão de ponto [específica.](timecard.md)

## <a name="properties"></a>Propriedades
|Propriedade               |Tipo           |Descrição                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| breakId                   |`Edm.string`  |ID do **timeCardBreak**.|
| iniciar                 |[timeCardEvent](timecardevent.md)    | O evento de início do **timeCardBreak**.|
| end                   |[timeCardEvent](timecardevent.md)    | O evento de início do **timeCardBreak**.|
| notes                 |[itemBody](itembody.md)  | Observações sobre **o timeCardBreak**.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardBreak"
}-->
```json
{
    "breakId":"string",
    "notes":{
        "content": "string",
        "contentType": "string"
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
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardBreak resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
