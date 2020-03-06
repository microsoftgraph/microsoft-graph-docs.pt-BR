---
title: tipo de recurso tokenMeetingInfo
description: O tipo tokenMeetingInfo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 786b3d1429d2f081207fa2d81b5f178d3cb5e08d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533445"
---
# <a name="tokenmeetinginfo-resource-type"></a>tipo de recurso tokenMeetingInfo

Namespace: microsoft.graph

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
