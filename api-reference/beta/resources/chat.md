---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7c365fd343af3078663cbd184b67b49feb37945c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193474"
---
# <a name="chat-resource-type"></a><span data-ttu-id="e3477-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="e3477-103">chat resource type</span></span>

<span data-ttu-id="e3477-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3477-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3477-105">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="e3477-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="e3477-106">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e3477-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="e3477-107">Methods</span><span class="sxs-lookup"><span data-stu-id="e3477-107">Methods</span></span>

|  <span data-ttu-id="e3477-108">Método</span><span class="sxs-lookup"><span data-stu-id="e3477-108">Method</span></span>       |  <span data-ttu-id="e3477-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e3477-109">Return Type</span></span>  | <span data-ttu-id="e3477-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3477-110">Description</span></span>| <span data-ttu-id="e3477-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="e3477-111">Permissions</span></span> |
|:---------------|:--------|:----------|-----------|
|[<span data-ttu-id="e3477-112">Listar chats</span><span class="sxs-lookup"><span data-stu-id="e3477-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="e3477-113">coleção [chat](chat.md)</span><span class="sxs-lookup"><span data-stu-id="e3477-113">[chat](chat.md) collection</span></span> | <span data-ttu-id="e3477-114">Obter a lista de chats de que um usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="e3477-114">Get the list of chats a user is part of.</span></span>| <span data-ttu-id="e3477-115">**Somente delegada**</span><span class="sxs-lookup"><span data-stu-id="e3477-115">**Delegated only**</span></span> |
|[<span data-ttu-id="e3477-116">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="e3477-116">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="e3477-117">chat</span><span class="sxs-lookup"><span data-stu-id="e3477-117">chat</span></span>](chat.md) | <span data-ttu-id="e3477-118">Leia as propriedades e as relações do chat.</span><span class="sxs-lookup"><span data-stu-id="e3477-118">Read properties and relationships of the chat.</span></span>| <span data-ttu-id="e3477-119">**Somente delegada**</span><span class="sxs-lookup"><span data-stu-id="e3477-119">**Delegated only**</span></span> |
|[<span data-ttu-id="e3477-120">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="e3477-120">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="e3477-121">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="e3477-121">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="e3477-122">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="e3477-122">Get the list of all users in the chat.</span></span>| <span data-ttu-id="e3477-123">Delegado e aplicativo \*</span><span class="sxs-lookup"><span data-stu-id="e3477-123">Delegated and application\*</span></span> |
|[<span data-ttu-id="e3477-124">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="e3477-124">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="e3477-125">conversationmember</span><span class="sxs-lookup"><span data-stu-id="e3477-125">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="e3477-126">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="e3477-126">Get a single user in the chat.</span></span>| <span data-ttu-id="e3477-127">Delegado e aplicativo \*</span><span class="sxs-lookup"><span data-stu-id="e3477-127">Delegated and application\*</span></span> |
|[<span data-ttu-id="e3477-128">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="e3477-128">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="e3477-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e3477-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="e3477-130">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="e3477-130">Get messages in a 1:1 or group chat.</span></span> | <span data-ttu-id="e3477-131">Delegado e aplicativo \*</span><span class="sxs-lookup"><span data-stu-id="e3477-131">Delegated and application\*</span></span> |
|[<span data-ttu-id="e3477-132">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="e3477-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="e3477-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e3477-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="e3477-134">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="e3477-134">Get a single message in a chat.</span></span> | <span data-ttu-id="e3477-135">Delegado e aplicativo \*</span><span class="sxs-lookup"><span data-stu-id="e3477-135">Delegated and application\*</span></span> |

<span data-ttu-id="e3477-136">\*> **Observação:** Ao usar permissões de aplicativo, certifique-se de saber como você vai obter a ID de chat.</span><span class="sxs-lookup"><span data-stu-id="e3477-136">\*> **Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="e3477-137">Como a lista de chats com permissões de aplicativo não é suportada, nem todos os cenários são possíveis.</span><span class="sxs-lookup"><span data-stu-id="e3477-137">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="e3477-138">É possível obter IDs de chat com permissões delegadas e de notificações de [alteração para o/chats/getAllMessages](../api/subscription-post-subscriptions.md) com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3477-138">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="e3477-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3477-139">Properties</span></span>

| <span data-ttu-id="e3477-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3477-140">Property</span></span>   | <span data-ttu-id="e3477-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3477-141">Type</span></span> |<span data-ttu-id="e3477-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3477-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e3477-143">id</span><span class="sxs-lookup"><span data-stu-id="e3477-143">id</span></span>| <span data-ttu-id="e3477-144">String</span><span class="sxs-lookup"><span data-stu-id="e3477-144">String</span></span>| <span data-ttu-id="e3477-145">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="e3477-145">The chat's unique identifier.</span></span> <span data-ttu-id="e3477-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e3477-146">Read-only.</span></span>|
| <span data-ttu-id="e3477-147">topic</span><span class="sxs-lookup"><span data-stu-id="e3477-147">topic</span></span>| <span data-ttu-id="e3477-148">String</span><span class="sxs-lookup"><span data-stu-id="e3477-148">String</span></span>|  <span data-ttu-id="e3477-149">Opcion Assunto ou tópico do chat.</span><span class="sxs-lookup"><span data-stu-id="e3477-149">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="e3477-150">Disponível apenas para bate-papos de grupo.</span><span class="sxs-lookup"><span data-stu-id="e3477-150">Only available for group chats.</span></span>|
| <span data-ttu-id="e3477-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3477-151">createdDateTime</span></span>| <span data-ttu-id="e3477-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3477-152">dateTimeOffset</span></span>|  <span data-ttu-id="e3477-153">Data e hora em que o chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="e3477-153">Date and time at which the chat was created.</span></span> <span data-ttu-id="e3477-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e3477-154">Read-only.</span></span>|
| <span data-ttu-id="e3477-155">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3477-155">lastUpdatedDateTime</span></span>| <span data-ttu-id="e3477-156">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3477-156">dateTimeOffset</span></span>|  <span data-ttu-id="e3477-157">Data e hora em que o chat foi renomeado ou a associação foi alterada.</span><span class="sxs-lookup"><span data-stu-id="e3477-157">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="e3477-158">lastUpdatedDateTime não é atualizado quando uma mensagem é enviada ao chat.</span><span class="sxs-lookup"><span data-stu-id="e3477-158">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="e3477-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e3477-159">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3477-160">Relações</span><span class="sxs-lookup"><span data-stu-id="e3477-160">Relationships</span></span>

| <span data-ttu-id="e3477-161">Relação</span><span class="sxs-lookup"><span data-stu-id="e3477-161">Relationship</span></span> | <span data-ttu-id="e3477-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3477-162">Type</span></span> |<span data-ttu-id="e3477-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3477-163">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e3477-164">installedApps</span><span class="sxs-lookup"><span data-stu-id="e3477-164">installedApps</span></span> | <span data-ttu-id="e3477-165">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="e3477-165">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="e3477-166">Uma coleção de todos os aplicativos no chat.</span><span class="sxs-lookup"><span data-stu-id="e3477-166">A collection of all the apps in the chat.</span></span> <span data-ttu-id="e3477-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e3477-167">Nullable.</span></span> |
| <span data-ttu-id="e3477-168">members</span><span class="sxs-lookup"><span data-stu-id="e3477-168">members</span></span> | <span data-ttu-id="e3477-169">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="e3477-169">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="e3477-170">Uma coleção de todas as pessoas no chat.</span><span class="sxs-lookup"><span data-stu-id="e3477-170">A collection of all people in the chat.</span></span> <span data-ttu-id="e3477-171">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e3477-171">Nullable.</span></span> |
| <span data-ttu-id="e3477-172">messages</span><span class="sxs-lookup"><span data-stu-id="e3477-172">messages</span></span> | <span data-ttu-id="e3477-173">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="e3477-173">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="e3477-174">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="e3477-174">A collection of all the messages in the chat.</span></span> <span data-ttu-id="e3477-175">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e3477-175">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e3477-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3477-176">JSON representation</span></span>

<span data-ttu-id="e3477-177">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3477-177">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="e3477-178">Confira também</span><span class="sxs-lookup"><span data-stu-id="e3477-178">See also</span></span>

- [<span data-ttu-id="e3477-179">channel</span><span class="sxs-lookup"><span data-stu-id="e3477-179">channel</span></span>](channel.md)
- [<span data-ttu-id="e3477-180">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e3477-180">chatMessage</span></span>](chatmessage.md)

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


