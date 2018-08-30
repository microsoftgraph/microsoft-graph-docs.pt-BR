# <a name="filterdatetime-resource-type"></a>Tipo de recurso FilterDatetime

Indica como filtrar uma data ao filtrar valores.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|data|sequência de caracteres|A data no formato ISO8601 usada para filtrar os dados.|
|especificidade|sequência de caracteres|Quão específica a data deve ser para manter os dados. Por exemplo, se a data é 2005-04-02 e a especificidade estiver definida como "mês", a operação de filtro manterá todas as linhas com uma data no mês de abril de 2009. Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->