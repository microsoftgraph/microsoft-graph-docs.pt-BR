---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: ba72b813e0c68c3942a63b111e75298d7da3d68b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512693"
---
# <a name="thumbnailset-resource-type"></a>Tipo de recurso ThumbnailSet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **ThumbnailSet** é uma coleção com chave dos recursos [thumbnail](thumbnail.md). Ele é usado para representar um conjunto de miniaturas associado a um DriveItem.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                      | Descrição                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| id       | String                    | A id de dentro do item. Somente leitura.                                                |
| large    | [Thumbnail](thumbnail.md) | Uma miniatura em escala 1920 x 1920.                                                     |
| medium   | [Thumbnail](thumbnail.md) | Uma miniatura em escala 176 x 176.                                                       |
| small    | [Thumbnail](thumbnail.md) | Uma miniatura cortada em 48 x 48.                                                        |
| source   | [Thumbnail](thumbnail.md) | Uma imagem em miniatura personalizada ou a imagem original usada para gerar outras miniaturas. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/thumbnailset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
