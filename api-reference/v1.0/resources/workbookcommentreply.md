---
title: tipo de recurso workbookCommentReply
description: Definição do tipo de recurso workbookCommentReply
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 77402ad1566bcfa6822a326270306f1ea604896f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446727"
---
# <a name="workbookcommentreply-resource-type"></a>tipo de recurso workbookCommentReply

Namespace: Microsoft. Graph

Representa uma resposta a um comentário do Excel.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar workbookCommentReplies](../api/workbookcomment-list-replies.md) | coleção [workbookCommentReply](workbookcommentreply.md) | Recupere uma lista de objetos workbookcommentreply. |
| [Obter workbookCommentReply](../api/workbookcommentreply-get.md) | [workbookCommentReply](workbookcommentreply.md) | Leia as propriedades e os relacionamentos do objeto workbookCommentReply. |
| [Criar workbookCommentReply](../api/workbookcomment-post-replies.md) | [workbookCommentReply](workbookcommentreply.md) | Criar um novo workbookCommentReply. |
## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|content|Cadeia de caracteres|O conteúdo de uma resposta de comentário.|
|contentType|String|Indica o tipo da resposta de comentário.|
|id|Cadeia de caracteres|Representa o identificador de comentário. Somente leitura.|


## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookCommentReply",
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
  "description": "workbookCommentReply resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
