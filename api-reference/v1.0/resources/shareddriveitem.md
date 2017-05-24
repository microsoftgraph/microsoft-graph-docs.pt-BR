# <a name="shareddriveitem-resource-type"></a>Tipo de recurso SharedDriveItem

O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares_get.md) para acessar um [driveItem](driveitem.md) compartilhado.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.

O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.

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

    /* relationships*/
    "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
    "root": { "@odata.type": "microsoft.graph.driveItem" },
    "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
    "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                          | Descrição                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | String                        | O identificador exclusivo do compartilhamento que está sendo acessado.              |
| name     | String                        | O nome de exibição do item compartilhado.                             |
| owner    | [IdentitySet](identityset.md) | Informações sobre o proprietário do item compartilhado que está sendo referenciado. |

## <a name="relationships"></a>Relações

| Relação | Tipo                                  | Descrição                                                                                                                                                                                                |
| :----------- | :------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| itens        | Collection([DriveItem](driveitem.md)) | Um conjunto de recursos **driveItem** compartilhados. Não é possível enumerar este conjunto, mas os itens podem ser acessados por sua ID exclusiva.                                                                        |
| root         | [DriveItem](driveitem.md)             | O **driveItem** compartilhado de nível superior. Se um único arquivo for compartilhado, este item será o arquivo. Se uma pasta for compartilhada, este item será a pasta. Você pode usar aspectos do item para determinar qual caso é aplicável. |
| driveItem    | [driveItem](driveitem.md)             | Um **driveItem** do recurso que foi compartilhado.  É idêntico à propriedade **root**.                                                                                                             |
| site         | [site](site.md)                       | Um recurso **site** que contém o item que foi compartilhado.                                                                                                                                                |

## <a name="methods"></a>Métodos

| Método                                  | Caminho REST                |
| :-------------------------------------- | :----------------------- |
| [Obter item compartilhado](../api/shares_get.md) | `GET /shares/{share-id}` |

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