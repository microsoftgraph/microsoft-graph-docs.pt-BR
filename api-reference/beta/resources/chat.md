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
# <a name="chat-resource-type"></a><span data-ttu-id="7194a-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="7194a-103">chat resource type</span></span>

<span data-ttu-id="7194a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7194a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7194a-105">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="7194a-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="7194a-106">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="7194a-106">Participants can be users or apps.</span></span>

> <span data-ttu-id="7194a-107">**Observação**: se o chat estiver associado a uma instância do [onlineMeeting](../resources/onlinemeeting.md) , alguns dos métodos listados afetarão transitivamente a reunião.</span><span class="sxs-lookup"><span data-stu-id="7194a-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then some of the listed methods will transitively impact the meeting.</span></span>

## <a name="methods"></a><span data-ttu-id="7194a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7194a-108">Methods</span></span>

|  <span data-ttu-id="7194a-109">Método</span><span class="sxs-lookup"><span data-stu-id="7194a-109">Method</span></span>       |  <span data-ttu-id="7194a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7194a-110">Return Type</span></span>  | <span data-ttu-id="7194a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7194a-111">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="7194a-112">Listar chats</span><span class="sxs-lookup"><span data-stu-id="7194a-112">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="7194a-113">coleção [chat](chat.md)</span><span class="sxs-lookup"><span data-stu-id="7194a-113">[chat](chat.md) collection</span></span> | <span data-ttu-id="7194a-114">Obter a lista de chats de que um usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="7194a-114">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="7194a-115">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="7194a-115">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="7194a-116">chat</span><span class="sxs-lookup"><span data-stu-id="7194a-116">chat</span></span>](chat.md) | <span data-ttu-id="7194a-117">Leia as propriedades e as relações do chat.</span><span class="sxs-lookup"><span data-stu-id="7194a-117">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="7194a-118">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="7194a-118">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="7194a-119">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="7194a-119">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="7194a-120">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="7194a-120">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="7194a-121">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="7194a-121">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="7194a-122">conversationMember</span><span class="sxs-lookup"><span data-stu-id="7194a-122">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="7194a-123">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="7194a-123">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="7194a-124">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="7194a-124">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="7194a-125">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7194a-125">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="7194a-126">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="7194a-126">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="7194a-127">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="7194a-127">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="7194a-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7194a-128">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="7194a-129">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="7194a-129">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="7194a-130">Obter chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="7194a-130">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="7194a-131">chat</span><span class="sxs-lookup"><span data-stu-id="7194a-131">chat</span></span>](chat.md)| <span data-ttu-id="7194a-132">Obter um chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="7194a-132">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="7194a-133">Obter todas as mensagens de chat</span><span class="sxs-lookup"><span data-stu-id="7194a-133">Get all chat messages</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="7194a-134">coleção [chat](chat.md)</span><span class="sxs-lookup"><span data-stu-id="7194a-134">[chat](chat.md) collection</span></span>| <span data-ttu-id="7194a-135">Obter mensagens de todos os chats dos quais um usuário é um participante, incluindo chats de um a um, chats de grupo e bate-papos de reunião.</span><span class="sxs-lookup"><span data-stu-id="7194a-135">Get messages from all chats that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span> |
|[<span data-ttu-id="7194a-136">Listar aplicativos no chat</span><span class="sxs-lookup"><span data-stu-id="7194a-136">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="7194a-137">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="7194a-137">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="7194a-138">Listar aplicativos instalados em um chat (e uma reunião associada).</span><span class="sxs-lookup"><span data-stu-id="7194a-138">List apps installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="7194a-139">Obter aplicativo no chat</span><span class="sxs-lookup"><span data-stu-id="7194a-139">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="7194a-140">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7194a-140">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="7194a-141">Obter um aplicativo específico instalado em um chat (e uma reunião associada).</span><span class="sxs-lookup"><span data-stu-id="7194a-141">Get a specific app installed in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="7194a-142">Adicionar aplicativo ao chat</span><span class="sxs-lookup"><span data-stu-id="7194a-142">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="7194a-143">Adicionar (instalar) um aplicativo em um chat (e uma reunião associada).</span><span class="sxs-lookup"><span data-stu-id="7194a-143">Add (install) an app in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="7194a-144">Atualizar aplicativo no chat</span><span class="sxs-lookup"><span data-stu-id="7194a-144">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="7194a-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7194a-145">None</span></span> | <span data-ttu-id="7194a-146">Atualize para a versão mais recente do aplicativo instalado no chat (e na reunião associada).</span><span class="sxs-lookup"><span data-stu-id="7194a-146">Update to the latest version of the app installed in chat (and associated meeting).</span></span>|
|[<span data-ttu-id="7194a-147">Desinstalar o aplicativo do chat</span><span class="sxs-lookup"><span data-stu-id="7194a-147">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="7194a-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7194a-148">None</span></span> | <span data-ttu-id="7194a-149">Remover (desinstalar) o aplicativo de um chat (e uma reunião associada).</span><span class="sxs-lookup"><span data-stu-id="7194a-149">Remove (uninstall) app from a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="7194a-150">Guias de lista no chat</span><span class="sxs-lookup"><span data-stu-id="7194a-150">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="7194a-151">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7194a-151">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="7194a-152">Guias de lista fixadas para um chat (e reunião associada).</span><span class="sxs-lookup"><span data-stu-id="7194a-152">List tabs pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="7194a-153">Guia obter no chat</span><span class="sxs-lookup"><span data-stu-id="7194a-153">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="7194a-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7194a-154">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="7194a-155">Obtenha uma guia específica fixada para um chat (e reunião associada).</span><span class="sxs-lookup"><span data-stu-id="7194a-155">Get a specific tab pinned to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="7194a-156">Adicionar guia ao chat</span><span class="sxs-lookup"><span data-stu-id="7194a-156">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="7194a-157">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7194a-157">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="7194a-158">Adicionar (fixar) uma guia a um chat (e à reunião associada).</span><span class="sxs-lookup"><span data-stu-id="7194a-158">Add (pin) a tab to a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="7194a-159">Guia atualizar no chat</span><span class="sxs-lookup"><span data-stu-id="7194a-159">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="7194a-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7194a-160">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="7194a-161">Atualizar as propriedades de uma guia em um chat (e uma reunião associada).</span><span class="sxs-lookup"><span data-stu-id="7194a-161">Update the properties of a tab in a chat (and associated meeting).</span></span>|
|[<span data-ttu-id="7194a-162">Guia remover do chat</span><span class="sxs-lookup"><span data-stu-id="7194a-162">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="7194a-163">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7194a-163">None</span></span> | <span data-ttu-id="7194a-164">Remover (Desafixar) uma guia de um chat (e uma reunião associada).</span><span class="sxs-lookup"><span data-stu-id="7194a-164">Remove (unpin) a tab from a chat (and associated meeting).</span></span>|

><span data-ttu-id="7194a-165">**Observação:** Ao usar permissões de aplicativo, certifique-se de saber como você vai obter a ID de chat.</span><span class="sxs-lookup"><span data-stu-id="7194a-165">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="7194a-166">Como a lista de chats com permissões de aplicativo não é suportada, nem todos os cenários são possíveis.</span><span class="sxs-lookup"><span data-stu-id="7194a-166">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="7194a-167">É possível obter IDs de chat com permissões delegadas e de notificações de [alteração para o/chats/getAllMessages](../api/subscription-post-subscriptions.md) com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7194a-167">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="7194a-168">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7194a-168">Properties</span></span>

| <span data-ttu-id="7194a-169">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7194a-169">Property</span></span>   | <span data-ttu-id="7194a-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="7194a-170">Type</span></span> |<span data-ttu-id="7194a-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="7194a-171">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7194a-172">id</span><span class="sxs-lookup"><span data-stu-id="7194a-172">id</span></span>| <span data-ttu-id="7194a-173">String</span><span class="sxs-lookup"><span data-stu-id="7194a-173">String</span></span>| <span data-ttu-id="7194a-174">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="7194a-174">The chat's unique identifier.</span></span> <span data-ttu-id="7194a-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7194a-175">Read-only.</span></span>|
| <span data-ttu-id="7194a-176">topic</span><span class="sxs-lookup"><span data-stu-id="7194a-176">topic</span></span>| <span data-ttu-id="7194a-177">String</span><span class="sxs-lookup"><span data-stu-id="7194a-177">String</span></span>|  <span data-ttu-id="7194a-178">Opcion Assunto ou tópico do chat.</span><span class="sxs-lookup"><span data-stu-id="7194a-178">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="7194a-179">Disponível apenas para bate-papos de grupo.</span><span class="sxs-lookup"><span data-stu-id="7194a-179">Only available for group chats.</span></span>|
| <span data-ttu-id="7194a-180">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7194a-180">createdDateTime</span></span>| <span data-ttu-id="7194a-181">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7194a-181">dateTimeOffset</span></span>|  <span data-ttu-id="7194a-182">Data e hora em que o chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="7194a-182">Date and time at which the chat was created.</span></span> <span data-ttu-id="7194a-183">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7194a-183">Read-only.</span></span>|
| <span data-ttu-id="7194a-184">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7194a-184">lastUpdatedDateTime</span></span>| <span data-ttu-id="7194a-185">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7194a-185">dateTimeOffset</span></span>|  <span data-ttu-id="7194a-186">Data e hora em que o chat foi renomeado ou a associação foi alterada.</span><span class="sxs-lookup"><span data-stu-id="7194a-186">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="7194a-187">lastUpdatedDateTime não é atualizado quando uma mensagem é enviada ao chat.</span><span class="sxs-lookup"><span data-stu-id="7194a-187">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="7194a-188">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7194a-188">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7194a-189">Relações</span><span class="sxs-lookup"><span data-stu-id="7194a-189">Relationships</span></span>

| <span data-ttu-id="7194a-190">Relação</span><span class="sxs-lookup"><span data-stu-id="7194a-190">Relationship</span></span> | <span data-ttu-id="7194a-191">Tipo</span><span class="sxs-lookup"><span data-stu-id="7194a-191">Type</span></span> |<span data-ttu-id="7194a-192">Descrição</span><span class="sxs-lookup"><span data-stu-id="7194a-192">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7194a-193">installedApps</span><span class="sxs-lookup"><span data-stu-id="7194a-193">installedApps</span></span> | <span data-ttu-id="7194a-194">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="7194a-194">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="7194a-195">Uma coleção de todos os aplicativos no chat.</span><span class="sxs-lookup"><span data-stu-id="7194a-195">A collection of all the apps in the chat.</span></span> <span data-ttu-id="7194a-196">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7194a-196">Nullable.</span></span> |
| <span data-ttu-id="7194a-197">members</span><span class="sxs-lookup"><span data-stu-id="7194a-197">members</span></span> | <span data-ttu-id="7194a-198">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="7194a-198">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="7194a-199">Uma coleção de todas as pessoas no chat.</span><span class="sxs-lookup"><span data-stu-id="7194a-199">A collection of all people in the chat.</span></span> <span data-ttu-id="7194a-200">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7194a-200">Nullable.</span></span> |
| <span data-ttu-id="7194a-201">messages</span><span class="sxs-lookup"><span data-stu-id="7194a-201">messages</span></span> | <span data-ttu-id="7194a-202">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="7194a-202">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="7194a-203">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="7194a-203">A collection of all the messages in the chat.</span></span> <span data-ttu-id="7194a-204">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7194a-204">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7194a-205">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7194a-205">JSON representation</span></span>

<span data-ttu-id="7194a-206">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7194a-206">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7194a-207">Confira também</span><span class="sxs-lookup"><span data-stu-id="7194a-207">See also</span></span>

- [<span data-ttu-id="7194a-208">channel</span><span class="sxs-lookup"><span data-stu-id="7194a-208">channel</span></span>](channel.md)
- [<span data-ttu-id="7194a-209">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7194a-209">chatMessage</span></span>](chatmessage.md)

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


