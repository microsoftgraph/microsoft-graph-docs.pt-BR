---
title: tipo de recurso de oneNoteIdentitySet
description: '**Suporte em breve**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e149d5548ce3585bbcda1f0a199fa97d7543af77
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516711"
---
# <a name="onenoteidentityset-resource-type"></a>tipo de recurso de oneNoteIdentitySet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Suporte em breve**

O tipo de OneNoteIdentitySet é uma coleção com chave de objetos [OneNoteIdentity](onenoteidentity.md) .
Ele é usado para representar um conjunto de identidades associado a vários eventos para um _Bloco de anotações_, _seção_ ou da _página_, como _criado por_ ou _modificado pela última vez_. 
 
Atualmente, ele contém um único _**usuário**_ de chave.  No futuro, chaves, como o dispositivo ou aplicativo para alterar o item podem ser adicionadas.

No futuro, esse tipo de será mesclado com [IdentitySet](identityset.md)

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|user|[oneNoteIdentity](onenoteidentity.md)|Um recurso de OneNoteIdentity que representa um usuário.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentityset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
