---
author: daspek
ms.author: dspektor
title: tipo de recurso commentaction
description: O objeto commentaction fornece informações sobre um comentário que foi feito em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f3720d84624fa728a168515beb28422ab355b335
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531802"
---
# <a name="commentaction-resource-type"></a>tipo de recurso commentaction

Namespace: microsoft.graph

O recurso **commentaction** fornece informações sobre uma [atividade][] de comentário feita em um item.

>**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

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
