# <a name="permission-resource-type"></a>Tipo de recurso permission

O recurso **Permission** fornece informações sobre uma permissão concedida a um recurso [DriveItem](driveitem.md).

Permissões têm um número de formas diferentes. O recurso **Permission** representa estes diferentes formulários por meio de facetas do recurso.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "link", "grantedTo", "invitation", "inheritedFrom", "shareId" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permission"
}-->
```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                                      | Descrição
|:--------------|:------------------------------------------|:-----------------
| id            | String                                    | O identificador exclusivo da permissão entre todas as permissões no item. Somente leitura.
| grantedTo     | [IdentitySet](identityset.md)             | Para permissões de tipo de usuário, os detalhes de usuários e aplicativos para esta permissão. Somente leitura.
| invitation    | [SharingInvitation][]                     | Detalhes de um convite de compartilhamento associado para esta permissão. Somente leitura.
| inheritedFrom | [ItemReference](itemreference.md)         | Fornece uma referência para o ancestral da permissão atual, se ela for herdada de um ancestral. Somente leitura.
| vínculo          | [SharingLink][]                           | Fornece os detalhes do link de permissão atual, caso se trate de permissões de tipo de link. Somente leitura.
| role          | Coleção de Cadeias de Caracteres                      | O tipo de permissão, por exemplo, `read`. Veja abaixo a lista completa de funções. Somente leitura.
| shareId       | String                                    | Um token exclusivo que pode ser usado para acessar esse item compartilhado por meio da [ **API** Shares](../api/shares_get.md). Somente leitura.

O recurso permission usa _facetas_ para fornecer informações sobre o tipo de permissão representado pelo recurso.

Permissões com uma faceta [**link**][SharingLink] representam links de compartilhamento criados no item. Os links de compartilhamento contêm um token exclusivo que fornece acesso ao item para qualquer pessoa com o link.

Permissões com uma faceta [**invitation**][SharingInvitation] representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

## <a name="roles-enumeration"></a>Enumeração de funções

| Função        | Detalhes                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | Fornece a capacidade de ler os metadados e o conteúdo do item.            |
| `write`     | Fornece a capacidade de ler e modificar os metadados e o conteúdo do item. |
| `sp.owner`  | Para o SharePoint e o OneDrive for Business, isso representa a função de proprietário.       |
| `sp.member` | Para o SharePoint e o OneDrive for Business, isso representa a função de membro.      |

## <a name="methods"></a>Métodos

| Método                                              | Caminho REST
|:----------------------------------------------------|:-----------------------
| [Listar permissões](../api/item_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Obter permissão](../api/permission_get.md)          | `GET /drive/items/{item-id}/permissions/{id}`
| [Adicionar](../api/item_invite.md)                        | `POST /drive/items/{item-id}/invite`
| [Update](../api/permission_update.md)               | `PATCH /drive/items/{item-id}/permissions/{id}`
| [Delete](../api/permission_delete.md)               | `DELETE /drive/items/{item-id}/permissions/{id}`


## <a name="remarks"></a>Comentários

O OneDrive Business e as bibliotecas de documentos do SharePoint não retornam a propriedade **inheritedFrom**.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
