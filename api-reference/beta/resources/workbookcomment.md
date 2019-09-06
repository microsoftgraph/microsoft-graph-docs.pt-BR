---
title: tipo de recurso workbookComment
description: Representa um comentário na pasta de trabalho.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a7a3427512962bd38c90faa710c501380e353f22
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775892"
---
# <a name="workbookcomment-resource-type"></a>tipo de recurso workbookComment

Representa um comentário na pasta de trabalho.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar workbookComments](../api/workbook-list-comments.md) | coleção [workbookComment](workbookComment.md) | Obtenha uma coleção de objetos **workbookComment** . |
| [Obter workbookComment](../api/workbookcomment-get.md) | [workbookComment](workbookcomment.md) | Leia as propriedades e os relacionamentos de um objeto **workbookComment** . |


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|content|Cadeia de caracteres|O conteúdo do comentário.|
|contentType|String|Indica o tipo do comentário.|
|id|Cadeia de caracteres| Representa o identificador de comentário. Somente leitura.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Enviar|coleção [workbookCommentReply](workbookcommentreply.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
  "baseType": "",
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
