---
title: tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4cfa6fe84c18d4895e5d709d3ab6254258c1b970
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422279"
---
# <a name="patchcontentcommand-resource-type"></a>tipo de recurso patchContentCommand

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|ação|String|A ação a ser executada no elemento de destino. Os valores possíveis são: `replace`, `append`, `delete`, `insert` ou `prepend`.|
|content|Cadeia de caracteres|Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo. Se o conteúdo contiver dados binários, a solicitação deverá ser enviada `multipart/form-data` usando o tipo de conteúdo com uma parte "Commands". |
|position|String|O local para adicionar o conteúdo fornecido em relação ao elemento de destino. Os valores possíveis são `after` : (padrão) `before`ou.|
|destino|String|O elemento a ser atualizado. Deve ser o `#<data-id>` ou o gerado `{id}` do elemento, ou a `body` palavra- `title` chave ou.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
