# <a name="directoryobject-resource-type"></a>tipo de recurso directoryObject

Representa um objeto do Active Directory do Azure. O tipo **directoryObject** é o tipo básico de muitos outros tipos de entidade de diretório.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter directoryObject](../api/directoryobject_get.md) | [directoryObject](directoryobject.md) |Ler as propriedades de um objeto de diretório.|
|[Excluir directoryObject](../api/directoryobject_delete.md) | Nenhum |Excluir um objeto de diretório. |
|[checkMemberGroups](../api/directoryobject_checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.|
|[getMemberGroups](../api/directoryobject_getmembergroups.md)|Coleção de cadeias de caracteres|Retornar todos os grupos dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva.|
|[getMemberObjects](../api/directoryobject_getmemberobjects.md)|Coleção de cadeias de caracteres| Retornar todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. A verificação é transitiva. |
|[getByIds](../api/directoryobject_getbyids.md) | coleção [directoryObject](directoryobject.md) | Obter um conjunto de objetos de diretório com base em um conjunto de ids fornecidas. |

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|Um GUID que é o identificador exclusivo do objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde. Chave. Não anulável. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
