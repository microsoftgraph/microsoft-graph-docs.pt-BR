---
title: tipo de recurso de chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f38b797c18c315e6053d285ce0c2485cd44218aa
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690004"
---
# <a name="chat-resource-type"></a>tipo de recurso de chat

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes. Os participantes podem ser usuários ou aplicativos.

> **Observação**: se o chat estiver associado a uma instância [onlineMeeting](../resources/onlinemeeting.md) , alguns dos métodos listados afetarão a reunião de forma transitiva.

## <a name="methods"></a>Métodos

|  Método       |  Tipo de retorno  | Descrição| 
|:---------------|:--------|:----------|
| **Gerenciamento de chat** |||
|[Listar chats](../api/chat-list.md) | [coleção de chat](chat.md) | Obtenha a lista de chats dos que um usuário faz parte.| 
|[Criar chat](../api/chat-post.md) | [chat](chat.md) | Crie um novo chat.| 
|[Obter bate-papo](../api/chat-get.md) | [chat](chat.md) | Leia as propriedades e as relações do chat.| 
|[Atualizar chat](../api/chat-patch.md) | [chat](chat.md) | Atualize as propriedades do chat.|
|[Listar membros do bate-papo](../api/chat-list-members.md) | coleção [conversationMember](conversationmember.md) | Ver a lista de todos os usuários no bate-papo.| 
|[Adicionar membro do bate-papo](../api/chat-post-members.md) | Cabeçalho de local | Adicione um usuário ao chat.| 
|[Obter membro do bate-papo](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | Obter um único usuário no bate-papo.| 
|[Remover membro do bate-papo](../api/chat-delete-members.md)|Nenhum|Remova um usuário do chat.|
|[Obter chat entre o usuário e o aplicativo](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md)| Obtenha um chat entre o usuário e o aplicativo.|
|[Marcar o chat como lido](../api/chat-markchatreadforuser.md) |Nenhum| Marque o chat como lido para um usuário.|
|[Marcar o chat como não lido](../api/chat-markchatunreadforuser.md) |Nenhum| Marque o chat como não lido para um usuário.|
|[Ocultar chat](../api/chat-hideforuser.md)|Nenhum|Ocultar um chat para um usuário.|
|[Reexibir chat](../api/chat-unhideforuser.md)|Nenhum|Reexibir um chat para um usuário.|
| **Mensagens** |||
|[Listar mensagens no chat](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Receba mensagens em um chat. | 
|[Receba uma mensagem no bate-papo](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | Receba uma única mensagem em um bate-papo. | 
|[Obter mensagens em todos os chats para o usuário](../api/chats-getallmessages.md)| [coleção de chat](chat.md)| Obter mensagens de todos os chats nos quais um usuário é um participante. |
| **Aplicativos** |||
|[Listar aplicativos no chat](../api/chat-list-installedapps.md) |Coleção [teamsAppInstallation](teamsappinstallation.md) | Listar aplicativos instalados em um chat (e reunião associada).|
|[Obter aplicativo no chat](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Obter um aplicativo específico instalado em um chat (e reunião associada).|
|[Adicionar aplicativo no chat](../api/chat-post-installedapps.md) | | Adicione (instale) um aplicativo em um chat (e reunião associada).|
|[Atualizar aplicativo no chat](../api/chat-teamsappinstallation-upgrade.md) | Nenhum | Atualize para a versão mais recente do aplicativo instalado no chat (e na reunião associada).|
|[Desinstalar o aplicativo do chat](../api/chat-delete-installedapps.md) | Nenhum | Remova (desinstale) o aplicativo de um chat (e uma reunião associada).|
|[Listar as concessões de permissões](../api/chat-list-permissiongrants.md) | Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Listar permissões que foram concedidas aos aplicativos neste chat.|
| **Guias** |||
|[Listar guias no chat](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Listar guias fixadas em um chat (e reunião associada).|
|[Guia Obter no chat](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Obtenha uma guia específica fixada em um chat (e reunião associada).|
|[Adicionar guia ao chat](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Adicione (fixe) uma guia a um chat (e reunião associada).|
|[Guia Atualizar no chat](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Atualize as propriedades de uma guia em um chat (e reunião associada).|
|[Remover guia do chat](../api/chat-delete-tabs.md) | Nenhum | Remova (desafixar) uma guia de um chat (e uma reunião associada).|
| **Operations** |||
|[Listar operações no chat](../api/chat-list-operations.md) | Coleção [teamsAsyncOperation](teamsAsyncOperation.md) | Obtenha a lista de operações assíncronas que foram executadas ou estão em execução no chat.|
|[Obter operação no chat](../api/teamsasyncoperation-get.md#example-get-operation-on-chat) | [teamsAsyncOperation](teamsAsyncOperation.md) | Obtenha uma única operação assíncrona que foi executada ou está em execução no chat.|
| **Mensagens fixadas** |||
|[Listar mensagens fixadas](../api/chat-list-pinnedmessages.md)|[Coleção pinnedChatMessageInfo](../resources/pinnedchatmessageinfo.md)|Obtenha uma lista de mensagens fixadas em um chat.|
|[Fixar uma mensagem](../api/chat-post-pinnedmessages.md)|[pinnedChatMessageInfo](../resources/pinnedchatmessageinfo.md)|Fixe uma mensagem de chat em um chat.|
|[Desafixar uma mensagem](../api/chat-delete-pinnedmessages.md)|Nenhum|Desafixar uma mensagem de um chat.|

>**Nota:** Ao usar permissões de aplicativo, certifique-se de saber como obter a ID de chat. Como não há suporte para a listagem de chats com permissões de aplicativo, nem todos os cenários são possíveis. É possível obter IDs de chat com permissões delegadas e de notificações de alteração para [/chats/getAllMessages](../api/subscription-post-subscriptions.md) com permissões de aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
| chatType| [chatType](../resources/chat.md#chattype-values) | Especifica o tipo de chat. Os valores possíveis são: `group`, `oneOnOne`, `meeting`, `unknownFutureValue`.|
| createdDateTime| dateTimeOffset|  Data e hora em que o chat foi criado. Somente leitura.|
| id| Cadeia de caracteres| O identificador exclusivo do chat. Somente leitura.|
| lastUpdatedDateTime| dateTimeOffset|  Data e hora em que o chat foi renomeado ou a lista de membros foi alterada pela última vez. Somente leitura.|
| onlineMeetingInfo | [teamworkOnlineMeetingInfo](../resources/teamworkonlinemeetinginfo.md) | Representa detalhes sobre uma reunião online. Se o chat não estiver associado a uma reunião online, a propriedade estará vazia. Somente leitura.|
| tenantId| String | O identificador do locatário no qual o chat foi criado. Somente leitura.|
| topic| String|  (Opcional) Assunto ou tópico para o chat. Disponível apenas para chats em grupo.|
| Vista|[chatViewpoint](../resources/chatviewpoint.md)|Representa informações específicas do chamador sobre o chat, como data e hora de leitura da última mensagem. Essa propriedade é preenchida somente quando a solicitação é feita em um contexto delegado.|
| webUrl| String | A URL do chat no Microsoft Teams. A URL deve ser tratada como um blob opaco e não analisada. Somente leitura.|


### <a name="chattype-values"></a>Valores chatType 

| Membro             | Valor | Descrição               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | Indica que o chat é um chat 1:1. O tamanho da lista de participantes é fixo para esse tipo de chat; membros não podem ser removidos/adicionados.|
|group               | 1     | Indica que o chat é um chat em grupo. O tamanho da lista de participação (de pelo menos duas pessoas) pode ser atualizado para esse tipo de chat. Os membros podem ser removidos/adicionados posteriormente.|
|Reunião             | 2     | Indica que o chat está associado a uma reunião online. Esse tipo de chat só é criado como parte da criação de uma reunião online.|
|unknownFutureValue  | 3     | Valor de sentinel de enumeração evolvável. Não usar. |

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
| installedApps | Coleção [teamsAppInstallation](teamsappinstallation.md) | Uma coleção de todos os aplicativos no chat. Anulável. |
| lastMessagePreview | [chatMessageInfo](chatmessageinfo.md)| Visualização da última mensagem enviada no chat. Nulo se nenhuma mensagem tiver sido enviada no chat. Atualmente, somente a operação [de chats](../api/chat-list.md) de lista dá suporte a essa propriedade.|
| members | coleção [conversationMember](conversationmember.md) | Uma coleção de todos os membros no chat. Anulável. |
| messages | [chatMessage](chatmessage.md) collection | Uma coleção de todas as mensagens no chat. Anulável. |
| operations | Coleção [teamsAsyncOperation](teamsasyncoperation.md) | Uma coleção de todas as operações assíncronas do Teams que foram executadas ou estão em execução no chat. Anulável. |
| permissionGrants| Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)| Uma coleção de permissões concedidas aos aplicativos para o chat.|
| pinnedMessages | [Coleção pinnedChatMessageInfo](pinnedchatmessageinfo.md) | Uma coleção de todas as mensagens fixadas no chat. Anulável. |
| guias | [teamsTab](teamstab.md) collection | Uma coleção de todas as guias no chat. Anulável. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
  "topic": "string",
  "createdDateTime": "dateTimeOffset",
  "lastUpdatedDateTime": "dateTimeOffset",
  "chatType": "string",
  "webUrl": "string",
  "tenantId": "string",
  "viewpoint": {
    "@odata.type": "microsoft.graph.chatViewpoint"
  },
  "onlineMeetingInfo": {
    "@odata.type": "microsoft.graph.teamworkOnlineMeetingInfo"
  }
}
```

## <a name="see-also"></a>Confira também

- [channel](channel.md)
- [chatMessage](chatmessage.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->


