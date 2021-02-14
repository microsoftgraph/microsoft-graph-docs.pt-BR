---
author: daspek
title: Tipo de recurso commentAction
description: O objeto commentAction fornece informações sobre um comentário que foi feito em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f2f3ab7f0798ee1020b107c38262a912fdae53ef
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238411"
---
# <a name="commentaction-resource-type"></a>Tipo de recurso commentAction

Namespace: microsoft.graph

O **recurso commentAction** fornece informações sobre uma atividade [de comentário][] feita em um item.

>**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.

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
  "@type": "microsoft.graph.commentAction"
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

