---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a8e4c94681065d9686e9f17888d3abf35885a65
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658039"
---
# <a name="conversationmember-resource-type"></a>tipo de recurso conversationMember

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um usuário em um [bate-papo](chat.md) ou [canal](channel.md).
Confira também [aadUserConversationMember](aaduserconversationmember.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar membros de chat](../api/conversationmember-list.md) | coleção [conversationMember](conversationmember.md) | Ver a lista de todos os usuários no bate-papo.|
|[Obter membro de chat](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | Obter um único usuário no bate-papo.|
|[Listar membros da equipe](../api/team-list-members.md)|coleção [conversationMember](../resources/conversationmember.md)|Obtenha a lista de membros nessa equipe.|
|[Obter membro da equipe](../api/team-get-members.md) | [conversationMember](conversationmember.md)coleção | Obtenha um membro na equipe.|
|[Adicionar membro da equipe](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|Adicione um novo membro à equipe.|
|[Adicionar membros da equipe em massa](../api/conversationmembers-add.md)|coleção [actionResultPart](../resources/actionresultpart.md)|Adicionar vários membros à equipe em uma única solicitação.|
|[Atualizar a função do membro da equipe](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|Alterar um membro para um proprietário ou voltar para um membro regular.|
|[Remover membro da equipe](../api/team-delete-members.md)|Nenhum|Remova um membro existente da equipe.|
|[Obter canal do membro](../api/channel-get-members.md) | [conversationMember](conversationmember.md) coleção | Obtenha um membro em um canal.|
|[Criar membro do canal](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | Adicionar um membro a um canal. Suportado só para o`channel`com MembershipType de.`private`|
|[Atualizar a função do membro do canal](../api/channel-update-members.md) | [conversationMember](conversationmember.md) | Atualize as propriedades de um membro do canal. Suportado só para o canal com MembershipType de`private`.|
|[Remover membro do canal](../api/channel-delete-members.md) | Nenhum | Exclua um membro de um canal. Suportado só com o `channelType` de `private`.|



## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID exclusivo do usuário.|
|displayName| cadeia de caracteres | O nome de exibição do usuário. |
|funções| coleção de cadeias de caracteres | As funções desse usuário. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


