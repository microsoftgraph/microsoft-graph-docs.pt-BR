---
title: tipo de recurso workbookCommentReply
description: Definição do tipo de recurso workbookCommentReply
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9e71033e1665572e73dd672cd3a1e0e668b5f04ff1432f354fc27764055fa8ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54177769"
---
# <a name="workbookcommentreply-resource-type"></a>tipo de recurso workbookCommentReply

Namespace: microsoft.graph

Representa uma resposta a um Excel comentário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar workbookCommentReplies](../api/workbookcomment-list-replies.md) | [workbookCommentReply](workbookcommentreply.md) collection | Recupere uma lista de objetos workbookcommentreply. |
| [Obter workbookCommentReply](../api/workbookcommentreply-get.md) | [workbookCommentReply](workbookcommentreply.md) | Ler propriedades e relações do objeto workbookCommentReply. |
| [Criar workbookCommentReply](../api/workbookcomment-post-replies.md) | [workbookCommentReply](workbookcommentreply.md) | Crie uma nova workbookCommentReply. |
## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|content|Cadeia de caracteres|O conteúdo de uma resposta de comentário.|
|contentType|String|Indica o tipo para a resposta de comentário.|
|id|String|Representa o identificador de comentário. Somente leitura.|


## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookCommentReply",
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

