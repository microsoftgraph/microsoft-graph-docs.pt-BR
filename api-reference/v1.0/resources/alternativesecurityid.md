# <a name="alternativesecurityid-resource-type"></a>Tipo de recurso alternativeSecurityId

Contém uma ID de segurança alternativa associada a um dispositivo. A propriedade **alternativeSecurityIds** da entidade [Device](device.md) é uma coleção de **alternativeSecurityId**.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|identityProvider|Cadeia de caracteres|            |
|chave|Binário|            |
|type|Int32|            |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "identityProvider": "string",
  "key": "binary",
  "type": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alternativeSecurityId resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
