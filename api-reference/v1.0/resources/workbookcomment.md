---
title: tipo de recurso workbookComment
description: Definição do tipo de recurso workbookComment
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b89f7b1ed2ca1ca833d8d5bae72d74a58b714997
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015166"
---
# <a name="workbookcomment-resource-type"></a>tipo de recurso workbookComment

Namespace: microsoft.graph

Representa um comentário na pasta de trabalho.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar workbookComments](../api/workbook-list-comments.md) | coleção [workbookComment](workbookComment.md) | Obtenha uma coleção de objetos **workbookComment** . |
| [Obter workbookComment](../api/workbookcomment-get.md) | [workbookComment](workbookcomment.md) | Leia as propriedades e os relacionamentos de um objeto **workbookComment** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|content|Cadeia de caracteres|O conteúdo de comment.|
|contentType|String|Indica o tipo do comentário.|
|id|String| Representa o identificador de comentário. Somente leitura.|

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

