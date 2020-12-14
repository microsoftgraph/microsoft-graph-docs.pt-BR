---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dcfa853f8ba246443f0f5073a4a62fd84f92adc6
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659405"
---
# <a name="chat-resource-type"></a>tipo de recurso chat

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes. Os participantes podem ser usuários ou aplicativos.

> **Observação**: se o chat estiver associado a uma instância do [onlineMeeting](../resources/onlinemeeting.md) , alguns dos métodos listados afetarão transitivamente a reunião.

## <a name="methods"></a>Métodos

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
|[Listar aplicativos no chat](../api/chat-list-installedapps.md) |Coleção [teamsAppInstallation](teamsappinstallation.md) | Listar aplicativos instalados em um chat (e uma reunião associada).|
|[Obter aplicativo no chat](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Obter um aplicativo específico instalado em um chat (e uma reunião associada).|
|[Adicionar aplicativo ao chat](../api/chat-post-installedapps.md) | | Adicionar (instalar) um aplicativo em um chat (e uma reunião associada).|
|[Atualizar aplicativo no chat](../api/chat-teamsappinstallation-upgrade.md) | Nenhum | Atualize para a versão mais recente do aplicativo instalado no chat (e na reunião associada).|
|[Desinstalar o aplicativo do chat](../api/chat-delete-installedapps.md) | Nenhum | Remover (desinstalar) o aplicativo de um chat (e uma reunião associada).|
|[Guias de lista no chat](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Guias de lista fixadas para um chat (e reunião associada).|
|[Guia obter no chat](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Obtenha uma guia específica fixada para um chat (e reunião associada).|
|[Adicionar guia ao chat](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Adicionar (fixar) uma guia a um chat (e à reunião associada).|
|[Guia atualizar no chat](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Atualizar as propriedades de uma guia em um chat (e uma reunião associada).|
|[Guia remover do chat](../api/chat-delete-tabs.md) | Nenhum | Remover (Desafixar) uma guia de um chat (e uma reunião associada).|

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


