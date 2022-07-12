---
author: JeremyKelley
description: O tipo de recurso thumbnail representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.
ms.date: 09/10/2017
title: Miniatura
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 0833ed2e8b5957cd4faa3f5442c5770b93a3c5b8
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732188"
---
# <a name="thumbnail-resource-type"></a>Tipo de recurso thumbnail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| height       | Int32  | A altura da miniatura em pixels.                                                                                     |
| sourceItemId | String | O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta. |
| url          | Cadeia de caracteres | A URL usada para buscar o conteúdo da miniatura.                                                                                |
| width        | Int32  | A largura da miniatura em pixels.                                                                                      |
| conteúdo | Fluxo | O fluxo de conteúdo da miniatura. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **thumbnail**.

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": "Int32",
  "sourceItemId": "String",
  "url": "String",
  "width": "Int32",

  /* relationships */
  "content": "Stream"
}
```


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


