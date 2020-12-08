---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 88d08c8e6e0222c339c99db9cab9243f9c48c1f3
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597253"
---
# <a name="chat-resource-type"></a><span data-ttu-id="4f35e-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="4f35e-103">chat resource type</span></span>

<span data-ttu-id="4f35e-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4f35e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f35e-105">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="4f35e-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="4f35e-106">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="4f35e-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="4f35e-107">Methods</span><span class="sxs-lookup"><span data-stu-id="4f35e-107">Methods</span></span>

|  <span data-ttu-id="4f35e-108">Método</span><span class="sxs-lookup"><span data-stu-id="4f35e-108">Method</span></span>       |  <span data-ttu-id="4f35e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4f35e-109">Return Type</span></span>  | <span data-ttu-id="4f35e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f35e-110">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="4f35e-111">Listar chats</span><span class="sxs-lookup"><span data-stu-id="4f35e-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="4f35e-112">coleção [chat](chat.md)</span><span class="sxs-lookup"><span data-stu-id="4f35e-112">[chat](chat.md) collection</span></span> | <span data-ttu-id="4f35e-113">Obter a lista de chats de que um usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="4f35e-113">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="4f35e-114">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="4f35e-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="4f35e-115">chat</span><span class="sxs-lookup"><span data-stu-id="4f35e-115">chat</span></span>](chat.md) | <span data-ttu-id="4f35e-116">Leia as propriedades e as relações do chat.</span><span class="sxs-lookup"><span data-stu-id="4f35e-116">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="4f35e-117">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="4f35e-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="4f35e-118">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="4f35e-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="4f35e-119">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="4f35e-119">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="4f35e-120">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="4f35e-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="4f35e-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="4f35e-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="4f35e-122">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="4f35e-122">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="4f35e-123">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="4f35e-123">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="4f35e-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4f35e-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4f35e-125">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="4f35e-125">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="4f35e-126">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="4f35e-126">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="4f35e-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4f35e-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4f35e-128">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="4f35e-128">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="4f35e-129">Obter chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f35e-129">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="4f35e-130">chat</span><span class="sxs-lookup"><span data-stu-id="4f35e-130">chat</span></span>](chat.md)| <span data-ttu-id="4f35e-131">Obter um chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f35e-131">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="4f35e-132">Obter todas as mensagens de chat</span><span class="sxs-lookup"><span data-stu-id="4f35e-132">Get all chat messages</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="4f35e-133">coleção [chat](chat.md)</span><span class="sxs-lookup"><span data-stu-id="4f35e-133">[chat](chat.md) collection</span></span>| <span data-ttu-id="4f35e-134">Obter mensagens de todos os chats dos quais um usuário é um participante, incluindo chats de um a um, chats de grupo e bate-papos de reunião.</span><span class="sxs-lookup"><span data-stu-id="4f35e-134">Get messages from all chats that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span> |

><span data-ttu-id="4f35e-135">**Observação:** Ao usar permissões de aplicativo, certifique-se de saber como você vai obter a ID de chat.</span><span class="sxs-lookup"><span data-stu-id="4f35e-135">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="4f35e-136">Como a lista de chats com permissões de aplicativo não é suportada, nem todos os cenários são possíveis.</span><span class="sxs-lookup"><span data-stu-id="4f35e-136">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="4f35e-137">É possível obter IDs de chat com permissões delegadas e de notificações de [alteração para o/chats/getAllMessages](../api/subscription-post-subscriptions.md) com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f35e-137">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="4f35e-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f35e-138">Properties</span></span>

| <span data-ttu-id="4f35e-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f35e-139">Property</span></span>   | <span data-ttu-id="4f35e-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f35e-140">Type</span></span> |<span data-ttu-id="4f35e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f35e-141">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4f35e-142">id</span><span class="sxs-lookup"><span data-stu-id="4f35e-142">id</span></span>| <span data-ttu-id="4f35e-143">String</span><span class="sxs-lookup"><span data-stu-id="4f35e-143">String</span></span>| <span data-ttu-id="4f35e-144">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="4f35e-144">The chat's unique identifier.</span></span> <span data-ttu-id="4f35e-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4f35e-145">Read-only.</span></span>|
| <span data-ttu-id="4f35e-146">topic</span><span class="sxs-lookup"><span data-stu-id="4f35e-146">topic</span></span>| <span data-ttu-id="4f35e-147">String</span><span class="sxs-lookup"><span data-stu-id="4f35e-147">String</span></span>|  <span data-ttu-id="4f35e-148">Opcion Assunto ou tópico do chat.</span><span class="sxs-lookup"><span data-stu-id="4f35e-148">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="4f35e-149">Disponível apenas para bate-papos de grupo.</span><span class="sxs-lookup"><span data-stu-id="4f35e-149">Only available for group chats.</span></span>|
| <span data-ttu-id="4f35e-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f35e-150">createdDateTime</span></span>| <span data-ttu-id="4f35e-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f35e-151">dateTimeOffset</span></span>|  <span data-ttu-id="4f35e-152">Data e hora em que o chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="4f35e-152">Date and time at which the chat was created.</span></span> <span data-ttu-id="4f35e-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4f35e-153">Read-only.</span></span>|
| <span data-ttu-id="4f35e-154">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f35e-154">lastUpdatedDateTime</span></span>| <span data-ttu-id="4f35e-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f35e-155">dateTimeOffset</span></span>|  <span data-ttu-id="4f35e-156">Data e hora em que o chat foi renomeado ou a associação foi alterada.</span><span class="sxs-lookup"><span data-stu-id="4f35e-156">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="4f35e-157">lastUpdatedDateTime não é atualizado quando uma mensagem é enviada ao chat.</span><span class="sxs-lookup"><span data-stu-id="4f35e-157">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="4f35e-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4f35e-158">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f35e-159">Relações</span><span class="sxs-lookup"><span data-stu-id="4f35e-159">Relationships</span></span>

| <span data-ttu-id="4f35e-160">Relação</span><span class="sxs-lookup"><span data-stu-id="4f35e-160">Relationship</span></span> | <span data-ttu-id="4f35e-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f35e-161">Type</span></span> |<span data-ttu-id="4f35e-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f35e-162">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4f35e-163">installedApps</span><span class="sxs-lookup"><span data-stu-id="4f35e-163">installedApps</span></span> | <span data-ttu-id="4f35e-164">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="4f35e-164">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="4f35e-165">Uma coleção de todos os aplicativos no chat.</span><span class="sxs-lookup"><span data-stu-id="4f35e-165">A collection of all the apps in the chat.</span></span> <span data-ttu-id="4f35e-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4f35e-166">Nullable.</span></span> |
| <span data-ttu-id="4f35e-167">members</span><span class="sxs-lookup"><span data-stu-id="4f35e-167">members</span></span> | <span data-ttu-id="4f35e-168">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="4f35e-168">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="4f35e-169">Uma coleção de todas as pessoas no chat.</span><span class="sxs-lookup"><span data-stu-id="4f35e-169">A collection of all people in the chat.</span></span> <span data-ttu-id="4f35e-170">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4f35e-170">Nullable.</span></span> |
| <span data-ttu-id="4f35e-171">messages</span><span class="sxs-lookup"><span data-stu-id="4f35e-171">messages</span></span> | <span data-ttu-id="4f35e-172">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f35e-172">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="4f35e-173">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="4f35e-173">A collection of all the messages in the chat.</span></span> <span data-ttu-id="4f35e-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4f35e-174">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f35e-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f35e-175">JSON representation</span></span>

<span data-ttu-id="4f35e-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4f35e-176">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="4f35e-177">Confira também</span><span class="sxs-lookup"><span data-stu-id="4f35e-177">See also</span></span>

- [<span data-ttu-id="4f35e-178">channel</span><span class="sxs-lookup"><span data-stu-id="4f35e-178">channel</span></span>](channel.md)
- [<span data-ttu-id="4f35e-179">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4f35e-179">chatMessage</span></span>](chatmessage.md)

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


