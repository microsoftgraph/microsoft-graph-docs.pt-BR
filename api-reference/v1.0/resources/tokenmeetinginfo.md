---
title: tipo de recurso tokenMeetingInfo
description: O tipo tokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e34a10b9cd0fb09ff29c2d3373ad51a92109dcea
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865635"
---
# <a name="tokenmeetinginfo-resource-type"></a>tipo de recurso tokenMeetingInfo

Estas são as informações do token que permitem participar de uma reunião existente. Isso é obtido como parte da notificação de chamada de entrada. 

No caso de uma chamada ser desconectada, essas informações podem ajudá-lo a reingressar nessa chamada.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo    | Descrição                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| token                        | Cadeia de caracteres  | O token usado para ingressar na chamada.                                                 |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
    "token": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
