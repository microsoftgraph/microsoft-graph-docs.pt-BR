# <a name="recurrencerange-resource-type"></a>Tipo de recurso recurrenceRange

A duração de um evento.

## <a name="properties"></a>Propriedades

| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|endDate|Date|A data de término da série.|
|numberOfOccurrences|Int32|Quantas vezes o evento deve repetir.|
|recurrenceTimeZone|Cadeia de caracteres |Fuso horários das propriedades **startDate** e **endDate**. |
|startDate|Date|A data de início da série.|
|type|String|O intervalo de recorrência: EndDate = 0, NoEnd = 1, Numbered = 2. Os valores possíveis são: `EndDate`, `NoEnd` e `Numbered`.||


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencerange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
