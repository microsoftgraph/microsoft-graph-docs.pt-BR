---
title: tipo de recurso tokenMeetingInfo
description: O tipo tokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0df9a7a66420f20ff62677f54e617d64e9db0273
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007540"
---
# <a name="tokenmeetinginfo-resource-type"></a>tipo de recurso tokenMeetingInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo tokenMeetingInfo.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo    | Descrição                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| allowConversationWithoutHost | Booliano | Indica se uma conversa pode continuar assim que o host da conversa sair. |
| token                        | Cadeia de caracteres  | O token para ingressar/ativar a reunião.                                        |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType": "microsoft.graph.meetingInfo",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a>Exemplo

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
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
