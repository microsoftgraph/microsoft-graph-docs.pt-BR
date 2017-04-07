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
  "bitrate": 1024,
  "duration": 1024,
  "height": 1024,
  "width": 1024
}
```

## <a name="properties"></a>Propriedades

| Propriedade	 | Tipo	  | Descrição                               |
|:---------|:------|:------------------------------------------|
| bitrate  | Int32 | Taxa de bits do vídeo em bits por segundo. |
| duration | Int64 | Duração do arquivo em milissegundos.     |
| height   | Int32 | A altura do vídeo em pixels.           |
| width    | Int32 | A largura do vídeo em pixels.            |

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "video resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
