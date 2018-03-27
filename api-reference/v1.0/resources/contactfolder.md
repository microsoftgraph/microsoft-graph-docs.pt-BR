# <a name="contactfolder-resource-type"></a>tipo de recurso contactFolder

Uma pasta que contém contatos.

Esse recurso suporta a utilização da [consulta delta](../../../concepts/delta_query_overview.md) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contactfolder_delta.md).


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter contactFolder](../api/contactfolder_get.md) | [contactFolder](contactfolder.md) |Obtenha uma pasta de contatos usando a respectiva ID.|
|[Update](../api/contactfolder_update.md) | [contactFolder](contactfolder.md) |Atualize o objeto contactFolder. |
|[Delete](../api/contactfolder_delete.md) | Nenhuma |Exclua um objeto contactFolder. |
|[Listar childFolders](../api/contactfolder_list_childfolders.md) |Coleção [ContactFolder](contactfolder.md)| Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.|
|[Criar contactFolder filho](../api/contactfolder_post_childfolders.md) |[ContactFolder](contactfolder.md)| Crie uma nova contactFolder como um filho de uma pasta especificada.|
|[delta](../api/contact_delta.md)|Coleção [Contact](contact.md)| Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.|
|[Listar contatos na pasta](../api/contactfolder_list_contacts.md) |Coleção [Contact](contact.md)| Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.|
|[Criar contato na pasta](../api/contactfolder_post_contacts.md) |[Contact](contact.md)| Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.|
|[Criar propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[contactFolder](contactFolder.md)  |Criar uma ou mais propriedades estendidas de valor único em uma contactFolder nova ou existente.   |
|[Obter contactFolder com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_get.md)  | [contactFolder](contactFolder.md) | Obtenha contactFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [contactFolder](contactFolder.md) | Criar uma ou mais propriedades estendidas de vários valores em uma contactFolder nova ou existente.  |
|[Obter contactFolder com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_get.md)  | [contactFolder](contactFolder.md) | Obtenha uma contactFolder que contém uma propriedade estendida com vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String|O nome de exibição da pasta.|
|id|String|Identificador exclusivo da pasta de contatos. Somente leitura.|
|parentFolderId|String|A ID da pasta pai da pasta.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|childFolders|Coleção [ContactFolder](contactfolder.md)|A coleção de pastas filho na pasta. Propriedade de navegação. Somente leitura. Anulável.|
|contatos|Coleção [Contact](contact.md)|Os contatos na pasta. Propriedade de navegação. Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](../../../concepts/delta_query_overview.md)
- [Obter as alterações incrementais para as mensagens em uma pasta](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
