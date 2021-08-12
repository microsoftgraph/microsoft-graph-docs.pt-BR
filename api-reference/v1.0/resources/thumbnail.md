---
author: JeremyKelley
ms.date: 09/10/2017
title: Miniatura
localization_priority: Normal
description: O tipo de recurso thumbnail representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 66656ed7a286290691182b79cce079110fb602c1157a9eb064ac92c88c5b1cec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163639"
---
# <a name="thumbnail-resource-type"></a>Tipo de recurso thumbnail

Namespace: microsoft.graph

O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.

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
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,
  "content": "stream"
}
```

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição
| :----------- | :----- | :----------------------------------------------------
| height       | Int32  | A altura da miniatura em pixels.
| sourceItemId | String | O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta.
| url          | Cadeia de caracteres | A URL usada para buscar o conteúdo da miniatura.
| width        | Int32  | A largura da miniatura em pixels.
| conteúdo      | Fluxo | O fluxo de conteúdo da miniatura.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->

