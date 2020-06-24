---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 43ed088889a4b81d59cb9e1361ed978c9cb61141
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864200"
---
# <a name="chat-resource-type"></a><span data-ttu-id="688d9-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="688d9-103">chat resource type</span></span>

<span data-ttu-id="688d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="688d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="688d9-105">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="688d9-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="688d9-106">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="688d9-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="688d9-107">Methods</span><span class="sxs-lookup"><span data-stu-id="688d9-107">Methods</span></span>

|  <span data-ttu-id="688d9-108">Método</span><span class="sxs-lookup"><span data-stu-id="688d9-108">Method</span></span>       |  <span data-ttu-id="688d9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="688d9-109">Return Type</span></span>  | <span data-ttu-id="688d9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="688d9-110">Description</span></span>| <span data-ttu-id="688d9-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="688d9-111">Permissions</span></span> |
|:---------------|:--------|:----------|-----------|
|[<span data-ttu-id="688d9-112">Listar chats</span><span class="sxs-lookup"><span data-stu-id="688d9-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="688d9-113">coleção [chat](channel.md)</span><span class="sxs-lookup"><span data-stu-id="688d9-113">[chat](channel.md) collection</span></span> | <span data-ttu-id="688d9-114">Obter a lista de chats de que um usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="688d9-114">Get the list of chats a user is part of.</span></span>| <span data-ttu-id="688d9-115">**Somente delegada**</span><span class="sxs-lookup"><span data-stu-id="688d9-115">**Delegated only**</span></span> |
|[<span data-ttu-id="688d9-116">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="688d9-116">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="688d9-117">chat</span><span class="sxs-lookup"><span data-stu-id="688d9-117">chat</span></span>](channel.md) | <span data-ttu-id="688d9-118">Leia as propriedades e as relações do chat.</span><span class="sxs-lookup"><span data-stu-id="688d9-118">Read properties and relationships of the chat.</span></span>| <span data-ttu-id="688d9-119">**Somente delegada**</span><span class="sxs-lookup"><span data-stu-id="688d9-119">**Delegated only**</span></span> |
|[<span data-ttu-id="688d9-120">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="688d9-120">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="688d9-121">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="688d9-121">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="688d9-122">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="688d9-122">Get the list of all users in the chat.</span></span>| <span data-ttu-id="688d9-123">Delegado e aplicativo \*</span><span class="sxs-lookup"><span data-stu-id="688d9-123">Delegated and application\*</span></span> |
|[<span data-ttu-id="688d9-124">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="688d9-124">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="688d9-125">conversationmember</span><span class="sxs-lookup"><span data-stu-id="688d9-125">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="688d9-126">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="688d9-126">Get a single user in the chat.</span></span>| <span data-ttu-id="688d9-127">Delegado e aplicativo \*</span><span class="sxs-lookup"><span data-stu-id="688d9-127">Delegated and application\*</span></span> |
|[<span data-ttu-id="688d9-128">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="688d9-128">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="688d9-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="688d9-129">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="688d9-130">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="688d9-130">Get messages in a 1:1 or group chat.</span></span> | <span data-ttu-id="688d9-131">Delegado e aplicativo \*</span><span class="sxs-lookup"><span data-stu-id="688d9-131">Delegated and application\*</span></span> |
|[<span data-ttu-id="688d9-132">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="688d9-132">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="688d9-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="688d9-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="688d9-134">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="688d9-134">Get a single message in a chat.</span></span> | <span data-ttu-id="688d9-135">Delegado e aplicativo \*</span><span class="sxs-lookup"><span data-stu-id="688d9-135">Delegated and application\*</span></span> |

<span data-ttu-id="688d9-136">\*> **Observação:** Ao usar permissões de aplicativo, certifique-se de saber como você vai obter a ID de chat.</span><span class="sxs-lookup"><span data-stu-id="688d9-136">\*> **Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="688d9-137">Como a lista de chats com permissões de aplicativo não é suportada, nem todos os cenários são possíveis.</span><span class="sxs-lookup"><span data-stu-id="688d9-137">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="688d9-138">É possível obter IDs de chat com permissões delegadas e de notificações de [alteração para o/chats/allMessages](../api/subscription-post-subscriptions.md) com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="688d9-138">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/allMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="688d9-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="688d9-139">Properties</span></span>

| <span data-ttu-id="688d9-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="688d9-140">Property</span></span>   | <span data-ttu-id="688d9-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="688d9-141">Type</span></span> |<span data-ttu-id="688d9-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="688d9-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="688d9-143">id</span><span class="sxs-lookup"><span data-stu-id="688d9-143">id</span></span>| <span data-ttu-id="688d9-144">String</span><span class="sxs-lookup"><span data-stu-id="688d9-144">String</span></span>| <span data-ttu-id="688d9-145">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="688d9-145">The chat's unique identifier.</span></span> <span data-ttu-id="688d9-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="688d9-146">Read-only.</span></span>|
| <span data-ttu-id="688d9-147">topic</span><span class="sxs-lookup"><span data-stu-id="688d9-147">topic</span></span>| <span data-ttu-id="688d9-148">String</span><span class="sxs-lookup"><span data-stu-id="688d9-148">String</span></span>|  <span data-ttu-id="688d9-149">Opcion Assunto ou tópico do chat.</span><span class="sxs-lookup"><span data-stu-id="688d9-149">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="688d9-150">Disponível apenas para bate-papos de grupo.</span><span class="sxs-lookup"><span data-stu-id="688d9-150">Only available for group chats.</span></span>|
| <span data-ttu-id="688d9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="688d9-151">createdDateTime</span></span>| <span data-ttu-id="688d9-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="688d9-152">dateTimeOffset</span></span>|  <span data-ttu-id="688d9-153">Data e hora em que o chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="688d9-153">Date and time at which the chat was created.</span></span> <span data-ttu-id="688d9-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="688d9-154">Read-only.</span></span>|
| <span data-ttu-id="688d9-155">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="688d9-155">lastUpdatedDateTime</span></span>| <span data-ttu-id="688d9-156">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="688d9-156">dateTimeOffset</span></span>|  <span data-ttu-id="688d9-157">Data e hora em que o chat foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="688d9-157">Date and time at which the chat was updated.</span></span> <span data-ttu-id="688d9-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="688d9-158">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="688d9-159">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="688d9-159">Relationships</span></span>

| <span data-ttu-id="688d9-160">Relação</span><span class="sxs-lookup"><span data-stu-id="688d9-160">Relationship</span></span> | <span data-ttu-id="688d9-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="688d9-161">Type</span></span> |<span data-ttu-id="688d9-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="688d9-162">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="688d9-163">installedApps</span><span class="sxs-lookup"><span data-stu-id="688d9-163">installedApps</span></span> | <span data-ttu-id="688d9-164">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="688d9-164">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="688d9-165">Uma coleção de todos os aplicativos no chat.</span><span class="sxs-lookup"><span data-stu-id="688d9-165">A collection of all the apps in the chat.</span></span> <span data-ttu-id="688d9-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="688d9-166">Nullable.</span></span> |
| <span data-ttu-id="688d9-167">membros</span><span class="sxs-lookup"><span data-stu-id="688d9-167">members</span></span> | <span data-ttu-id="688d9-168">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="688d9-168">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="688d9-169">Uma coleção de todas as pessoas no chat.</span><span class="sxs-lookup"><span data-stu-id="688d9-169">A collection of all people in the chat.</span></span> <span data-ttu-id="688d9-170">Anulável.</span><span class="sxs-lookup"><span data-stu-id="688d9-170">Nullable.</span></span> |
| <span data-ttu-id="688d9-171">messages</span><span class="sxs-lookup"><span data-stu-id="688d9-171">messages</span></span> | <span data-ttu-id="688d9-172">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="688d9-172">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="688d9-173">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="688d9-173">A collection of all the messages in the chat.</span></span> <span data-ttu-id="688d9-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="688d9-174">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="688d9-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="688d9-175">JSON representation</span></span>

<span data-ttu-id="688d9-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="688d9-176">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="688d9-177">Confira também</span><span class="sxs-lookup"><span data-stu-id="688d9-177">See also</span></span>

- [<span data-ttu-id="688d9-178">channel</span><span class="sxs-lookup"><span data-stu-id="688d9-178">channel</span></span>](channel.md)
- [<span data-ttu-id="688d9-179">chatMessage</span><span class="sxs-lookup"><span data-stu-id="688d9-179">chatMessage</span></span>](chatmessage.md)

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
