# <a name="shareddriveitem-resource-type"></a>Tipo de recurso SharedDriveItem

O recurso **SharedDriveItem** é retornado ao se usar a API [Shares](../api/shares_get.md) para acessar um [DriveItem](driveitem.md) compartilhado. Este recurso é semelhante a um recurso [Drive](drive.md), mas tem o escopo delimitado somente para DriveItems que podem ser acessados pelo link de compartilhamento ou shareId.

### <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->
```json
{
    "id": "string",
    "name": "string",
    "owner": { "@odata.type": "microsoft.graph.identitySet" },
    "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
    "root": { "@odata.type": "microsoft.graph.driveItem" }
}
```

### <a name="properties"></a>Propriedades

| Propriedade	  | Tipo	                                  | Descrição                                                          |
|:----------|:--------------------------------------|:---------------------------------------------------------------------|
| id        | String                                | O identificador exclusivo do compartilhamento que está sendo acessado.                  |
| name      | String                                | O nome de exibição do item compartilhado.                                 |
| owner     | [IdentitySet](identityset.md)         | Informações sobre o proprietário do item compartilhado que está sendo referenciado.     |
| items     | Collection([DriveItem](driveitem.md)) | Uma coleção de recursos DriveItem compartilhados. Não é possível enumerar esta coleção, mas os itens podem ser acessados por sua ID exclusiva. |
| root      | [DriveItem](driveitem.md)             | O DriveItem compartilhado de nível superior. Se um único arquivo for compartilhado, este item será o arquivo. Se uma pasta for compartilhada, este item será a pasta. Você pode usar aspectos do item para determinar qual caso é aplicável. |

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