---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e6316f7c3aad0fc90e258d145b57942395265ce7
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563447"
---
# <a name="chat-resource-type"></a><span data-ttu-id="42d97-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="42d97-103">chat resource type</span></span>

<span data-ttu-id="42d97-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42d97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42d97-105">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="42d97-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="42d97-106">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="42d97-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="42d97-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="42d97-107">Methods</span></span>

|  <span data-ttu-id="42d97-108">Método</span><span class="sxs-lookup"><span data-stu-id="42d97-108">Method</span></span>       |  <span data-ttu-id="42d97-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="42d97-109">Return Type</span></span>  | <span data-ttu-id="42d97-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="42d97-110">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="42d97-111">Listar chats</span><span class="sxs-lookup"><span data-stu-id="42d97-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="42d97-112">coleção [chat](chat.md)</span><span class="sxs-lookup"><span data-stu-id="42d97-112">[chat](chat.md) collection</span></span> | <span data-ttu-id="42d97-113">Obter a lista de chats de que um usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="42d97-113">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="42d97-114">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="42d97-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="42d97-115">chat</span><span class="sxs-lookup"><span data-stu-id="42d97-115">chat</span></span>](chat.md) | <span data-ttu-id="42d97-116">Leia as propriedades e as relações do chat.</span><span class="sxs-lookup"><span data-stu-id="42d97-116">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="42d97-117">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="42d97-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="42d97-118">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="42d97-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="42d97-119">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="42d97-119">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="42d97-120">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="42d97-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="42d97-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="42d97-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="42d97-122">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="42d97-122">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="42d97-123">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="42d97-123">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="42d97-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="42d97-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="42d97-125">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="42d97-125">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="42d97-126">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="42d97-126">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="42d97-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="42d97-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="42d97-128">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="42d97-128">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="42d97-129">Obter chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="42d97-129">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="42d97-130">chat</span><span class="sxs-lookup"><span data-stu-id="42d97-130">chat</span></span>](chat.md)| <span data-ttu-id="42d97-131">Obter um chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="42d97-131">Get one-on-one chat between user and the app</span></span> |

><span data-ttu-id="42d97-132">**Observação:** Ao usar permissões de aplicativo, certifique-se de saber como você vai obter a ID de chat.</span><span class="sxs-lookup"><span data-stu-id="42d97-132">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="42d97-133">Como a lista de chats com permissões de aplicativo não é suportada, nem todos os cenários são possíveis.</span><span class="sxs-lookup"><span data-stu-id="42d97-133">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="42d97-134">É possível obter IDs de chat com permissões delegadas e de notificações de [alteração para o/chats/getAllMessages](../api/subscription-post-subscriptions.md) com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42d97-134">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="42d97-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42d97-135">Properties</span></span>

| <span data-ttu-id="42d97-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42d97-136">Property</span></span>   | <span data-ttu-id="42d97-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="42d97-137">Type</span></span> |<span data-ttu-id="42d97-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="42d97-138">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42d97-139">id</span><span class="sxs-lookup"><span data-stu-id="42d97-139">id</span></span>| <span data-ttu-id="42d97-140">String</span><span class="sxs-lookup"><span data-stu-id="42d97-140">String</span></span>| <span data-ttu-id="42d97-141">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="42d97-141">The chat's unique identifier.</span></span> <span data-ttu-id="42d97-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42d97-142">Read-only.</span></span>|
| <span data-ttu-id="42d97-143">topic</span><span class="sxs-lookup"><span data-stu-id="42d97-143">topic</span></span>| <span data-ttu-id="42d97-144">String</span><span class="sxs-lookup"><span data-stu-id="42d97-144">String</span></span>|  <span data-ttu-id="42d97-145">Opcion Assunto ou tópico do chat.</span><span class="sxs-lookup"><span data-stu-id="42d97-145">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="42d97-146">Disponível apenas para bate-papos de grupo.</span><span class="sxs-lookup"><span data-stu-id="42d97-146">Only available for group chats.</span></span>|
| <span data-ttu-id="42d97-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42d97-147">createdDateTime</span></span>| <span data-ttu-id="42d97-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42d97-148">dateTimeOffset</span></span>|  <span data-ttu-id="42d97-149">Data e hora em que o chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="42d97-149">Date and time at which the chat was created.</span></span> <span data-ttu-id="42d97-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42d97-150">Read-only.</span></span>|
| <span data-ttu-id="42d97-151">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="42d97-151">lastUpdatedDateTime</span></span>| <span data-ttu-id="42d97-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42d97-152">dateTimeOffset</span></span>|  <span data-ttu-id="42d97-153">Data e hora em que o chat foi renomeado ou a associação foi alterada.</span><span class="sxs-lookup"><span data-stu-id="42d97-153">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="42d97-154">lastUpdatedDateTime não é atualizado quando uma mensagem é enviada ao chat.</span><span class="sxs-lookup"><span data-stu-id="42d97-154">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="42d97-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42d97-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42d97-156">Relações</span><span class="sxs-lookup"><span data-stu-id="42d97-156">Relationships</span></span>

| <span data-ttu-id="42d97-157">Relação</span><span class="sxs-lookup"><span data-stu-id="42d97-157">Relationship</span></span> | <span data-ttu-id="42d97-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="42d97-158">Type</span></span> |<span data-ttu-id="42d97-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="42d97-159">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42d97-160">installedApps</span><span class="sxs-lookup"><span data-stu-id="42d97-160">installedApps</span></span> | <span data-ttu-id="42d97-161">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="42d97-161">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="42d97-162">Uma coleção de todos os aplicativos no chat.</span><span class="sxs-lookup"><span data-stu-id="42d97-162">A collection of all the apps in the chat.</span></span> <span data-ttu-id="42d97-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="42d97-163">Nullable.</span></span> |
| <span data-ttu-id="42d97-164">members</span><span class="sxs-lookup"><span data-stu-id="42d97-164">members</span></span> | <span data-ttu-id="42d97-165">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="42d97-165">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="42d97-166">Uma coleção de todas as pessoas no chat.</span><span class="sxs-lookup"><span data-stu-id="42d97-166">A collection of all people in the chat.</span></span> <span data-ttu-id="42d97-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="42d97-167">Nullable.</span></span> |
| <span data-ttu-id="42d97-168">messages</span><span class="sxs-lookup"><span data-stu-id="42d97-168">messages</span></span> | <span data-ttu-id="42d97-169">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="42d97-169">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="42d97-170">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="42d97-170">A collection of all the messages in the chat.</span></span> <span data-ttu-id="42d97-171">Anulável.</span><span class="sxs-lookup"><span data-stu-id="42d97-171">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42d97-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42d97-172">JSON representation</span></span>

<span data-ttu-id="42d97-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42d97-173">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="42d97-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="42d97-174">See also</span></span>

- [<span data-ttu-id="42d97-175">channel</span><span class="sxs-lookup"><span data-stu-id="42d97-175">channel</span></span>](channel.md)
- [<span data-ttu-id="42d97-176">chatMessage</span><span class="sxs-lookup"><span data-stu-id="42d97-176">chatMessage</span></span>](chatmessage.md)

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


