---
author: JeremyKelley
description: O tipo de recurso thumbnail representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.
ms.date: 09/10/2017
title: Thumbnail
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 53001d2459af4dc382501e33930bc8aca55a26b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519761"
---
# <a name="thumbnail-resource-type"></a>Tipo de recurso thumbnail

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **thumbnail**.

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| height       | Int32  | A altura da miniatura em pixels.                                                                                     |
| sourceItemId | String | O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta. |
| url          | Cadeia de caracteres | A URL usada para buscar o conteúdo da miniatura.                                                                                |
| width        | Int32  | A largura da miniatura em pixels.                                                                                      |
| conteúdo | Fluxo | O fluxo de conteúdo da miniatura. |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail",
  "suppressions": []
}
-->
