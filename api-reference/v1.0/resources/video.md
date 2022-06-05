---
author: JeremyKelley
title: tipo de recurso de vídeo
ms.localizationpriority: medium
description: O recurso de vídeo agrupa itens de dados relacionados a vídeo em uma única estrutura.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 81a2ccd6250261c87b5af84cc0bef0ace4342702
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65897822"
---
# <a name="video-resource-type"></a>tipo de recurso de vídeo

Namespace: microsoft.graph

O **recurso** de vídeo agrupa itens de dados relacionados a vídeo em uma única estrutura.

Se um [**driveItem**](driveitem.md) tiver uma faceta de vídeo **não nula** , o item representará um arquivo de vídeo.
As propriedades do recurso **de** vídeo são preenchidas extraindo metadados do arquivo.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.video"
}-->

```json
{
  "audioBitsPerSample": 16,
  "audioChannels": 1,
  "audioFormat": "AAC",
  "audioSamplesPerSecond": 44100,
  "bitrate": 39101896,
  "duration": 8053,
  "fourCC": "H264",
  "frameRate": 239.877,
  "height": 1280,
  "width": 720
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade             | Tipo   | Descrição
|:--------------------------|:-------|:----------------------------------------
| **audioBitsPerSample**    | Int32  | Número de bits áudio por amostra.
| **audioChannels**         | Int32  | Número de canais de áudio.
| **audioFormat**           | string | Nome do formato áudio (AAC, MP3, etc.).
| **audioSamplesPerSecond** | Int32  | Número de amostras de áudio por segundo.
| **bitrate**               | Int32  | Taxa de bits do vídeo em bits por segundo.
| **duration**              | Int64  | Duração do arquivo em milissegundos.
| **fourCC**                | string | Nome do formato de vídeo "Código de quatro caracteres".
| **Framerate**             | double | Taxa de quadros do vídeo.
| **height**                | Int32  | A altura do vídeo em pixels.
| **width**                 | Int32  | A largura do vídeo em pixels.

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Comentários

Para obter mais informações sobre as facetas em um driveItem, consulte [driveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->

