# <a name="workbooksessioninfo-resource-type"></a>Tipo de recurso workbookSessionInfo

Fornece informações sobre a sessão de pasta de trabalho.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo  | Descrição                               |
|:---------|:------|:------------------------------------------|
| id  | cadeia de caracteres | ID da sessão de pasta de trabalho. |
| persistChanges | booleano |  `true` para sessão persistente. `false` para sessão não persistente (modo de exibição) |

