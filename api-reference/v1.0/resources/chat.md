---
title: tipo de recurso de chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 724319be29968d0cbd74e21ed3fcaae63772e9e8
ms.sourcegitcommit: 6ae8c124fac63a195ccf516c9cff739f730b6b13
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2021
ms.locfileid: "60084060"
---
# <a name="chat-resource-type"></a>tipo de recurso de chat

Namespace: microsoft.graph

Um chat é uma coleção [de chatMessages](chatmessage.md) entre um ou mais participantes. Os participantes podem ser usuários ou aplicativos.

> **Observação**: se o chat estiver associado a uma instância [onlineMeeting,](../resources/onlinemeeting.md) alguns dos métodos listados afetarão transitivamente a reunião.

## <a name="methods"></a>Methods

|  Método       |  Tipo de retorno  | Descrição| 
|:---------------|:--------|:----------|
| **Gerenciamento de chat** |||
|[Criar chat](../api/chat-post.md) | [chat](chat.md) | Crie um novo chat.| 
|[Obter bate-papo](../api/chat-get.md) | [chat](chat.md) | Leia propriedades e relações do chat.| 
|[Atualizar chat](../api/chat-patch.md) | [chat](chat.md) | Atualize as propriedades do chat.|
|[Listar membros do bate-papo](../api/chat-list-members.md) | coleção [conversationMember](conversationmember.md) | Ver a lista de todos os usuários no bate-papo.| 
|[Adicionar membro do bate-papo](../api/chat-post-members.md) | Cabeçalho de local | Adicione um usuário ao chat.| 
|[Obter membro do bate-papo](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | Obter um único usuário no bate-papo.| 
|[Remover membro do bate-papo](../api/chat-delete-members.md)|Nenhum|Remova um usuário do chat.|
|[Obter chat entre o usuário e o aplicativo](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md)| Obter chat um-a-um entre o usuário e o aplicativo |
| **Mensagens** |||
|[Listar mensagens no chat](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Obter mensagens em um chat. | 
|[Receba uma mensagem no bate-papo](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | Receba uma única mensagem em um bate-papo. | 
|[Obter mensagens em todos os chats para o usuário](../api/chats-getallmessages.md)| [coleção chat](chat.md)| Obter mensagens de todos os chats nos quais um usuário é um participante. |
| **Aplicativos** |||
|[Listar aplicativos no chat](../api/chat-list-installedapps.md) |Coleção [teamsAppInstallation](teamsappinstallation.md) | Listar aplicativos instalados em um chat (e reunião associada).|
|[Obter aplicativo no chat](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Obter um aplicativo específico instalado em um chat (e reunião associada).|
|[Adicionar aplicativo no chat](../api/chat-post-installedapps.md) | | Adicionar (instalar) um aplicativo em um chat (e reunião associada).|
|[Atualizar aplicativo no chat](../api/chat-teamsappinstallation-upgrade.md) | Nenhum | Atualizar para a versão mais recente do aplicativo instalado no chat (e reunião associada).|
|[Desinstalar aplicativo do chat](../api/chat-delete-installedapps.md) | Nenhum | Remover (desinstalar) aplicativo de um chat (e reunião associada).|
| **Guias** |||
|[Listar guias no chat](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Listar guias fixadas em um chat (e reunião associada).|
|[Obter guia no chat](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Obter uma guia específica fixada em um chat (e reunião associada).|
|[Adicionar guia ao chat](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Adicione (pin) uma guia a um chat (e reunião associada).|
|[Guia Atualizar no chat](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Atualize as propriedades de uma guia em um chat (e reunião associada).|
|[Remover guia do chat](../api/chat-delete-tabs.md) | Nenhum | Remover (desempinar) uma guia de um chat (e reunião associada).|

>**Observação:** Ao usar permissões de aplicativo, certifique-se de saber como obter a ID do chat. Como não há suporte para listagem de chats com permissões de aplicativo, nem todos os cenários são possíveis. É possível obter IDs de chat com permissões delegadas e de notificações de alteração para [/chats/getAllMessages](../api/subscription-post-subscriptions.md) com permissões de aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
| id| Cadeia de caracteres| O identificador exclusivo do chat. Somente leitura.|
| topic| String|  (Opcional) Assunto ou tópico para o chat. Disponível apenas para chats em grupo.|
| createdDateTime| dateTimeOffset|  Data e hora em que o chat foi criado. Somente leitura.|
| lastUpdatedDateTime| dateTimeOffset|  Data e hora em que o chat foi renomeado ou a lista de membros foi alterada pela última vez. Somente leitura.|
| chatType| [chatType](../resources/chat.md#chattype-values) | Especifica o tipo de chat. Os valores possíveis são: `group` e `oneOnOne` `meeting` .|

### <a name="chattype-values"></a>valores chatType 

| Membro             | Valor | Descrição               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | Indica que o chat é um chat 1:1. O tamanho da lista é fixo para esse tipo de chat; os membros não podem ser removidos/adicionados.|
|group               | 1     | Indica que o chat é um chat em grupo. O tamanho da lista (de pelo menos duas pessoas) pode ser atualizado para esse tipo de chat. Os membros podem ser removidos/adicionados posteriormente.|
|meeting             | 2     | Indica que o chat está associado a uma reunião online. Esse tipo de chat só é criado como parte da criação de uma reunião online.|
|unknownFutureValue  | 3     | Valor sentinel para indicar valores futuros. |

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
| installedApps | Coleção [teamsAppInstallation](teamsappinstallation.md) | Uma coleção de todos os aplicativos no chat. Anulável. |
| members | coleção [conversationMember](conversationmember.md) | Uma coleção de todos os membros no chat. Anulável. |
| messages | [chatMessage](chatmessage.md) collection | Uma coleção de todas as mensagens no chat. Anulável. |

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
  "chatType": "String"
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


