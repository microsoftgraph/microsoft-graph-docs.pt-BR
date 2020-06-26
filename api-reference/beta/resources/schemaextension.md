---
title: Tipo de recurso schemaExtension (extensões de esquema)
description: 'Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource. '
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 6959a21d2341c9868c8a3e20e39098c1fe048277
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896963"
---
# <a name="schemaextension-resource-type-schema-extensions"></a>Tipo de recurso schemaExtension (extensões de esquema)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource. 

As extensões de esquema são suportadas pelos seguintes tipos de recursos:

- [administrativeUnit](administrativeunit.md)
- [contact](contact.md)
- [device](device.md)
- [evento](event.md) em um usuário ou calendário de grupo do Microsoft 365
- [postagem](post.md) de um grupo do Microsoft 365
- [group](group.md)
- [message](message.md) 
- [organization](organization.md)
- [user](user.md)

Confira o [exemplo de extensão de esquema](/graph/extensibility-schema-groups) para aprender a adicionar dados personalizados aos grupos.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar](../api/schemaextension-post-schemaextensions.md) | schemaExtension |Crie uma definição de extensão de esquema.|
|[Listar](../api/schemaextension-list.md) | schemaExtension |Liste a avaialbe schemaExtension defintions e suas propriedades.|
|[Get](../api/schemaextension-get.md) | schemaExtension |Leia as propriedades da definição de schemaExtension específica.|
|[Atualizar](../api/schemaextension-update.md) | schemaExtension   |Atualize uma definição de schemaExtension. |
|[Excluir](../api/schemaextension-delete.md) | None |Exclua uma definição de schemaExtension. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|Cadeia de caracteres|Descrição da extensão de esquema.|
|id|String|O identificador exclusivo da definição de extensão de esquema. <br>Você pode atribuir um valor em uma destas duas maneiras: <ul><li>Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </li><li>Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</li></ul>Esta propriedade não pode ser alterada após a criação. |
|owner|String|O `appId` do aplicativo que é o proprietário da extensão de esquema. Essa propriedade pode ser fornecida na criação, para definir o proprietário.  Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário. Em ambos os casos, o usuário conectado deve ser o proprietário do aplicativo. Uma vez definida, essa propriedade é somente leitura e não pode ser alterada.|
|properties|Coleção [extensionSchemaProperty](extensionschemaproperty.md)|A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.|
|status|String|The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.|
|targetTypes|Coleção de cadeias de caracteres|Conjunto de tipos do Microsoft Graph (que podem suportar extensões) à qual a extensão de esquema pode ser aplicada. Selecione entre **administrativeUnit**, **contato**, **dispositivo**, **evento**, **grupo**, **mensagem**, **organização**, **postagem**ou **usuário**.|

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
<!--
{
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
