---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f1745f987577d94f14f81d79a9f8afb89c1ab793
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606934"
---
# <a name="chat-resource-type"></a>tipo de recurso chat

Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes. Os participantes podem ser usuários ou aplicativos.

## <a name="methods"></a>Methods

|  Método       |  Tipo de retorno  | Descrição| 
|:---------------|:--------|:----------|
|[Listar chats](../api/chat-list.md) | coleção [chat](chat.md) | Obter a lista de chats de que um usuário faz parte.| 
|[Obter bate-papo](../api/chat-get.md) | [chat](chat.md) | Leia as propriedades e as relações do chat.| 
|[Listar membros de chat](../api/conversationmember-list.md) | coleção [conversationMember](conversationmember.md) | Ver a lista de todos os usuários no bate-papo.| 
|[Obter membro de chat](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | Obter um único usuário no bate-papo.| 
|[Listar mensagens em um bate-papo](../api/chat-list-message.md)  | [chatMessage](../resources/chatmessage.md) | Receba mensagens em um bate-papo de um para um ou de grupo. | 
|[Receba uma mensagem no bate-papo](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Receba uma única mensagem em um bate-papo. | 
|[Obter chat entre o usuário e o aplicativo](../api/userscopeteamsappinstallation-get-chat.md) | [chat](chat.md)| Obter um chat entre o usuário e o aplicativo |
|[Obter todas as mensagens de chat](../api/chats-getallmessages.md)| coleção [chat](chat.md)| Obter mensagens de todos os chats dos quais um usuário é um participante, incluindo chats de um a um, chats de grupo e bate-papos de reunião. |
|[Listar aplicativos no chat](../api/chat-list-installedapps.md) |Coleção [teamsAppInstallation](teamsappinstallation.md) | Listar aplicativos instalados em um chat.|
|[Obter aplicativo no chat](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Obtenha um aplicativo específico instalado em um chat.|
|[Adicionar aplicativo ao chat](../api/chat-post-installedapps.md) | | Adiciona (instala) um aplicativo em um chat.|
|[Atualizar aplicativo no chat](../api/chat-teamsappinstallation-upgrade.md) | Nenhum | Atualize para a versão mais recente do aplicativo instalado no chat.|
|[Desinstalar o aplicativo do chat](../api/chat-delete-installedapps.md) | Nenhum | Remova (desinstale) o aplicativo de um chat.|
|[Guias de lista no chat](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Listar guias fixadas a um chat.|
|[Guia obter no chat](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Obtenha uma guia específica fixada para um chat.|
|[Adicionar guia ao chat](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Adicionar (fixar) uma guia a um chat.|
|[Guia atualizar no chat](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Atualiza as propriedades de uma guia em um chat.|
|[Guia remover do chat](../api/chat-delete-tabs.md) | Nenhum | Remover (Desafixar) uma guia de um chat.|

>**Observação:** Ao usar permissões de aplicativo, certifique-se de saber como você vai obter a ID de chat. Como a lista de chats com permissões de aplicativo não é suportada, nem todos os cenários são possíveis. É possível obter IDs de chat com permissões delegadas e de notificações de [alteração para o/chats/getAllMessages](../api/subscription-post-subscriptions.md) com permissões de aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
| id| String| O identificador exclusivo do chat. Somente leitura.|
| topic| String|  Opcion Assunto ou tópico do chat. Disponível apenas para bate-papos de grupo.|
| createdDateTime| dateTimeOffset|  Data e hora em que o chat foi criado. Somente leitura.|
| lastUpdatedDateTime| dateTimeOffset|  Data e hora em que o chat foi renomeado ou a associação foi alterada. lastUpdatedDateTime não é atualizado quando uma mensagem é enviada ao chat. Somente leitura.|

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
| installedApps | Coleção [teamsAppInstallation](teamsappinstallation.md) | Uma coleção de todos os aplicativos no chat. Anulável. |
| members | coleção [conversationMember](conversationmember.md) | Uma coleção de todas as pessoas no chat. Anulável. |
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
  "lastUpdatedDateTime": "dateTimeOffset"
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


