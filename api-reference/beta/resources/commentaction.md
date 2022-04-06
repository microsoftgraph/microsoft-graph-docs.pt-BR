---
author: daspek
description: O recurso CommentAction fornece informações sobre uma atividade de comentário feitas em um item.
ms.date: 09/14/2017
title: CommentAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 32532bf0771da739db86915091cdc8b79aa942c2
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722754"
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
