---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 83ab8428fb09a7a2dc0546dcebdf2f409d90d25a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908486"
---
# <a name="chat-resource-type"></a><span data-ttu-id="e74e4-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="e74e4-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e74e4-104">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="e74e4-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="e74e4-105">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e74e4-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="e74e4-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e74e4-106">Methods</span></span>

|  <span data-ttu-id="e74e4-107">Método</span><span class="sxs-lookup"><span data-stu-id="e74e4-107">Method</span></span>       |  <span data-ttu-id="e74e4-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e74e4-108">Return Type</span></span>  | <span data-ttu-id="e74e4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e74e4-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e74e4-110">Listar chats</span><span class="sxs-lookup"><span data-stu-id="e74e4-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="e74e4-111">coleção [chat](channel.md)</span><span class="sxs-lookup"><span data-stu-id="e74e4-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="e74e4-112">Obter a lista de chats de que um usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="e74e4-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="e74e4-113">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="e74e4-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="e74e4-114">chat</span><span class="sxs-lookup"><span data-stu-id="e74e4-114">chat</span></span>](channel.md) | <span data-ttu-id="e74e4-115">Leia as propriedades e as relações do chat.</span><span class="sxs-lookup"><span data-stu-id="e74e4-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="e74e4-116">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="e74e4-116">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="e74e4-117">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="e74e4-117">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="e74e4-118">Obtenha a lista de todos os usuários no chat.</span><span class="sxs-lookup"><span data-stu-id="e74e4-118">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="e74e4-119">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="e74e4-119">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="e74e4-120">conversationmember</span><span class="sxs-lookup"><span data-stu-id="e74e4-120">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="e74e4-121">Obtenha um único usuário no chat.</span><span class="sxs-lookup"><span data-stu-id="e74e4-121">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="e74e4-122">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="e74e4-122">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="e74e4-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e74e4-123">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="e74e4-124">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="e74e4-124">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="e74e4-125">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="e74e4-125">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="e74e4-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e74e4-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="e74e4-127">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="e74e4-127">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="e74e4-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e74e4-128">Properties</span></span>

| <span data-ttu-id="e74e4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e74e4-129">Property</span></span>   | <span data-ttu-id="e74e4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e74e4-130">Type</span></span> |<span data-ttu-id="e74e4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e74e4-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e74e4-132">id</span><span class="sxs-lookup"><span data-stu-id="e74e4-132">id</span></span>| <span data-ttu-id="e74e4-133">String</span><span class="sxs-lookup"><span data-stu-id="e74e4-133">String</span></span>| <span data-ttu-id="e74e4-134">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="e74e4-134">The chat's unique identifier.</span></span> <span data-ttu-id="e74e4-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e74e4-135">Read-only.</span></span>|
| <span data-ttu-id="e74e4-136">topic</span><span class="sxs-lookup"><span data-stu-id="e74e4-136">topic</span></span>| <span data-ttu-id="e74e4-137">String</span><span class="sxs-lookup"><span data-stu-id="e74e4-137">String</span></span>|  <span data-ttu-id="e74e4-138">Opcion Assunto ou tópico do chat.</span><span class="sxs-lookup"><span data-stu-id="e74e4-138">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="e74e4-139">Disponível apenas para bate-papos de grupo.</span><span class="sxs-lookup"><span data-stu-id="e74e4-139">Only available for group chats.</span></span>|
| <span data-ttu-id="e74e4-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e74e4-140">createdDateTime</span></span>| <span data-ttu-id="e74e4-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e74e4-141">dateTimeOffset</span></span>|  <span data-ttu-id="e74e4-142">Data e hora em que o chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="e74e4-142">Date and time at which the chat was created.</span></span> <span data-ttu-id="e74e4-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e74e4-143">Read-only.</span></span>|
| <span data-ttu-id="e74e4-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e74e4-144">lastUpdatedDateTime</span></span>| <span data-ttu-id="e74e4-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e74e4-145">dateTimeOffset</span></span>|  <span data-ttu-id="e74e4-146">Data e hora em que o chat foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="e74e4-146">Date and time at which the chat was updated.</span></span> <span data-ttu-id="e74e4-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e74e4-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e74e4-148">Relações</span><span class="sxs-lookup"><span data-stu-id="e74e4-148">Relationships</span></span>

| <span data-ttu-id="e74e4-149">Relação</span><span class="sxs-lookup"><span data-stu-id="e74e4-149">Relationship</span></span> | <span data-ttu-id="e74e4-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="e74e4-150">Type</span></span> |<span data-ttu-id="e74e4-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="e74e4-151">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e74e4-152">installedApps</span><span class="sxs-lookup"><span data-stu-id="e74e4-152">installedApps</span></span> | <span data-ttu-id="e74e4-153">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="e74e4-153">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="e74e4-154">Uma coleção de todos os aplicativos no chat.</span><span class="sxs-lookup"><span data-stu-id="e74e4-154">A collection of all the apps in the chat.</span></span> <span data-ttu-id="e74e4-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e74e4-155">Nullable.</span></span> |
| <span data-ttu-id="e74e4-156">members</span><span class="sxs-lookup"><span data-stu-id="e74e4-156">members</span></span> | <span data-ttu-id="e74e4-157">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="e74e4-157">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="e74e4-158">Uma coleção de todas as pessoas no chat.</span><span class="sxs-lookup"><span data-stu-id="e74e4-158">A collection of all people in the chat.</span></span> <span data-ttu-id="e74e4-159">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e74e4-159">Nullable.</span></span> |
| <span data-ttu-id="e74e4-160">messages</span><span class="sxs-lookup"><span data-stu-id="e74e4-160">messages</span></span> | <span data-ttu-id="e74e4-161">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="e74e4-161">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="e74e4-162">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="e74e4-162">A collection of all the messages in the chat.</span></span> <span data-ttu-id="e74e4-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e74e4-163">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e74e4-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e74e4-164">JSON representation</span></span>

<span data-ttu-id="e74e4-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e74e4-165">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="e74e4-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="e74e4-166">See also</span></span>

- [<span data-ttu-id="e74e4-167">channel</span><span class="sxs-lookup"><span data-stu-id="e74e4-167">channel</span></span>](channel.md)
- [<span data-ttu-id="e74e4-168">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e74e4-168">chatMessage</span></span>](chatmessage.md)

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
