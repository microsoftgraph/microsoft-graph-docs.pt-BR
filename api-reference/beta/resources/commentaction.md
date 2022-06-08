---
author: daspek
description: O recurso CommentAction fornece informações sobre uma atividade de comentário feitas em um item.
ms.date: 09/14/2017
title: CommentAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 984e9777c31fb1ce6b6b748b9ffb0cdfe9b6446a
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944140"
---
# <a name="commentaction-resource-type"></a>Tipo de recurso CommentAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **CommentAction** fornece informações sobre uma [atividade][] de comentário feitas em um item.

[atividade]: itemactivity.md

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

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                       | Descrição                                                       |
| :----------- | :------------------------- | :---------------------------------------------------------------- |
| isReply      | booliano                    | Se for verdadeiro, essa atividade era uma resposta para um thread de comentário existente. |
| parentAuthor | [identitySet][]            | A identidade do usuário que iniciou o thread de comentários.          |
| participantes | Coleção [identitySet][] | As identidades dos usuários que participam deste thread de comentário. |

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
