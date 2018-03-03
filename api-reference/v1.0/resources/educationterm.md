# <a name="educationterm-resource-type"></a>Tipo de recurso educationTerm

Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de [educationClass](educationclass.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName| Cadeia de caracteres| Nome de exibição do termo.| 
|externalId|Cadeia de caracteres| ID do termo no sistema de sincronização.|
|startDate|Data|Início do termo.|
|endDate|Data|Fim do termo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->