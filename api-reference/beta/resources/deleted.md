# <a name="deleted-resource-type"></a>Tipo de recurso Deleted

O recurso **Deleted** indica que o item foi excluído. Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído. Um valor nulo (ou faltante) indica que o arquivo não foi excluído.

Consulte [Exibir alterações de um item](../api/item_delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "state"
  ],
  "@odata.type": "microsoft.graph.deleted"
}-->
```json
{
  "state": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade	 | Tipo	   | Descrição                               |
|:---------|:-------|:------------------------------------------|
| state    | Cadeia de caracteres | Representa o estado do item excluído. |

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deleted resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
