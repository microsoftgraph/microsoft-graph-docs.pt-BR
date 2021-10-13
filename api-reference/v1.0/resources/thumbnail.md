---
author: JeremyKelley
ms.date: 09/10/2017
title: Miniatura
ms.localizationpriority: medium
description: O tipo de recurso thumbnail representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eecd879dd91bf165f1b5374cb813c2ce4210bd19
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2021
ms.locfileid: "60288324"
---
# <a name="thumbnail-resource-type"></a>Tipo de recurso thumbnail

Namespace: microsoft.graph

O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição|
| :----------- | :----- | :----------------------------------------------------|
| height       | Int32  | A altura da miniatura em pixels.|
| sourceItemId | String | O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta.|
| url          | Cadeia de caracteres | A URL usada para buscar o conteúdo da miniatura.|
| width        | Int32  | A largura da miniatura em pixels.|
| conteúdo      | Fluxo | O fluxo de conteúdo da miniatura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **thumbnail**.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "content",
    "height",
    "width",
    "sourceItemId"
  ],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": "Int32",
  "sourceItemId": "String",
  "url": "String",
  "width": "Int32",
  "content": "Stream"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->

