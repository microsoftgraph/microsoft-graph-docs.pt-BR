---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Miniatura
localization_priority: Normal
ms.openlocfilehash: 05fcb6ec4b0821a4243692aab9c15419eb2f630d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529751"
---
# <a name="thumbnail-resource-type"></a>Tipo de recurso thumbnail

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

## <a name="relationships"></a>Relacionamentos

| Nome    | Tipo   | Descrição                           |
| :------ | :----- | :------------------------------------ |
| content | Fluxo | O fluxo de conteúdo da miniatura. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail",
  "suppressions": [
    "Error: /api-reference/beta/resources/thumbnail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
