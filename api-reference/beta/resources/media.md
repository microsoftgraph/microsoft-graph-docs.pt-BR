---
author: MarcMroz
description: O recurso de mídia contém metadados sobre o item de unidade de mídia (áudio ou vídeo).
title: tipo de recurso de mídia
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 3dd985c7259088f41412ea5d579c1e49d99acf4c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091199"
---
# <a name="media-resouce-type"></a>tipo de resouce de mídia

Contém metadados sobre o item de unidade de mídia (áudio ou vídeo).

Ele está disponível na propriedade de mídia dos [recursos driveItem.][item-resource]


## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo                  | Descrição                                                                                                   |
| :----------------------- | :-------------------- | :------------------------------------------------------------------------------------------------------------ 
| **isTranscriptionShown** | Boleano               | Se um arquivo tiver uma transcrição, essa configuração controlará se as legendas/transcrição fechadas do arquivo de mídia devem ser mostradas para as pessoas durante a exibição. Leitura-Gravação.                                                    |
| **mediaSource**          | [mediaSource](mediaSource.md)         | Informações sobre a origem da mídia. Somente leitura.                                                             | 


## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.media"
}-->

```json
{
  "isTranscriptionShown" : true,
  "mediaSource": { "@odata.type": "microsoft.graph.mediaSource" }
}
```

## <a name="see-also"></a>Confira também 

Para obter mais informações sobre as facetas em um driveItem, [consulte driveItem](driveitem.md).

[item-resource]: ../resources/driveitem.md
[mediaSource]: mediaSource.md

<!-- {
  "type": "#page.annotation",
  "description": "The media resource type provides information about the media item.",
  "keywords": "mediaItem,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/Media"
} -->
