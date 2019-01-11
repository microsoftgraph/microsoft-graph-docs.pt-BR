---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Vídeo
localization_priority: Normal
ms.openlocfilehash: 0e26804991128363780ed4336849486c92fc5a07
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889254"
---
# <a name="video-resource-type"></a>Tipo de recurso Video

O recurso **Video** agrupa itens de dados relacionados a vídeos em uma única estrutura.

Se um [**DriveItem**](driveitem.md) tiver uma faceta **video** não nula, o item representa um vídeo. As propriedades do recurso **Video** são preenchidas extraindo-se os metadados do arquivo.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

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
| **taxa de quadros**             | double | Taxa de quadros do vídeo.
| **height**                | Int32  | A altura do vídeo em pixels.
| **width**                 | Int32  | A largura do vídeo em pixels.

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
