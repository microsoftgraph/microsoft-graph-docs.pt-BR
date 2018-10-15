# <a name="sortfield-resource-type"></a>Tipo de recurso SortField

Representa uma condição em uma operação de classificação.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|ascendente|booliano|Indica se a classificação é feita de forma crescente.|
|cor|sequência de caracteres|Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.|
|dataOption|sequência de caracteres|Representa as opções de classificação adicionais para esse campo. Os valores possíveis são: `Normal`, `TextAsNumber`.|
|chave|int|Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).|
|sortOn|sequência de caracteres|Representa o tipo de classificação dessa condição. Os valores possíveis são: `Value`, `CellColor`, `FontColor`, `Icon`.|
|ícone|[WorkbookIcon](icon.md)|Representa o ícone que é o destino da condição, se a classificação estiver no ícone da célula.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->