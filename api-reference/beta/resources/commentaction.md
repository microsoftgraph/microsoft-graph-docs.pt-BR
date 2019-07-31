---
author: daspek
description: O recurso CommentAction fornece informações sobre uma atividade de comentário feitas em um item.
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b7782c6e4dd30b503a9be88737ef6bd2dbad109b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973255"
---
# <a name="commentaction-resource-type"></a>Tipo de recurso CommentAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **CommentAction** fornece informações sobre uma [atividade][] de comentário feitas em um item.

[atividade]: itemactivity.md

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

## <a name="properties"></a>Propriedades

| Nome da propriedade    | Tipo                       | Descrição
|:-----------------|:---------------------------|:-----------------------------
| isReply          | booliano                    | Se for verdadeiro, essa atividade era uma resposta para um thread de comentário existente.
| parentAuthor     | [identitySet][]            | A identidade do usuário que iniciou o thread de comentários.
| participantes     | Coleção [identitySet][] | As identidades dos usuários que participam deste thread de comentário.

[identitySet]: identityset.md

## <a name="remarks"></a>Comentários

Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": []
}
-->
