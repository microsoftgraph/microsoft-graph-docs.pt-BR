---
author: JeremyKelley
description: O recurso identityset é uma coleção com chave de recursos de identidade.
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c43981c1f7e79567afe901217030a0b5abed6f53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006287"
---
# <a name="identityset-resource-type"></a>tipo de recurso identityset

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **** recurso identityset é uma coleção com chave de recursos de [identidade](identity.md) .

É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "conversation",
    "conversationIdentityType",
    "device",
    "encrypted",
    "guest",
    "phone",
    "user"
  ],
  "openType": true
} -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "microsoft.graph.identity"},
  "conversation": {"@odata.type": "microsoft.graph.identity"},
  "conversationIdentityType": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "encrypted": {"@odata.type": "microsoft.graph.identity"},
  "guest": {"@odata.type": "microsoft.graph.identity"},
  "phone": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo                    | Descrição                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| application | [Identidade](identity.md) | Opcional. O aplicativo associado a essa ação.  |
| conversation| [Identity](identity.md) | Opcional. A equipe ou canal associado a esta ação.       |
| conversationIdentityType| [Identity](identity.md) | Opcional. Indica se a propriedade de **conversa** identifica uma equipe ou um canal.|
| device      | [Identidade](identity.md) | Opcional. O dispositivo associado a essa ação.       |
| phone       | [identity](identity.md) | Opcional. O número de telefone associado a esta ação. |
| user        | [Identity](identity.md) | Opcional. O usuário associado a essa ação.         |

## <a name="remarks"></a>Comentários 

Confira [chamada](call.md) para uso **** de recursos identityset.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
