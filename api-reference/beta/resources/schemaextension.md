---
title: Tipo de recurso schemaExtension (extensões de esquema)
description: 'As extensões de esquema permitem que você defina um esquema para estender e adicionar dados personalizados digitados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. '
ms.localizationpriority: medium
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: fbbdeccaf38bda627c9a3aab23d784b184c364fb
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555938"
---
# <a name="schemaextension-resource-type-schema-extensions"></a>Tipo de recurso schemaExtension (extensões de esquema)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As extensões de esquema permitem definir um esquema para estender e adicionar dados personalizados fortemente tipados a um tipo de recurso. Os dados personalizados aparecem como um tipo complexo no recurso estendido. As extensões de esquema são suportadas pelos seguintes tipos de recursos:

+ [user](/graph/api/resources/user)
+ [group](/graph/api/resources/group)
+ [administrativeUnit](/graph/api/resources/administrativeunit)
+ [contact](/graph/api/resources/contact)
+ [device](/graph/api/resources/device)
+ [evento](/graph/api/resources/event) (para calendários de usuário e grupo)
+ [message](/graph/api/resources/message)
+ [organização](/graph/api/resources/organization)
+ [postagem](/graph/api/resources/post)
+ [todoTask](/graph/api/resources/todotask)
+ [todoTaskList](/graph/api/resources/todotasklist)

Use esse recurso e métodos associados para gerenciar as [definições de extensão de esquema](/graph/api/resources/schemaextension). Para gerenciar os dados de extensão de esquema na instância de recurso estendido, use a mesma solicitação REST que você usa para gerenciar a instância de recurso. Confira o [exemplo de extensão de esquema](/graph/extensibility-schema-groups) para aprender a adicionar dados personalizados aos grupos.

Para obter mais informações sobre a extensibilidade do Microsoft Graph, incluindo limites para extensões de esquema, consulte Adicionar propriedades personalizadas aos recursos [usando extensões](/graph/extensibility-overview).

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
|id|String|O identificador exclusivo da definição de extensão de esquema. <br>Você pode atribuir um valor em uma destas duas maneiras: <ul><li>Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </li><li>Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</li></ul>Esta propriedade não pode ser alterada após a criação. Suporta `$filter` (`eq`).<br/><br> **Observação:** recomendamos que sua **id** comece com uma letra alfabética entre A-Z porque os recursos de consulta podem ser limitados para as IDs que começam com inteiros. |
|proprietário|String| O `appId` do aplicativo que é o proprietário da extensão de esquema. Essa propriedade pode ser fornecida na criação, para definir o proprietário.  Se não for fornecida, o aplicativo de chamada `appId` será definido como o proprietário. Em ambos os casos, o usuário conectado deve ser o proprietário do aplicativo. Então, por exemplo, se criar uma nova definição de extensão do esquema usando o Explorador do Graph, você **deverá** fornecer a propriedade de proprietário. Uma vez definida, essa propriedade é somente leitura e não pode ser alterada. Suporta `$filter` (`eq`).|
|properties|Coleção [extensionSchemaProperty](extensionschemaproperty.md)|A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.|
|status|String|O estado do ciclo de vida da extensão do esquema. Os estados possíveis `InDevelopment`são `Available`, e `Deprecated`. Definido automaticamente como `InDevelopment` na criação. Para obter mais informações sobre as possíveis transições de estado e comportamentos, consulte [o ciclo de vida das extensões de esquema](#schema-extensions-lifecycle). Suporta `$filter` (`eq`).|
|targetTypes|Coleção de cadeias de caracteres|Conjunto de tipos do Microsoft Graph (que podem dar suporte a extensões) aos quais a extensão de esquema pode ser aplicada. Selecione entre **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, **todoTask**, **todoTaskList** ou **user**.|


### <a name="schema-extensions-lifecycle"></a>Ciclo de vida das extensões do esquema

Quando o aplicativo cria uma definição de extensão do esquema, ele é marcado como proprietária da extensão do esquema.

O aplicativo proprietário pode mover a extensão pelos diferentes estados de um ciclo de vida, usando uma operação PATCH na propriedade **status**. Dependendo do estado atual, o aplicativo proprietário poderá atualizar ou excluir a extensão. Todas as atualizações para uma extensão de esquema devem ser sempre apenas aditivas e incondicionais.

|Estado |Comportamento de estado de ciclo de vida |
|:-------------|:------------|
| InDevelopment | <ul><li>Estado inicial após a criação. O aplicativo de proprietário ainda está desenvolvendo a extensão do esquema. </li><li>Nesse estado, qualquer aplicativo no mesmo diretório em que o aplicativo proprietário está registrado pode estender instâncias de recurso com essa definição de esquema (se o aplicativo tiver permissões para esse recurso). </li><li>Para um aplicativo proprietário multilocatário, somente a instância do aplicativo proprietário que está em um diretório diferente do diretório base pode estender instâncias de recurso com essa definição de esquema (se o aplicativo tiver permissões para esse recurso) ou ler os dados da extensão. </li><li>O aplicativo proprietário pode atualizar a definição de extensão com alterações aditivas. </li><li>Somente o aplicativo proprietário pode excluir a definição de extensão. </li><li>O aplicativo proprietário pode mover a extensão do esquema de **InDevelopment** para o estado **Disponível**.</li></ul> |
| Disponível | <ul><li>A extensão do esquema está disponível para ser usada por todos os aplicativos em qualquer locatário. </li><li>Depois que o aplicativo proprietário define **a** extensão como Disponível, qualquer aplicativo pode simplesmente adicionar dados personalizados a instâncias desses tipos de recursos especificados na extensão (se o aplicativo tiver permissões para esse recurso). O aplicativo pode atribuir dados personalizados ao criar uma nova instância ou atualizar uma instância existente. </li><li>O aplicativo proprietário pode atualizar a definição de extensão com alterações aditivas. Nenhum aplicativo pode excluir a definição de extensão nesse estado. </li><li>O proprietário do aplicativo pode mover a extensão do esquema de **Disponível** para o estado **Preterido**.</li></ul> |
| Preterido | <ul><li>A definição de extensão de esquema não pode ser lido nem modificada. </li><li>Nenhum aplicativo pode ler, atualizar, adicionar novas propriedades ou excluir a extensão. </li><li>No entanto, os aplicativos ainda podem ler, atualizar ou excluir _valores de propriedade_ de extensões existentes. </li></ul> |

> **Observação:** As definições de extensão de esquema (marcadas como `Available`) criadas por outros desenvolvedores de outros locatários são visíveis para todos os desenvolvedores (pela listagem de todas as extensões de esquema). Isto é diferente de outras APIs que retornam apenas os dados específicos do locatário. Por outro lado, os dados de extensão criados com base nas definições de extensão de esquema, são específicos do locatário e só podem ser acessados por aplicativos explicitamente autorizados. 

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

## <a name="see-also"></a>Confira também

+ [Adicionar propriedades personalizadas a recursos usando extensões](/graph/extensibility-overview)

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


