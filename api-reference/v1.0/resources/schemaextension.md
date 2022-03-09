---
title: Tipo de recurso schemaExtension (extensões de esquema)
description: 'As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. '
ms.localizationpriority: high
author: dkershaw10
ms.prod: extensions
doc_type: resourcePageType
ms.openlocfilehash: 57a0aba5157265c2b9f7ba49e796f786d36f2b81
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335917"
---
# <a name="schemaextension-resource-type-schema-extensions"></a>Tipo de recurso schemaExtension (extensões de esquema)

Namespace: microsoft.graph

As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. 

As extensões de esquema são suportadas pelos seguintes tipos de recursos:

- [contact](contact.md)
- [device](device.md)
- [event](event.md) em um usuário ou calendário de grupo do Microsoft 365
- [post](post.md) de um grupo do Microsoft 365
- [grupo](group.md)
- [message](message.md) 
- [organization](organization.md)
- [user](user.md)

Confira o [exemplo de extensão de esquema](/graph/extensibility-schema-groups) para aprender a adicionar dados personalizados aos grupos.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar](../api/schemaextension-post-schemaextensions.md) | schemaExtension |Crie uma definição de extensão de esquema.|
|[Listar](../api/schemaextension-list.md) | schemaExtension |Lista as definições de schemaExtension disponíveis e suas propriedades.|
|[Get](../api/schemaextension-get.md) | schemaExtension |Leia as propriedades da definição de schemaExtension específica.|
|[Atualizar](../api/schemaextension-update.md) | schemaExtension   |Atualize uma definição de schemaExtension. |
|[Excluir](../api/schemaextension-delete.md) | None |Exclua uma definição de schemaExtension. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição da extensão de esquema. Suporta `$filter` (`eq`).|
|id|String|O identificador exclusivo da definição de extensão de esquema. <br>Você pode atribuir um valor em uma destas duas maneiras: <ul><li>Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </li><li>Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</li></ul>Esta propriedade não pode ser alterada após a criação. Suporta `$filter` (`eq`). **Observação:** recomendamos que sua **id** comece com uma letra alfabética entre A-Z porque os recursos de consulta podem ser limitados para as IDs que começam com inteiros. |
|proprietário|String|O `appId` do aplicativo que é o proprietário da extensão de esquema. Essa propriedade pode ser fornecida na criação, para definir o proprietário.  Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário. Em ambos os casos, o usuário conectado deve ser o proprietário do aplicativo. Então, por exemplo, se criar uma nova definição de extensão do esquema usando o Explorador do Graph, você **deverá** fornecer a propriedade de proprietário. Uma vez definida, essa propriedade é somente leitura e não pode ser alterada. Suporta `$filter` (`eq`).| 
|properties|Coleção [extensionSchemaProperty](extensionschemaproperty.md)|A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.|
|status|String|O estado do ciclo de vida da extensão do esquema. Os estados possíveis são **EmDesenvolvimento**, **Disponível** e **Preterido**. Defina automaticamente como **EmDesenvolvimento** na criação. As [Extensões de esquema](/graph/extensibility-overview#schema-extensions) fornecem mais informações sobre as possíveis transições e comportamentos. Suporta `$filter` (`eq`).|
|targetTypes|Coleção de cadeias de caracteres|O conjunto de tipos do Microsoft Graph (que podem suportar extensões) ao qual a extensão de esquema pode ser aplicada. Escolha entre **contact**, **device**, **event**, **group**, **message**, **organization**, **post** ou **user**.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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

