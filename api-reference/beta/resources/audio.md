# <a name="audio-resource-type"></a>Tipo de recurso de áudio

O recurso **Audio** agrupa propriedades relacionadas a áudio em um item em uma estrutura simples.

Se um [**DriveItem**](driveitem.md) tiver uma faceta **audio** não nula, o item representará um arquivo de áudio. As propriedades do recurso **Áudio** são preenchidas extraindo-se os metadados do arquivo. 

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.audio"
}-->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 1024,
  "composers": "string",
  "copyright": "string",
  "disc": 1024,
  "discCount": 1024,
  "duration": 1024,
  "genre": "string",
  "hasDrm": true,
  "isVariableBitrate": true,
  "title": "string",
  "track": 1024,
  "trackCount": 1024,
  "year": 1024
}
```

## <a name="properties"></a>Propriedades

| Propriedade	          | Tipo	    | Descrição                                                          |
|:------------------|:--------|:---------------------------------------------------------------------|
| album             | string  | O título do álbum para este arquivo de áudio.                          |
| albumArtist       | string  | Artista nomeado no álbum para o arquivo de áudio.                    |
| artist            | string  | O artista do arquivo de áudio.                            |
| bitrate           | string  | Taxa de bits expressa em kbps.                                           |
| composers         | string  | O nome do compositor do arquivo de áudio.                          |
| copyright         | string  | Informações de direitos autorais para o arquivo de áudio.                            |
| disc              | number  | O número do disco do qual este arquivo de áudio é proveniente.                    |
| discCount         | number  | O número total de discos neste álbum.                             |
| duration          | number  | Duração do arquivo de áudio, expressa em milissegundos                |
| genre             | string  | O gênero deste arquivo de áudio.                                        |
| hasDrm            | booliano | Indica se o arquivo está protegido com o gerenciamento de direitos digitais.   |
| isVariableBitrate | booliano | Indica se o arquivo é codificado com uma taxa de bits variável.            |
| title             | string  | O título do arquivo de áudio.                                         |
| track             | number  | O número da faixa no disco original para este arquivo de áudio.    |
| trackCount        | number  | O número total de faixas no disco original para este arquivo de áudio. |
| year              | number  | O ano em que o arquivo de áudio foi gravado.                                |

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audio resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->