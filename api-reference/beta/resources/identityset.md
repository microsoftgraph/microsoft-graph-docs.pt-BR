---
author: JeremyKelley
description: O recurso identitySet é uma coleção chave de recursos de identidade.
title: IdentitySet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
ms.openlocfilehash: 50f6b45c3121f770019d9b5be7e0492242711e1c
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453713"
---
# <a name="identityset-resource-type"></a>Tipo de recurso identitySet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso identitySet** é uma coleção chave de [recursos de](identity.md) identidade.

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
| application | [Identity](identity.md) | Opcional. O aplicativo associado a essa ação.  |
| conversa| [Identity](identity.md) | Opcional. A equipe ou canal associado a essa ação.       |
| conversationIdentityType| [Identity](identity.md) | Opcional. Indica se a **propriedade conversation** identifica uma equipe ou canal.|
| device      | [Identity](identity.md) | Opcional. O dispositivo associado a essa ação.       |
| phone       | [identity](identity.md) | Opcional. O número de telefone associado a essa ação. |
| user        | [Identity](identity.md) | Opcional. O usuário associado a essa ação.         |

## <a name="remarks"></a>Comentários 

Consulte [Call](call.md) for usage of **identitySet** resources.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->


