<a id="schemaextension-resource-type-schema-extensions" class="xliff"></a>

# Tipo de recurso schemaExtension (extensões de esquema)

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

<a id="methods" class="xliff"></a>

## Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar](../api/schemaextension_post_schemaextensions.md) | schemaExtension |Crie uma definição de extensão de esquema.|
|[Listar](../api/schemaextension_list.md) | schemaExtension |Lista as definições de schemaExtension disponíveis e suas propriedades.|
|[Get](../api/schemaextension_get.md) | schemaExtension |Leia as propriedades da definição de schemaExtension específica.|
|[Atualizar](../api/schemaextension_update.md) | schemaExtension   |Atualize uma definição de schemaExtension. |
|[Excluir](../api/schemaextension_delete.md) | None |Exclua uma definição de schemaExtension. |

<a id="properties" class="xliff"></a>

## Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição da extensão de esquema.|
|id|String|O identificador exclusivo da definição de extensão de esquema. <br>Você pode atribuir um valor em uma destas duas maneiras: <ul><li>Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </li><li>Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</li></ul>Esta propriedade não pode ser alterada após a criação. |
|owner|String|O appId do aplicativo que criou a extensão do esquema. Somente leitura.|
|propriedades|Coleção [extensionSchemaProperty](extensionschemaproperty.md)|A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.|
|status|String|O estado do ciclo de vida da extensão de esquema. Os estados possíveis são **InDevelopment**, **Available** e **Deprecated**. Defina automaticamente como **InDevelopment** na criação. As [extensões de esquema](../../../concepts/extensibility_overview.md#schema-extensions) fornecem mais informações sobre as possíveis transições e comportamentos.|
|targetTypes|Coleção de cadeias de caracteres|O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada. Escolha entre **contact**, **device**, **event**, **group**, **message**, **organization**, **post** ou **user**.|

<a id="json-representation" class="xliff"></a>

## Representação JSON

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