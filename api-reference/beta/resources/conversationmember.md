---
title: tipo de recurso conversationMember
description: Representa um usuário em uma conversa.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f6b24b65a6ae25f8a05bf067659c04d49c06d24
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706055"
---
# <a name="conversationmember-resource-type"></a>tipo de recurso conversationMember

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um usuário em um [bate-papo](chat.md) ou [canal](channel.md).
Confira também [aadUserConversationMember](aaduserconversationmember.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar membros da equipe](../api/team-list-members.md)|coleção [conversationMember](../resources/conversationmember.md)|Obtenha a lista de membros nessa equipe.|
|[Obter membro da equipe](../api/team-get-members.md) | [conversationMember](conversationmember.md)coleção | Obtenha um membro na equipe.|
|[Adicionar membro da equipe](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|Adicione um novo membro à equipe.|
|[Adicionar membros da equipe em massa](../api/conversationmembers-add.md)|coleção[actionResultPart](../resources/actionresultpart.md)|Adicione vários membros à equipe em uma única solicitação.|
|[Atualizar a função do membro da equipe](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|Alterar um membro para um proprietário ou voltar para um membro regular.|
|[Remover membro da equipe](../api/team-delete-members.md)|Nenhum|Remova um membro existente da equipe.|
|[Listar membros do canal](../api/channel-list-members.md) | coleção [conversationMember](conversationmember.md) | Obter a lista de todos os membros em um canal.|
|[Obter canal do membro](../api/channel-get-members.md) | coleção [conversationMember](conversationmember.md) | Obtenha um membro em um canal.|
|[Criar membro do canal](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | Adicionar um membro a um canal. Suportado só para o`channel`com MembershipType de.`private`|
|[Atualizar a função do membro do canal](../api/channel-update-members.md) | [conversationMember](conversationmember.md) | Atualize as propriedades de um membro do canal. Suportado só para o canal com MembershipType de`private`.|
|[Remover membro do canal](../api/channel-delete-members.md) | Nenhum | Exclua um membro de um canal. Suportado só com o `channelType` de `private`.|
|[Listar membros de chat](../api/chat-list-members.md) | coleção [conversationMember](conversationmember.md) | Obter a lista de todos os membros em um chat.|
|[Obter membro de chat](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | Obter um membro em um chat.|
|[Adicionar membro de chat](../api/chat-post-members.md) | Cabeçalho location | Adicionar um membro a um chat.| 

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID exclusivo do usuário.|
|displayName| cadeia de caracteres | O nome de exibição do usuário. |
|funções| coleção de cadeias de caracteres | As funções desse usuário. |
|visibleHistoryStartDateTime| DateTimeOffset | O carimbo de data/hora que indica o quanto o histórico de uma conversa é compartilhado com o membro da conversa. Essa propriedade é configurável somente para os membros de um chat. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)"
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


