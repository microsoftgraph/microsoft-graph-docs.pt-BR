---
author: ananmishr
ms.date: 09/10/2017
title: Áudio
localization_priority: Normal
ms.prod: microsoft-teams
description: O recurso Audio agrupa propriedades relacionadas a áudio em um item em uma estrutura simples.
doc_type: resourcePageType
ms.openlocfilehash: 1351ae9dcd363d156997fd5cc75e7e3387a0fb38
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913482"
---
# <a name="audio-facet"></a>Faceta Audio

O recurso **Audio** agrupa propriedades relacionadas a áudio em um item em uma estrutura simples.

Se um [**DriveItem**](driveitem.md) tiver uma faceta **audio** não nula, o item representará um arquivo de áudio. As propriedades do recurso **Áudio** são preenchidas extraindo-se os metadados do arquivo. 

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.audio" } -->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 128,
  "composers": "string",
  "copyright": "string",
  "disc": 0,
  "discCount": 0,
  "duration": 567,
  "genre": "string",
  "hasDrm": false,
  "isVariableBitrate": false,
  "title": "string",
  "track": 1,
  "trackCount": 16,
  "year": 2014
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade         | Tipo    | Descrição                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| **album**             | cadeia de caracteres  | O título do álbum deste arquivo de áudio.                          |
| **albumArtist**       | cadeia de caracteres  | Artista nomeado no álbum para o arquivo de áudio.                    |
| **artist**            | cadeia de caracteres  | O artista do arquivo de áudio.                            |
| **bitrate**           | Int64   | Taxa de bits expressa em kbps.                                           |
| **composers**         | cadeia de caracteres  | O nome do compositor do arquivo de áudio.                          |
| **copyright**         | cadeia de caracteres  | Informações de direitos autorais para o arquivo de áudio.                            |
| **disc**              | Int16   | O número do disco do qual este arquivo de áudio é proveniente.                    |
| **discCount**         | Int16   | O número total de discos neste álbum.                             |
| **duration**          | Int64   | Duração do arquivo de áudio, expressa em milissegundos                |
| **genre**             | cadeia de caracteres  | O gênero deste arquivo de áudio.                                        |
| **hasDrm**            | booliano | Indica se o arquivo está protegido com o gerenciamento de direitos digitais.   |
| **isVariableBitrate** | booliano | Indica se o arquivo é codificado com uma taxa de bits variável.            |
| **title**             | string  | O título do arquivo de áudio.                                         |
| **track**             | Int32   | O número da faixa no disco original para este arquivo de áudio.    |
| **trackCount**        | Int32   | O número total de faixas no disco original para este arquivo de áudio. |
| **year**              | Int32   | O ano em que o arquivo de áudio foi gravado.                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
