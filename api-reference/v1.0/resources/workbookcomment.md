---
title: tipo de recurso workbookComment
description: Definição do tipo de recurso workbookComment
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8a81ac565e9dd65dfccfdef4eeb7eca86786eee4c225a8a1c91c4333e1c34573
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235230"
---
# <a name="workbookcomment-resource-type"></a>tipo de recurso workbookComment

Namespace: microsoft.graph

Representa um comentário na workbook.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar workbookComments](../api/workbook-list-comments.md) | [workbookComment](workbookComment.md) collection | Obter uma **coleção de objetos workbookComment.** |
| [Obter workbookComment](../api/workbookcomment-get.md) | [workbookComment](workbookcomment.md) | Leia as propriedades e as relações de um **objeto workbookComment.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|content|Cadeia de caracteres|O conteúdo do comentário.|
|contentType|String|Indica o tipo do comentário.|
|id|String| Representa o identificador de comentário. Somente leitura.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|respostas|[workbookCommentReply](workbookcommentreply.md) collection| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
  "keyProperty": "id"
}-->

```json
{
  "content": "String",
  "contentType": "String",
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookComment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

