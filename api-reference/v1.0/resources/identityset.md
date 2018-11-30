---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
ms.openlocfilehash: ea49f904197b2f4a661b781576f06240e41cf808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006988"
---
# <a name="identityset-resource-type"></a>Tipo de recurso IdentitySet

O recurso **IdentitySet** é uma coleção de chaves dos recursos [identity](identity.md). É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identitySet",
       "optionalProperties": ["user", "application", "device"],
       "openType": true } -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo                    | Descrição                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| application | [Identity](identity.md) | Opcional. O aplicativo associado a essa ação. |
| dispositivo      | [Identity](identity.md) | Opcional. O dispositivo associado a essa ação.      |
| Usuário        | [Identity](identity.md) | Opcional. O usuário associado a essa ação.        |

## <a name="remarks"></a>Comentários 

Consulte [DriveItem](driveitem.md) para saber mais sobre o uso de recursos **IdentitySet**.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
