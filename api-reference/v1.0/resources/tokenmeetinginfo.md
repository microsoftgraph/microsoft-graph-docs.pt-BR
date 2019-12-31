---
title: tipo de recurso tokenMeetingInfo
description: O tipo tokenMeetingInfo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 05cc4c21fe3a8ea0d4b27b6c27b737ec6fe317d2
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912969"
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
