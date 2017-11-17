# <a name="recurrencepattern-resource-type"></a>Tipo de recurso recurrencePattern

A frequência de um evento.


## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|dayOfMonth|Int32|O dia do mês em que o evento ocorre.|
|daysOfWeek|Coleção de cadeias de caracteres|Uma coleção de dias da semana em que o evento ocorre. Os valores possíveis são: `Sunday`, `Monday`, `Tuesday`, `Wednesday`, `Thursday`, `Friday` e `Saturday`.|
|firstDayOfWeek|String|O dia da semana em que a recorrência começa. Os valores possíveis são: `Sunday`, `Monday`, `Tuesday`, `Wednesday`, `Thursday`, `Friday` e `Saturday`.|
|índice|Cadeia de caracteres|O índice da semana em que a recorrência ocorre: `First`, `Second`, `Third`, `Fourth` e `Last`.|
|interval|Int32|O número de unidades de um determinado tipo de recorrência entre as ocorrências.|
|month|Int32|O mês em que o evento ocorre.  É um número entre 1 e 12.|
|type|Cadeia de caracteres|O tipo de padrão da recorrência: `Daily`, `Weekly`, `AbsoluteMonthly`, `RelativeMonthly`, `AbsoluteYearly` e `RelativeYearly`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencepattern"
}-->

```json
{
  "dayOfMonth": 1024,
  "daysOfWeek": ["String"],
  "firstDayOfWeek": "String",
  "index": "String",
  "interval": 1024,
  "month": 1024,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->