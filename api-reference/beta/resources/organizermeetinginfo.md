---
title: tipo de recurso organizerMeetingInfo
description: Informações de reunião que contêm o organizador da reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 129e8a60edd89d45eb6e48715a59231475d52b99
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341754"
---
# <a name="organizermeetinginfo-resource-type"></a>tipo de recurso organizerMeetingInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações de reunião que contêm o organizador da reunião.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                          | Descrição                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| allowConversationWithoutHost | Boolean                       | Indica se uma conversa pode continuar assim que o host da conversa sair. |
| organizer                    | [identitySet](identityset.md) | A identidade do Azure Active Directory do organizador.  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.meetingInfo",
   "openType": true,
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "microsoft.graph.identitySet" }
}
```

## <a name="example"></a>Exemplo

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": {
    "user": {
      "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
      "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
