---
author: JeremyKelley
ms.date: 09/10/2017
title: Vídeo
localization_priority: Normal
description: O recurso Video agrupa itens de dados relacionados a vídeos em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: be2c9c87be0bb7d36b5af6f1feb6dc1c8a16365d1fe062b40e65b10e026e6884
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230400"
---
# <a name="video-resource-type"></a>Tipo de recurso Video

Namespace: microsoft.graph

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
| **frameRate**             | double | Taxa de quadros do vídeo.
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

