---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4d0f1009079c4994814385ae8758af6c211f17a2
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344973"
---
# <a name="chat-resource-type"></a><span data-ttu-id="46493-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="46493-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46493-104">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="46493-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="46493-105">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="46493-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="46493-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="46493-106">Methods</span></span>

|  <span data-ttu-id="46493-107">Método</span><span class="sxs-lookup"><span data-stu-id="46493-107">Method</span></span>       |  <span data-ttu-id="46493-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="46493-108">Return Type</span></span>  | <span data-ttu-id="46493-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="46493-109">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="46493-110">Listar chats</span><span class="sxs-lookup"><span data-stu-id="46493-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="46493-111">coleção [chat](channel.md)</span><span class="sxs-lookup"><span data-stu-id="46493-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="46493-112">Obter a lista de chats de que um usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="46493-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="46493-113">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="46493-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="46493-114">chat</span><span class="sxs-lookup"><span data-stu-id="46493-114">chat</span></span>](channel.md) | <span data-ttu-id="46493-115">Leia as propriedades e as relações do chat.</span><span class="sxs-lookup"><span data-stu-id="46493-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="46493-116">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="46493-116">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="46493-117">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="46493-117">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="46493-118">Obtenha a lista de todos os usuários no chat.</span><span class="sxs-lookup"><span data-stu-id="46493-118">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="46493-119">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="46493-119">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="46493-120">conversationmember</span><span class="sxs-lookup"><span data-stu-id="46493-120">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="46493-121">Obtenha um único usuário no chat.</span><span class="sxs-lookup"><span data-stu-id="46493-121">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="46493-122">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="46493-122">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="46493-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="46493-123">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="46493-124">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="46493-124">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="46493-125">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="46493-125">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="46493-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="46493-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="46493-127">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="46493-127">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="46493-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46493-128">Properties</span></span>

| <span data-ttu-id="46493-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46493-129">Property</span></span>     | <span data-ttu-id="46493-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="46493-130">Type</span></span>   |<span data-ttu-id="46493-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="46493-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46493-132">id</span><span class="sxs-lookup"><span data-stu-id="46493-132">id</span></span>| <span data-ttu-id="46493-133">String</span><span class="sxs-lookup"><span data-stu-id="46493-133">String</span></span>| <span data-ttu-id="46493-134">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="46493-134">The chat's unique identifier.</span></span> <span data-ttu-id="46493-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46493-135">Read-only.</span></span>|
| <span data-ttu-id="46493-136">topic</span><span class="sxs-lookup"><span data-stu-id="46493-136">topic</span></span>| <span data-ttu-id="46493-137">String</span><span class="sxs-lookup"><span data-stu-id="46493-137">String</span></span>|  <span data-ttu-id="46493-138">Opcion Assunto ou tópico do chat.</span><span class="sxs-lookup"><span data-stu-id="46493-138">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="46493-139">Disponível apenas para bate-papos de grupo.</span><span class="sxs-lookup"><span data-stu-id="46493-139">Only available for group chats.</span></span>|
| <span data-ttu-id="46493-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46493-140">createdDateTime</span></span>| <span data-ttu-id="46493-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46493-141">dateTimeOffset</span></span>|  <span data-ttu-id="46493-142">Data e hora em que o chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="46493-142">Date and time at which the chat was created.</span></span> <span data-ttu-id="46493-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46493-143">Read-only.</span></span>|
| <span data-ttu-id="46493-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="46493-144">lastUpdatedDateTime</span></span>| <span data-ttu-id="46493-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46493-145">dateTimeOffset</span></span>|  <span data-ttu-id="46493-146">Data e hora em que o chat foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="46493-146">Date and time at which the chat was updated.</span></span> <span data-ttu-id="46493-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46493-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46493-148">Relações</span><span class="sxs-lookup"><span data-stu-id="46493-148">Relationships</span></span>
| <span data-ttu-id="46493-149">Relação</span><span class="sxs-lookup"><span data-stu-id="46493-149">Relationship</span></span> | <span data-ttu-id="46493-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="46493-150">Type</span></span>   |<span data-ttu-id="46493-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="46493-151">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46493-152">membros</span><span class="sxs-lookup"><span data-stu-id="46493-152">members</span></span> | <span data-ttu-id="46493-153">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="46493-153">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="46493-154">Uma coleção de todas as pessoas no chat.</span><span class="sxs-lookup"><span data-stu-id="46493-154">A collection of all people in the chat.</span></span> <span data-ttu-id="46493-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="46493-155">Nullable.</span></span> |
| <span data-ttu-id="46493-156">messages</span><span class="sxs-lookup"><span data-stu-id="46493-156">messages</span></span> | <span data-ttu-id="46493-157">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="46493-157">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="46493-158">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="46493-158">A collection of all the messages in the chat.</span></span> <span data-ttu-id="46493-159">Anulável.</span><span class="sxs-lookup"><span data-stu-id="46493-159">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="46493-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46493-160">JSON representation</span></span>

<span data-ttu-id="46493-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46493-161">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="46493-162">Confira também</span><span class="sxs-lookup"><span data-stu-id="46493-162">See also</span></span>

- [<span data-ttu-id="46493-163">channel</span><span class="sxs-lookup"><span data-stu-id="46493-163">channel</span></span>](channel.md)
- [<span data-ttu-id="46493-164">chatMessage</span><span class="sxs-lookup"><span data-stu-id="46493-164">chatMessage</span></span>](chatmessage.md)

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
