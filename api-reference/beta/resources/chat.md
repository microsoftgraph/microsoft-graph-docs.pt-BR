---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3fa6952640a1986d0139007ba863275aef2bc6aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507737"
---
# <a name="chat-resource-type"></a><span data-ttu-id="43fe9-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="43fe9-103">chat resource type</span></span>

<span data-ttu-id="43fe9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="43fe9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43fe9-105">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="43fe9-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="43fe9-106">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="43fe9-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="43fe9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="43fe9-107">Methods</span></span>

|  <span data-ttu-id="43fe9-108">Método</span><span class="sxs-lookup"><span data-stu-id="43fe9-108">Method</span></span>       |  <span data-ttu-id="43fe9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="43fe9-109">Return Type</span></span>  | <span data-ttu-id="43fe9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="43fe9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43fe9-111">Listar chats</span><span class="sxs-lookup"><span data-stu-id="43fe9-111">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="43fe9-112">coleção [chat](channel.md)</span><span class="sxs-lookup"><span data-stu-id="43fe9-112">[chat](channel.md) collection</span></span> | <span data-ttu-id="43fe9-113">Obter a lista de chats de que um usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="43fe9-113">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="43fe9-114">Obter bate-papo</span><span class="sxs-lookup"><span data-stu-id="43fe9-114">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="43fe9-115">chat</span><span class="sxs-lookup"><span data-stu-id="43fe9-115">chat</span></span>](channel.md) | <span data-ttu-id="43fe9-116">Leia as propriedades e as relações do chat.</span><span class="sxs-lookup"><span data-stu-id="43fe9-116">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="43fe9-117">Listar membros de chat</span><span class="sxs-lookup"><span data-stu-id="43fe9-117">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="43fe9-118">coleção [conversationmember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="43fe9-118">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="43fe9-119">Ver a lista de todos os usuários no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="43fe9-119">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="43fe9-120">Obter membro de chat</span><span class="sxs-lookup"><span data-stu-id="43fe9-120">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="43fe9-121">conversationmember</span><span class="sxs-lookup"><span data-stu-id="43fe9-121">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="43fe9-122">Obter um único usuário no bate-papo.</span><span class="sxs-lookup"><span data-stu-id="43fe9-122">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="43fe9-123">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="43fe9-123">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="43fe9-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="43fe9-124">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="43fe9-125">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="43fe9-125">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="43fe9-126">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="43fe9-126">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="43fe9-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="43fe9-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="43fe9-128">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="43fe9-128">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="43fe9-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43fe9-129">Properties</span></span>

| <span data-ttu-id="43fe9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43fe9-130">Property</span></span>   | <span data-ttu-id="43fe9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="43fe9-131">Type</span></span> |<span data-ttu-id="43fe9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="43fe9-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="43fe9-133">id</span><span class="sxs-lookup"><span data-stu-id="43fe9-133">id</span></span>| <span data-ttu-id="43fe9-134">String</span><span class="sxs-lookup"><span data-stu-id="43fe9-134">String</span></span>| <span data-ttu-id="43fe9-135">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="43fe9-135">The chat's unique identifier.</span></span> <span data-ttu-id="43fe9-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="43fe9-136">Read-only.</span></span>|
| <span data-ttu-id="43fe9-137">topic</span><span class="sxs-lookup"><span data-stu-id="43fe9-137">topic</span></span>| <span data-ttu-id="43fe9-138">String</span><span class="sxs-lookup"><span data-stu-id="43fe9-138">String</span></span>|  <span data-ttu-id="43fe9-139">Opcion Assunto ou tópico do chat.</span><span class="sxs-lookup"><span data-stu-id="43fe9-139">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="43fe9-140">Disponível apenas para bate-papos de grupo.</span><span class="sxs-lookup"><span data-stu-id="43fe9-140">Only available for group chats.</span></span>|
| <span data-ttu-id="43fe9-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43fe9-141">createdDateTime</span></span>| <span data-ttu-id="43fe9-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43fe9-142">dateTimeOffset</span></span>|  <span data-ttu-id="43fe9-143">Data e hora em que o chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="43fe9-143">Date and time at which the chat was created.</span></span> <span data-ttu-id="43fe9-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="43fe9-144">Read-only.</span></span>|
| <span data-ttu-id="43fe9-145">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="43fe9-145">lastUpdatedDateTime</span></span>| <span data-ttu-id="43fe9-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43fe9-146">dateTimeOffset</span></span>|  <span data-ttu-id="43fe9-147">Data e hora em que o chat foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="43fe9-147">Date and time at which the chat was updated.</span></span> <span data-ttu-id="43fe9-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="43fe9-148">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43fe9-149">Relações</span><span class="sxs-lookup"><span data-stu-id="43fe9-149">Relationships</span></span>

| <span data-ttu-id="43fe9-150">Relação</span><span class="sxs-lookup"><span data-stu-id="43fe9-150">Relationship</span></span> | <span data-ttu-id="43fe9-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="43fe9-151">Type</span></span> |<span data-ttu-id="43fe9-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="43fe9-152">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="43fe9-153">installedApps</span><span class="sxs-lookup"><span data-stu-id="43fe9-153">installedApps</span></span> | <span data-ttu-id="43fe9-154">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="43fe9-154">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="43fe9-155">Uma coleção de todos os aplicativos no chat.</span><span class="sxs-lookup"><span data-stu-id="43fe9-155">A collection of all the apps in the chat.</span></span> <span data-ttu-id="43fe9-156">Anulável.</span><span class="sxs-lookup"><span data-stu-id="43fe9-156">Nullable.</span></span> |
| <span data-ttu-id="43fe9-157">membros</span><span class="sxs-lookup"><span data-stu-id="43fe9-157">members</span></span> | <span data-ttu-id="43fe9-158">coleção [conversationMember](conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="43fe9-158">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="43fe9-159">Uma coleção de todas as pessoas no chat.</span><span class="sxs-lookup"><span data-stu-id="43fe9-159">A collection of all people in the chat.</span></span> <span data-ttu-id="43fe9-160">Anulável.</span><span class="sxs-lookup"><span data-stu-id="43fe9-160">Nullable.</span></span> |
| <span data-ttu-id="43fe9-161">messages</span><span class="sxs-lookup"><span data-stu-id="43fe9-161">messages</span></span> | <span data-ttu-id="43fe9-162">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="43fe9-162">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="43fe9-163">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="43fe9-163">A collection of all the messages in the chat.</span></span> <span data-ttu-id="43fe9-164">Anulável.</span><span class="sxs-lookup"><span data-stu-id="43fe9-164">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="43fe9-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43fe9-165">JSON representation</span></span>

<span data-ttu-id="43fe9-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43fe9-166">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="43fe9-167">Confira também</span><span class="sxs-lookup"><span data-stu-id="43fe9-167">See also</span></span>

- [<span data-ttu-id="43fe9-168">canal</span><span class="sxs-lookup"><span data-stu-id="43fe9-168">channel</span></span>](channel.md)
- [<span data-ttu-id="43fe9-169">chatMessage</span><span class="sxs-lookup"><span data-stu-id="43fe9-169">chatMessage</span></span>](chatmessage.md)

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
