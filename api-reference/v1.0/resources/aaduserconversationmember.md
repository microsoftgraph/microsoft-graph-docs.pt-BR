---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
ms.localizationpriority: high
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9aa64f0f6cfc6ea3571b0c2a1995c57644db4074
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007324"
---
# <a name="aaduserconversationmember-resource-type"></a>tipo de recurso aadUserConversationMember

Namespace: microsoft.graph

Representa um usuário do Azure Active Directory em uma [equipe](team.md), um [canal](channel.md), ou um [bate-papo](chat.md).
Esse tipo é herdado do [conversationMember](conversationmember.md).

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
|userId| cadeia de caracteres | O guid do usuário. |
|email| cadeia de caracteres  | O endereço de email do usuário. |
|tenantId| cadeia de caracteres  | TenantId para o qual o usuário do Azure AD pertence. |
|visibleHistoryStartDateTime| DateTimeOffset  | O carimbo de data/hora indicando quanto o histórico de uma conversa é compartilhado com o membro da conversa. Essa propriedade é configurável somente para os membros de um bate-papo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aadUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "string (identifier)",
  "displayName" : "string",
  "visibleHistoryStartDateTime": "string (timestamp)",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string",
  "tenantId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

