---
title: tipo de recurso oneNoteIdentitySet
description: '**Suporte em breve**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e149d5548ce3585bbcda1f0a199fa97d7543af77
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568876"
---
# <a name="onenoteidentityset-resource-type"></a>tipo de recurso oneNoteIdentitySet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Suporte em breve**

O tipo OneNoteIdentitySet é uma coleção com chave de objetos [OneNoteIdentity](onenoteidentity.md) .
É usado para representar um conjunto de identidades associadas a vários eventos para um _bloco de anotações_, uma _seção_ ou uma _página_, como _criado por_ ou _modificado pela última vez por_. 
 
Atualmente, ele contém uma única chave, _**User**_.  No futuro, chaves como o dispositivo ou aplicativo para alterar o item podem ser adicionadas.

No futuro, esse tipo será mesclado com [identityset](identityset.md)

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.onenoteIdentity"}
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|user|[oneNoteIdentity](onenoteidentity.md)|Um recurso OneNoteIdentity que representa um usuário.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
