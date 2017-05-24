# <a name="schemaextension-resource-type-schema-extensions"></a>Tipo de recurso schemaExtension (extensões de esquema)

As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. 

As extensões de esquema são suportadas pelos seguintes tipos de recursos:

 - [contact](contact.md)
 - [device](device.md)
 - [event](event.md) em um usuário ou calendário de grupo do Office 365
 - [post](post.md) de um grupo do Office 365
 - [group](group.md)
 - [message](message.md) 
 - [organization](organization.md)
 - [user](user.md)

Confira o [exemplo de extensão de esquema](../../../concepts/extensibility_schema_groups.md) para aprender a adicionar dados personalizados aos grupos.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar](../api/schemaextension_post_schemaextensions.md) | schemaExtension |Crie uma definição de extensão de esquema.|
|[Listar](../api/schemaextension_list.md) | schemaExtension |Lista as definições de schemaExtension disponíveis e suas propriedades.|
|[Get](../api/schemaextension_get.md) | schemaExtension |Leia as propriedades da definição de schemaExtension específica.|
|[Atualizar](../api/schemaextension_update.md) | schemaExtension    |Atualize uma definição de schemaExtension. |
|[Excluir](../api/schemaextension_delete.md) | None |Exclua uma definição de schemaExtension. |

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição da extensão de esquema.|
|id|String|O identificador exclusivo da definição de extensão de esquema. O valor deve ser uma concatenação de um dos seus domínios verificados (por exemplo, contoso.com) e um nome da extensão de esquema (por exemplo, *contoso_mySchema*). |
|owner|String|O appId do aplicativo que criou a extensão do esquema. Somente leitura.|
|propriedades|Coleção [extensionSchemaProperty](extensionschemaproperty.md)|A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.|
|status|String|O estado do ciclo de vida da extensão de esquema. Os estados possíveis são **InDevelopment**, **Available** e **Deprecated**. Defina automaticamente como **InDevelopment** na criação. As [extensões de esquema](../../../concepts/extensibility_overview.md#schema-extensions) fornecem mais informações sobre as possíveis transições e comportamentos.|
|targetTypes|Coleção de cadeias de caracteres|O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada. Escolha entre **contact**, **device**, **event**, **group**, **message**, **organization**, **post** ou **user**.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->