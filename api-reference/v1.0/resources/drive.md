# <a name="drive-resource-type"></a>Tipo de unidade de recurso

O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.

Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "items", "root", "special" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive"
}-->
```json
{
  "id": "string (identifier)",
  "driveType": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "root": {"@odata.type": "microsoft.graph.driveItem" },
  "items": [ {"@odata.type": "microsoft.graph.driveItem" }],
  "special": [ {"@odata.type": "microsoft.graph.driveItem" }]
}
```

## <a name="properties"></a>Propriedades

| Propriedade	  | Tipo	                          | Descrição                                                                                          |
|:----------|:------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| id        | String                        | O identificador exclusivo da unidade. Somente leitura.                                                                                                           |
| driveType | String                        | Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura. |
| owner     | [identitySet](identityset.md) | Opcional. A conta do usuário que é proprietário da unidade.                                                                                                                    |
| cota     | [quota](quota.md)             | Opcional. Informações sobre a cota de espaço de armazenamento da unidade.                                                                                                       |

## <a name="relationships"></a>Relações

| Relação | Tipo	 |Descrição |
|:--------|:---------------------------|:-------------------------------------------------------------------------|
| items   | Coleção [driveitem](driveitem.md) | Todos os itens contidos na unidade. Somente leitura. Anulável.                   |
| root    | [driveitem](driveitem.md)            | A pasta raiz da unidade. Somente leitura.                                 |
| special | Coleção [driveitem](driveitem.md) | Coleção de pastas comuns disponíveis no OneDrive. Somente leitura. Anulável. |


## <a name="methods"></a>Métodos

Os métodos a seguir estão disponíveis para os recursos drive.

| Método                                                    | Caminho REST                            | 
|:----------------------------------------------------------|:-------------------------------------|
| [Obter unidade padrão do usuário](../api/drive_get.md)           | `GET /me/drive`                      |
| [Obter a unidade de outro usuário](../api/drive_get.md)           | `GET /users/{user-id}/drive`         |
| [Obter pasta raiz de uma unidade](../api/item_get.md)         | `GET /drives/{drive-id}/root`        |
| [Listar itens em uma unidade](../api/item_list_children.md)     | `GET /me/drive/root/children`        |
| [Listar alterações em uma unidade](../api/item_delta.md)           | `GET /me/drive/root/delta`           |
| [Pesquisar itens em uma unidade](../api/item_search.md)          | `GET /me/drive/search(q='text')`     |




<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "drive resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive"
}-->
