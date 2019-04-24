---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
ms.openlocfilehash: d11f9eead6faf885bee579c634267e038f8a8ee4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522220"
---
# <a name="thumbnail-resource-type"></a>Tipo de recurso thumbnail

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
