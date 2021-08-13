---
title: tipo de recurso conversationMember
description: Representa o usuário em uma conversa.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 73d7e7526c870887edbade4555b3a699e458183f3b3753176574448525997105
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155166"
---
# <a name="conversationmember-resource-type"></a>tipo de recurso conversationMember

Namespace: microsoft.graph

Representa um usuário em uma [equipe,](team.md)um [canal](channel.md)ou [um chat.](chat.md)
Consulte também [aadUserConversationMember](aaduserconversationmember.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar membros de equipe](../api/team-list-members.md)|coleção [conversationMember](../resources/conversationmember.md)|Obtenha a lista de membros nessa equipe.|
|[Adicionar membro à equipe](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|Adicione um novo membro à equipe.|
|[Obter membro da equipe](../api/team-get-members.md) | [conversationMember](conversationmember.md)coleção | Obtenha um membro na equipe.|
|[Atualizar a função do membro](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|Alterar um membro para um proprietário ou voltar para um membro regular.|
|[Remover membro da equipe](../api/team-delete-members.md)|Nenhum|Remova um membro existente da equipe.|
|[Listar membros do canal](../api/channel-list-members.md) | coleção [conversationMember](conversationmember.md) | Obter a lista de todos os membros em um canal.|
|[Adicionar membro do canal](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | Adicionar um membro a um canal. Somente suportado para `channel` com o membershipType de `private`.|
|[Obter canal do membro](../api/channel-get-members.md) | coleção [conversationMember](conversationmember.md) | Obtenha um membro em um canal.|
|[Atualizar a função do membro do canal](../api/channel-update-members.md) | [conversationMember](conversationmember.md) | Atualize as propriedades de um membro do canal. Suportado só para o canal com MembershipType de`private`.|
|[Remover membro do canal](../api/channel-delete-members.md) | Nenhum | Exclua um membro de um canal. Suportado só com o `channelType` de `private`.|
|[Listar membros do bate-papo](../api/chat-list-members.md) | coleção [conversationMember](conversationmember.md) | Obter a lista de todos os membros em um chat.|
|[Adicionar membro do bate-papo](../api/chat-post-members.md) | Cabeçalho de local | Adicionar um membro a um bate-papo.| 
|[Obter membro do bate-papo](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | Obtenha um membro em um chat.|
|[Remover membro do bate-papo](../api/chat-delete-members.md) | Nenhum | Remover um membro de um bate-papo.| 

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID exclusiva do usuário.|
|displayName| cadeia de caracteres | O nome de exibição do usuário. |
|funções| coleção de cadeias de caracteres | As funções desse usuário. |
|visibleHistoryStartDateTime| DateTimeOffset | O carimbo de data/hora indicando quanto o histórico de uma conversa é compartilhado com o membro da conversa. Essa propriedade é configurável somente para os membros de um bate-papo. |

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

