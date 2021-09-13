---
author: daspek
title: Tipo de recurso commentAction
description: O objeto commentAction fornece informações sobre um comentário que foi feito em um item.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: fd9d33c0b65654603e4d2d9393bb3ea71f636c37
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062779"
---
# <a name="commentaction-resource-type"></a>Tipo de recurso commentAction

Namespace: microsoft.graph

O **recurso commentAction** fornece informações sobre uma atividade [de comentário][] feita em um item.

>**Observação:** No momento, os registros de atividade do item estão disponíveis apenas SharePoint e OneDrive for Business.

[atividade]: itemactivity.md

## <a name="properties"></a>Propriedades

| Nome da propriedade    | Tipo                       | Descrição
|:-----------------|:---------------------------|:-----------------------------
| isReply          | booliano                    | Se for verdadeiro, essa atividade era uma resposta para um thread de comentário existente.
| parentAuthor     | [identitySet][]            | A identidade do usuário que iniciou o thread de comentários.
| participantes     | Coleção [identitySet][] | As identidades dos usuários que participam deste thread de comentário.

[identitySet]: identityset.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.commentAction"
}-->

```json
{
  "isReply": false,
  "parentAuthor": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```
<!--
{
  "type": "#page.annotation",
  "description": "The commentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/commentAction",
  "suppressions": []
}
-->

