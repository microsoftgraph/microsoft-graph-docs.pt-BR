# <a name="directory-resource-type-deleted-items"></a>Tipo de recurso directory (itens excluídos)

Representa um item excluído no diretório. Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos. Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.

Atualmente, a funcionalidade de itens excluídos apenas tem suporte para [grupos](group.md) e [usuários](users.md) do Office 365.

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno | Descrição |
|:---------------|:------------|:------------|
|[Obter item excluído](../api/directory_deleteditems_get.md) | [directoryObject](directoryobject.md) | Obtém as propriedades de um item excluído. |
|[Restaurar item excluído](../api/directory_deleteditems_restore.md) |[directoryObject](directoryobject.md)| Restaura um item recentemente excluído. |
|[Listar itens excluídos](../api/directory_deleteditems_list.md) |coleção [directoryObject](directoryobject.md)| Obtém uma lista de itens recentemente excluídos. |
|[Excluir permanentemente um item](../api/directory_deleteditems_delete.md) | Nenhum | Exclui permanentemente um item. |
|[Lista itens excluídos pertencentes a um usuário](../api/directory_deleteditems_user_owned.md) | coleção [directoryObject](directoryobject.md) | Lista os itens de diretório pertencentes a um usuário. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|deleteditems|coleção [directoryObject](directoryobject.md)| Itens recentemente excluídos. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a>Exemplo

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->