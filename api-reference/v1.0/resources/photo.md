# <a name="photo-resource-type"></a>Tipo de recurso Photo

O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1024,
  "exposureNumerator": 1024,
  "fNumber": 1024,
  "focalLength": 1024,
  "iso": 1024,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>Propriedades
| Propriedade                | Tipo                      | Descrição                                                     |
|:------------------------|:--------------------------|:----------------------------------------------------------------|
| **takenDateTime**       | DateTimeOffset            | Representa a data e a hora em que a foto foi tirada. Somente leitura.               |
| **cameraMake**          | Cadeia de caracteres                    | Fabricante da câmera. Somente leitura.                                            |
| **cameraModel**         | Cadeia de caracteres                    | Modelo da câmera. Somente leitura.                                                   |
| **fNumber**             | Double                    | O valor de f-stop da câmera. Somente leitura.                               |
| **exposureDenominator** | Int32                     | O denominador da fração do tempo de exposição da câmera. Somente leitura. |
| **exposureNumerator**   | Int32                     | O numerador da fração do tempo de exposição da câmera. Somente leitura.   |
| **focalLength**         | Double                    | A distância focal da câmera. Somente leitura.                               |
| **iso**                 | Int32                     | O valor de ISO da câmera. Somente leitura.                                  |

## <a name="remarks"></a>Comentários
O OneDrive for Business e o SharePoint retornam apenas a propriedade **takenDateTime**.

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "photo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
