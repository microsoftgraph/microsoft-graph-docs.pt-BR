# <a name="educationorganization-resource-type"></a>tipo de recurso educationOrganization

Entidade abstrata usada para modelar o que há de comum entre tipos diferentes de organização dentro do setor de educação.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|descrição|Cadeia de caracteres| Descrição da organização.|
|displayName|Cadeia de caracteres| Nome para exibição da organização.|
|externalSource|educationExternalSource| Fonte a partir da qual esta organização foi criada. Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->