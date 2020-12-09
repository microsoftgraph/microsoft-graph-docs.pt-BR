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
# <a name="chat-resource-type"></a><span data-ttu-id="e5d0f-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-103">chat resource type</span></span>

<span data-ttu-id="e5d0f-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e5d0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5d0f-105">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="e5d0f-106">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="e5d0f-107">Methods</span><span class="sxs-lookup"><span data-stu-id="e5d0f-107">Methods</span></span>

|  <span data-ttu-id="e5d0f-108">Método</span><span class="sxs-lookup"><span data-stu-id="e5d0f-108">Method</span></span>       |  <span data-ttu-id="e5d0f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e5d0f-109">Return Type</span></span>  | <span data-ttu-id="e5d0f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5d0f-110">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5d0f-111">Listar chats</span><span class="sxs-lookup"><span data-stu-id="e5d0f-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="e5d0f-112">coleção [chat](chat.md)</span><span class="sxs-lookup"><span data-stu-id="e5d0f-112">[chat](chat.md) collection</span></span> | <span data-ttu-id="e5d0f-113">Obter a lista de chats de que um usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-113">Get the list of chats a user is part of.</span></span>| 
|[<span data-ttu-id="e5d0f-114">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="e5d0f-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="e5d0f-115">chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-115">chat</span></span>](chat.md) | <span data-ttu-id="e5d0f-116">Leia as propriedades e as relações do chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-116">Read properties and relationships of the chat.</span></span>| 
|[<span data-ttu-id="e5d0f-117">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="e5d0f-118">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="e5d0f-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="e5d0f-119">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-119">Get the list of all users in the chat.</span></span>| 
|[<span data-ttu-id="e5d0f-120">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="e5d0f-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="e5d0f-121">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="e5d0f-122">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-122">Get a single user in the chat.</span></span>| 
|[<span data-ttu-id="e5d0f-123">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="e5d0f-123">List messages in a chat</span></span>](../api/chat-list-message.md)  | [<span data-ttu-id="e5d0f-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e5d0f-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="e5d0f-125">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-125">Get messages in a 1:1 or group chat.</span></span> | 
|[<span data-ttu-id="e5d0f-126">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="e5d0f-126">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="e5d0f-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e5d0f-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="e5d0f-128">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-128">Get a single message in a chat.</span></span> | 
|[<span data-ttu-id="e5d0f-129">Obter chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5d0f-129">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="e5d0f-130">chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-130">chat</span></span>](chat.md)| <span data-ttu-id="e5d0f-131">Obter um chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5d0f-131">Get one-on-one chat between user and the app</span></span> |
|[<span data-ttu-id="e5d0f-132">Obter todas as mensagens de chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-132">Get all chat messages</span></span>](../api/chats-getallmessages.md)| <span data-ttu-id="e5d0f-133">coleção [chat](chat.md)</span><span class="sxs-lookup"><span data-stu-id="e5d0f-133">[chat](chat.md) collection</span></span>| <span data-ttu-id="e5d0f-134">Obter mensagens de todos os chats dos quais um usuário é um participante, incluindo chats de um a um, chats de grupo e bate-papos de reunião.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-134">Get messages from all chats that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span> |
|[<span data-ttu-id="e5d0f-135">Listar aplicativos no chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-135">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="e5d0f-136">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="e5d0f-136">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="e5d0f-137">Listar aplicativos instalados em um chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-137">List apps installed in a chat.</span></span>|
|[<span data-ttu-id="e5d0f-138">Obter aplicativo no chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-138">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="e5d0f-139">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e5d0f-139">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="e5d0f-140">Obtenha um aplicativo específico instalado em um chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-140">Get a specific app installed in a chat.</span></span>|
|[<span data-ttu-id="e5d0f-141">Adicionar aplicativo ao chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-141">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="e5d0f-142">Adiciona (instala) um aplicativo em um chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-142">Adds (installs) an app in a chat.</span></span>|
|[<span data-ttu-id="e5d0f-143">Atualizar aplicativo no chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-143">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="e5d0f-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5d0f-144">None</span></span> | <span data-ttu-id="e5d0f-145">Atualize para a versão mais recente do aplicativo instalado no chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-145">Update to the latest version of the app installed in chat.</span></span>|
|[<span data-ttu-id="e5d0f-146">Desinstalar o aplicativo do chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-146">Uninstall app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="e5d0f-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5d0f-147">None</span></span> | <span data-ttu-id="e5d0f-148">Remova (desinstale) o aplicativo de um chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-148">Remove (uninstall) app from a chat.</span></span>|
|[<span data-ttu-id="e5d0f-149">Guias de lista no chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-149">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="e5d0f-150">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e5d0f-150">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e5d0f-151">Listar guias fixadas a um chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-151">List tabs pinned to a chat.</span></span>|
|[<span data-ttu-id="e5d0f-152">Guia obter no chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-152">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="e5d0f-153">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e5d0f-153">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e5d0f-154">Obtenha uma guia específica fixada para um chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-154">Get a specific tab pinned to a chat.</span></span>|
|[<span data-ttu-id="e5d0f-155">Adicionar guia ao chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-155">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="e5d0f-156">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e5d0f-156">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e5d0f-157">Adicionar (fixar) uma guia a um chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-157">Add (pin) a tab to a chat.</span></span>|
|[<span data-ttu-id="e5d0f-158">Guia atualizar no chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-158">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="e5d0f-159">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e5d0f-159">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e5d0f-160">Atualiza as propriedades de uma guia em um chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-160">Updates the properties of a tab in a chat.</span></span>|
|[<span data-ttu-id="e5d0f-161">Guia remover do chat</span><span class="sxs-lookup"><span data-stu-id="e5d0f-161">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="e5d0f-162">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5d0f-162">None</span></span> | <span data-ttu-id="e5d0f-163">Remover (Desafixar) uma guia de um chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-163">Remove (unpin) a tab from a chat.</span></span>|

><span data-ttu-id="e5d0f-164">**Observação:** Ao usar permissões de aplicativo, certifique-se de saber como você vai obter a ID de chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-164">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="e5d0f-165">Como a lista de chats com permissões de aplicativo não é suportada, nem todos os cenários são possíveis.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-165">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="e5d0f-166">É possível obter IDs de chat com permissões delegadas e de notificações de [alteração para o/chats/getAllMessages](../api/subscription-post-subscriptions.md) com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-166">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="e5d0f-167">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5d0f-167">Properties</span></span>

| <span data-ttu-id="e5d0f-168">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5d0f-168">Property</span></span>   | <span data-ttu-id="e5d0f-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5d0f-169">Type</span></span> |<span data-ttu-id="e5d0f-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5d0f-170">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5d0f-171">id</span><span class="sxs-lookup"><span data-stu-id="e5d0f-171">id</span></span>| <span data-ttu-id="e5d0f-172">String</span><span class="sxs-lookup"><span data-stu-id="e5d0f-172">String</span></span>| <span data-ttu-id="e5d0f-173">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-173">The chat's unique identifier.</span></span> <span data-ttu-id="e5d0f-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-174">Read-only.</span></span>|
| <span data-ttu-id="e5d0f-175">topic</span><span class="sxs-lookup"><span data-stu-id="e5d0f-175">topic</span></span>| <span data-ttu-id="e5d0f-176">String</span><span class="sxs-lookup"><span data-stu-id="e5d0f-176">String</span></span>|  <span data-ttu-id="e5d0f-177">Opcion Assunto ou tópico do chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-177">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="e5d0f-178">Disponível apenas para bate-papos de grupo.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-178">Only available for group chats.</span></span>|
| <span data-ttu-id="e5d0f-179">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5d0f-179">createdDateTime</span></span>| <span data-ttu-id="e5d0f-180">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d0f-180">dateTimeOffset</span></span>|  <span data-ttu-id="e5d0f-181">Data e hora em que o chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-181">Date and time at which the chat was created.</span></span> <span data-ttu-id="e5d0f-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-182">Read-only.</span></span>|
| <span data-ttu-id="e5d0f-183">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5d0f-183">lastUpdatedDateTime</span></span>| <span data-ttu-id="e5d0f-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d0f-184">dateTimeOffset</span></span>|  <span data-ttu-id="e5d0f-185">Data e hora em que o chat foi renomeado ou a associação foi alterada.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-185">Date and time at which the chat was renamed or membership changed.</span></span> <span data-ttu-id="e5d0f-186">lastUpdatedDateTime não é atualizado quando uma mensagem é enviada ao chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-186">lastUpdatedDateTime is not updated when a message is sent to the chat.</span></span> <span data-ttu-id="e5d0f-187">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-187">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5d0f-188">Relações</span><span class="sxs-lookup"><span data-stu-id="e5d0f-188">Relationships</span></span>

| <span data-ttu-id="e5d0f-189">Relação</span><span class="sxs-lookup"><span data-stu-id="e5d0f-189">Relationship</span></span> | <span data-ttu-id="e5d0f-190">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5d0f-190">Type</span></span> |<span data-ttu-id="e5d0f-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5d0f-191">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5d0f-192">installedApps</span><span class="sxs-lookup"><span data-stu-id="e5d0f-192">installedApps</span></span> | <span data-ttu-id="e5d0f-193">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="e5d0f-193">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="e5d0f-194">Uma coleção de todos os aplicativos no chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-194">A collection of all the apps in the chat.</span></span> <span data-ttu-id="e5d0f-195">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-195">Nullable.</span></span> |
| <span data-ttu-id="e5d0f-196">members</span><span class="sxs-lookup"><span data-stu-id="e5d0f-196">members</span></span> | <span data-ttu-id="e5d0f-197">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="e5d0f-197">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="e5d0f-198">Uma coleção de todas as pessoas no chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-198">A collection of all people in the chat.</span></span> <span data-ttu-id="e5d0f-199">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-199">Nullable.</span></span> |
| <span data-ttu-id="e5d0f-200">messages</span><span class="sxs-lookup"><span data-stu-id="e5d0f-200">messages</span></span> | <span data-ttu-id="e5d0f-201">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="e5d0f-201">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="e5d0f-202">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-202">A collection of all the messages in the chat.</span></span> <span data-ttu-id="e5d0f-203">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-203">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e5d0f-204">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5d0f-204">JSON representation</span></span>

<span data-ttu-id="e5d0f-205">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5d0f-205">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="e5d0f-206">Confira também</span><span class="sxs-lookup"><span data-stu-id="e5d0f-206">See also</span></span>

- [<span data-ttu-id="e5d0f-207">channel</span><span class="sxs-lookup"><span data-stu-id="e5d0f-207">channel</span></span>](channel.md)
- [<span data-ttu-id="e5d0f-208">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e5d0f-208">chatMessage</span></span>](chatmessage.md)

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


