---
title: tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3c8aab8770304f8616025d0d5ac2e70ad41a1340
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534075"
---
# <a name="patchcontentcommand-resource-type"></a>tipo de recurso patchContentCommand

Namespace: microsoft.graph

As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [patch Pages/{ID}](../api/page-update.md) . 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|ação|onenotePatchActionType|A ação a ser executada no elemento de destino. Os valores possíveis são: `replace`, `append`, `delete`, `insert`, ou `prepend`.|
|content|Cadeia de caracteres|Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo. Se o conteúdo contiver dados binários, a solicitação deverá ser enviada `multipart/form-data` usando o tipo de conteúdo com uma parte "Commands". |
|position|onenotePatchInsertPosition|O local para adicionar o conteúdo fornecido em relação ao elemento de destino. Os valores possíveis são: `after` (padrão) ou `before`.|
|destino|String|O elemento a ser atualizado. Deve ser o `#<data-id>` ou o gerado `<id>` do elemento, ou a `body` palavra- `title` chave ou.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
