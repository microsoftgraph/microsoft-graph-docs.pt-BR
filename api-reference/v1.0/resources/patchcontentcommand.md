---
title: Tipo de recurso patchContentCommand
description: As alterações feitas em uma página OneNote em uma solicitação PATCH.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0b34271f08cc8f8e234c6a10ecd28229ddbce451ca0f54b26197bc1a9d02f56f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205250"
---
# <a name="patchcontentcommand-resource-type"></a>Tipo de recurso patchContentCommand

Namespace: microsoft.graph

As alterações feitas em uma página OneNote em uma solicitação PATCH.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON do recurso, que é enviada no corpo da solicitação [páginas PATCH/{id}'.](../api/page-update.md)

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
|ação|onenotePatchActionType|A ação a ser executada no elemento de destino. Os valores possíveis são: `replace` , , , , ou `append` `delete` `insert` `prepend` .|
|content|Cadeia de caracteres|Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo. Se o conteúdo contiver dados binários, a solicitação deverá ser enviada usando o tipo `multipart/form-data` de conteúdo com uma parte "Comandos". |
|position|onenotePatchInsertPosition|O local para adicionar o conteúdo fornecido em relação ao elemento de destino. Os valores possíveis são: `after` (padrão) ou `before` .|
|destino|Cadeia de caracteres|O elemento a ser atualizado. Deve ser `#<data-id>` o ou o gerado do `<id>` elemento, ou a `body` `title` palavra-chave ou.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

