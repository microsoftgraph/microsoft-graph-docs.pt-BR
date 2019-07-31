---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 61c23e32d455dd18af639dad31806d54d9e8bd07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974021"
---
# <a name="chat-resource-type"></a><span data-ttu-id="2f04f-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="2f04f-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f04f-104">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="2f04f-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="2f04f-105">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="2f04f-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="2f04f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2f04f-106">Methods</span></span>

|  <span data-ttu-id="2f04f-107">Método</span><span class="sxs-lookup"><span data-stu-id="2f04f-107">Method</span></span>       |  <span data-ttu-id="2f04f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2f04f-108">Return Type</span></span>  | <span data-ttu-id="2f04f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f04f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f04f-110">Listar chats</span><span class="sxs-lookup"><span data-stu-id="2f04f-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="2f04f-111">coleção [chat](channel.md)</span><span class="sxs-lookup"><span data-stu-id="2f04f-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="2f04f-112">Obter a lista de chats de que um usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="2f04f-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="2f04f-113">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="2f04f-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="2f04f-114">chat</span><span class="sxs-lookup"><span data-stu-id="2f04f-114">chat</span></span>](channel.md) | <span data-ttu-id="2f04f-115">Leia as propriedades e as relações do chat.</span><span class="sxs-lookup"><span data-stu-id="2f04f-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="2f04f-116">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="2f04f-116">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="2f04f-117">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="2f04f-117">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="2f04f-118">Obtenha a lista de todos os usuários no chat.</span><span class="sxs-lookup"><span data-stu-id="2f04f-118">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="2f04f-119">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="2f04f-119">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="2f04f-120">conversationmember</span><span class="sxs-lookup"><span data-stu-id="2f04f-120">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="2f04f-121">Obtenha um único usuário no chat.</span><span class="sxs-lookup"><span data-stu-id="2f04f-121">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="2f04f-122">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="2f04f-122">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="2f04f-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2f04f-123">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="2f04f-124">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="2f04f-124">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="2f04f-125">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="2f04f-125">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="2f04f-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2f04f-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="2f04f-127">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="2f04f-127">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="2f04f-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f04f-128">Properties</span></span>

| <span data-ttu-id="2f04f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f04f-129">Property</span></span>   | <span data-ttu-id="2f04f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f04f-130">Type</span></span> |<span data-ttu-id="2f04f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f04f-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f04f-132">id</span><span class="sxs-lookup"><span data-stu-id="2f04f-132">id</span></span>| <span data-ttu-id="2f04f-133">String</span><span class="sxs-lookup"><span data-stu-id="2f04f-133">String</span></span>| <span data-ttu-id="2f04f-134">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="2f04f-134">The chat's unique identifier.</span></span> <span data-ttu-id="2f04f-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f04f-135">Read-only.</span></span>|
| <span data-ttu-id="2f04f-136">topic</span><span class="sxs-lookup"><span data-stu-id="2f04f-136">topic</span></span>| <span data-ttu-id="2f04f-137">String</span><span class="sxs-lookup"><span data-stu-id="2f04f-137">String</span></span>|  <span data-ttu-id="2f04f-138">Opcion Assunto ou tópico do chat.</span><span class="sxs-lookup"><span data-stu-id="2f04f-138">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="2f04f-139">Disponível apenas para bate-papos de grupo.</span><span class="sxs-lookup"><span data-stu-id="2f04f-139">Only available for group chats.</span></span>|
| <span data-ttu-id="2f04f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f04f-140">createdDateTime</span></span>| <span data-ttu-id="2f04f-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f04f-141">dateTimeOffset</span></span>|  <span data-ttu-id="2f04f-142">Data e hora em que o chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="2f04f-142">Date and time at which the chat was created.</span></span> <span data-ttu-id="2f04f-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f04f-143">Read-only.</span></span>|
| <span data-ttu-id="2f04f-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f04f-144">lastUpdatedDateTime</span></span>| <span data-ttu-id="2f04f-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f04f-145">dateTimeOffset</span></span>|  <span data-ttu-id="2f04f-146">Data e hora em que o chat foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="2f04f-146">Date and time at which the chat was updated.</span></span> <span data-ttu-id="2f04f-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f04f-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f04f-148">Relações</span><span class="sxs-lookup"><span data-stu-id="2f04f-148">Relationships</span></span>

| <span data-ttu-id="2f04f-149">Relação</span><span class="sxs-lookup"><span data-stu-id="2f04f-149">Relationship</span></span> | <span data-ttu-id="2f04f-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f04f-150">Type</span></span> |<span data-ttu-id="2f04f-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f04f-151">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f04f-152">installedApps</span><span class="sxs-lookup"><span data-stu-id="2f04f-152">installedApps</span></span> | <span data-ttu-id="2f04f-153">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="2f04f-153">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="2f04f-154">Uma coleção de todos os aplicativos no chat.</span><span class="sxs-lookup"><span data-stu-id="2f04f-154">A collection of all the apps in the chat.</span></span> <span data-ttu-id="2f04f-155">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f04f-155">Nullable.</span></span> |
| <span data-ttu-id="2f04f-156">members</span><span class="sxs-lookup"><span data-stu-id="2f04f-156">members</span></span> | <span data-ttu-id="2f04f-157">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="2f04f-157">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="2f04f-158">Uma coleção de todas as pessoas no chat.</span><span class="sxs-lookup"><span data-stu-id="2f04f-158">A collection of all people in the chat.</span></span> <span data-ttu-id="2f04f-159">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f04f-159">Nullable.</span></span> |
| <span data-ttu-id="2f04f-160">messages</span><span class="sxs-lookup"><span data-stu-id="2f04f-160">messages</span></span> | <span data-ttu-id="2f04f-161">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="2f04f-161">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="2f04f-162">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="2f04f-162">A collection of all the messages in the chat.</span></span> <span data-ttu-id="2f04f-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f04f-163">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2f04f-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f04f-164">JSON representation</span></span>

<span data-ttu-id="2f04f-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f04f-165">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="2f04f-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="2f04f-166">See also</span></span>

- [<span data-ttu-id="2f04f-167">channel</span><span class="sxs-lookup"><span data-stu-id="2f04f-167">channel</span></span>](channel.md)
- [<span data-ttu-id="2f04f-168">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2f04f-168">chatMessage</span></span>](chatmessage.md)

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
