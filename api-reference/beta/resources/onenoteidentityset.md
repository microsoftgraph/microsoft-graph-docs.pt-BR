---
title: tipo de recurso oneNoteIdentitySet
description: '**Suporte em breve**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: c0d2f0b4ed65ac83a59036c362136b7af772d21c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290578"
---
# <a name="onenoteidentityset-resource-type"></a>tipo de recurso oneNoteIdentitySet

Namespace: microsoft.graph

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
|user|[onenoteIdentity](onenoteidentity.md)|Um recurso OneNoteIdentity que representa um usuário.|

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
