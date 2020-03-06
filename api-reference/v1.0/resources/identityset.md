---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
description: O recurso IdentitySet é uma coleção de chaves dos recursos identity.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0a5d53769dc023e79ac9f50db2c085647775cab0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531338"
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
| application | [Identidade](identity.md) | Opcional. O aplicativo associado a essa ação. |
| device      | [Identidade](identity.md) | Opcional. O dispositivo associado a essa ação.      |
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
