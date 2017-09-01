# <a name="itemreference-resource-type"></a>Tipo de recurso ItemReference

O recurso **ItemReference** proporciona as informações necessárias para enviar um [DriveItem](driveitem.md) pela API.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                              | Descrição                                                                                                |
| :------------ | :-------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| driveId       | String                            | O identificador exclusivo da instância da unidade que contém o item. Somente leitura.                                 |
| id            | String                            | Identificador exclusivo do item na unidade. Somente leitura.                                                     |
| nome          | String                            | O nome do item ao qual se faz referência. Somente leitura.                                                          |
| caminho          | String                            | Caminho que pode ser usado para navegar até o item. Somente leitura.                                                  |
| shareId       | String                            | Um identificador exclusivo para um recurso compartilhado que pode ser acessado através da API [Shares](../api/shares_get.md). |
| sharepointIds | [sharepointIds](sharepointids.md) | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.                                   |

## <a name="remarks"></a>Comentários

Para lidar com um **driveItem** de um recurso **itemReference**, crie uma URL no formato:

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

O valor **path** é um caminho da API relativo à unidade de destino, por exemplo: `/drive/root:/Documents/myfile.docx`.

Para recuperar o caminho legível para a navegação estrutural, ignore tudo até o primeiro `:` na cadeia de caracteres do caminho.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
