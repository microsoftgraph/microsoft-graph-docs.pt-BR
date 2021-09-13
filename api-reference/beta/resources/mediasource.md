---
author: MarcMroz
description: O recurso mediaSource contém metadados sobre a origem do item de unidade de mídia (áudio ou vídeo).
title: Tipo de recurso mediaSource
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: fac36dbd1112289e289b6f74ce16e5a971076e60
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59124109"
---
# <a name="mediasource-resouce-type"></a>tipo de resouce mediaSource

O **recurso mediaSource** contém metadados sobre a origem do item de unidade de mídia (áudio ou vídeo).

Ele está disponível na propriedade de mídia dos [recursos driveItem.][item-resource]

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo                       | Descrição                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| **contentCategory**      | mediaSourceContentCategory | Valor de enumeração que indica a categoria de conteúdo de mídia.                                     |

### <a name="mediasourcecontentcategory-values"></a>valores mediaSourceContentCategory

| Valor               | Descrição                                         |
|:------------------- |:----------------------------------------------------|
| meeting             | A mídia é uma reunião.                             |
| liveStream          | A mídia é uma transmissão ao vivo.                         |
| presentation        | A mídia é uma apresentação.                        |
| screenRecording     | A mídia é uma gravação de tela.                    |
| unknownFutureValue  | Valor do marcador para compatibilidade futura.              |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentCategory"
  ],
  "@odata.type": "microsoft.graph.mediaSource"
}-->

```json
{
  "contentCategory" : "string"
}
```

## <a name="see-also"></a>Confira também

Para obter mais informações sobre as facetas em um driveItem, [consulte driveItem](driveitem.md).

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The mediaSource facet provides information about drive item source.",
  "keywords": "mediaSource,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/MediaSource"
} -->
