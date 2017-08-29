# <a name="geocoordinates-resource-type"></a>Tipo de recurso GeoCoordinates

O recurso **GeoCoordinates** fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo. Se um [**DriveItem**](driveitem.md) tiver uma faceta **location** não nula, o item representa um arquivo com um local conhecido associado a ele.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo   | Descrição                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| altitude  | Double | Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura. |
| latitude  | Double | Opcional. A latitude, em valor decimal, para o item. Somente leitura.   |
| longitude | Double | Opcional. A longitude, em valor decimal, para o item. Somente leitura.  |

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "geoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
