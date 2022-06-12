---
title: Tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma OneNote em uma solicitação PATCH.
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: notes
doc_type: resourcePageType
ms.openlocfilehash: b5432bf68cfc4acdc42db0c502555469ca025d71
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034681"
---
# <a name="patchcontentcommand-resource-type"></a>Tipo de recurso patchContentCommand

Namespace: microsoft.graph

As alterações a serem feitas em uma OneNote em uma solicitação PATCH.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON do recurso, que é enviada no corpo da solicitação [de páginas PATCH/{id}](../api/page-update.md) '.

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
|ação|onenotePatchActionType|A ação a ser executada no elemento de destino. Os valores possíveis são: `replace`, `append`, `delete`, `insert`ou `prepend`.|
|content|Cadeia de caracteres|Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo. Se o conteúdo contiver dados binários, a solicitação deverá ser enviada `multipart/form-data` usando o tipo de conteúdo com uma parte "Comandos". |
|position|onenotePatchInsertPosition|O local para adicionar o conteúdo fornecido em relação ao elemento de destino. Os valores possíveis são: `after` (padrão) ou `before`.|
|destino|Cadeia de caracteres|O elemento a ser atualizado. Deve ser o `#<data-id>` ou o gerado `<id>` do elemento, ou a palavra-chave `body` ou `title` .|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

