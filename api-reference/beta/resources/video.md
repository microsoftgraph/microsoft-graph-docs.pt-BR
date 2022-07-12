---
author: JeremyKelley
description: O recurso Video agrupa itens de dados relacionados a vídeos em uma única estrutura.
ms.date: 09/10/2017
title: Vídeos
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 7bd266b8905620bfede51bea0f79c71f6b7f417d
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734659"
---
# <a name="video-resource-type"></a>Tipo de recurso Video

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
  "height": 1280,
  "width": 720,
  "framerate": 2.75
}
```

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo   | Descrição                                     |
| :------------------------ | :----- | :---------------------------------------------- |
| **audioBitsPerSample**    | Int32  | Número de bits áudio por amostra.                |
| **audioChannels**         | Int32  | Número de canais de áudio.                       |
| **audioFormat**           | string | Nome do formato áudio (AAC, MP3, etc.).      |
| **audioSamplesPerSecond** | Int32  | Número de amostras de áudio por segundo.             |
| **bitrate**               | Int32  | Taxa de bits do vídeo em bits por segundo.       |
| **duration**              | Int64  | Duração do arquivo em milissegundos.           |
| **fourCC**                | string | Nome do formato de vídeo "Código de quatro caracteres". |
| **framerate**             | double | Taxa de quadros do vídeo.                        |
| **height**                | Int32  | A altura do vídeo em pixels.                 |
| **width**                 | Int32  | A largura do vídeo em pixels.                  |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
