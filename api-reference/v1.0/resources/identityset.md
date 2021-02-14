---
author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
description: O recurso IdentitySet é uma coleção de chaves dos recursos identity.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e6f7aef915596e39173f286a3433e0114656e707
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239958"
---
# <a name="identityset-resource-type"></a>Tipo de recurso IdentitySet

Namespace: microsoft.graph

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
| device      | [Identity](identity.md) | Opcional. O dispositivo associado a essa ação.      |
| user        | [Identity](identity.md) | Opcional. O usuário associado a essa ação.        |

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

