# <a name="sharepointids-resource-type"></a>Tipo de recurso SharePointIds

O recurso **SharePointIds** agrupa os vários identificadores de um item armazenado em um site do SharePoint ou no OneDrive for Business em uma única estrutura.

**Observação:** itens retornados do OneDrive pessoal não incluirão uma faceta **SharePointIds**.

### <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->
```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "webId": "string"
}
```

### <a name="properties"></a>Propriedades

| Propriedade	          | Tipo	    | Descrição                                                          |
|:------------------|:--------|:---------------------------------------------------------------------|
| listId            | cadeia de caracteres  | O identificador exclusivo da lista do item no SharePoint.                          |
| listItemId        | cadeia de caracteres  | Um identificador inteiro para o item na lista contida.                    |
| listItemUniqueId  | cadeia de caracteres  | O identificador exclusivo para o item dentro do OneDrive for Busienss ou de um site do SharePoint. |
| siteId            | cadeia de caracteres  | O identificador exclusivo da coleção de sites do item. |
| webId             | cadeia de caracteres  | O identificador exclusivo do site do item.                          |

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharepointIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
