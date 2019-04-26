---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1091021235a50d3dfa237467e319da9b131b7a72
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339710"
---
# <a name="chat-resource-type"></a><span data-ttu-id="688c1-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="688c1-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="688c1-104">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="688c1-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="688c1-105">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="688c1-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="688c1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="688c1-106">Methods</span></span>

|  <span data-ttu-id="688c1-107">Método</span><span class="sxs-lookup"><span data-stu-id="688c1-107">Method</span></span>       |  <span data-ttu-id="688c1-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="688c1-108">Return Type</span></span>  | <span data-ttu-id="688c1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="688c1-109">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="688c1-110">Listar chats</span><span class="sxs-lookup"><span data-stu-id="688c1-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="688c1-111">coleção [chat](channel.md)</span><span class="sxs-lookup"><span data-stu-id="688c1-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="688c1-112">Obter a lista de chats de que um usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="688c1-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="688c1-113">Obter chat</span><span class="sxs-lookup"><span data-stu-id="688c1-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="688c1-114">chat</span><span class="sxs-lookup"><span data-stu-id="688c1-114">chat</span></span>](channel.md) | <span data-ttu-id="688c1-115">Leia as propriedades e as relações do chat.</span><span class="sxs-lookup"><span data-stu-id="688c1-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="688c1-116">Listar mensagens em um chat</span><span class="sxs-lookup"><span data-stu-id="688c1-116">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="688c1-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="688c1-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="688c1-118">Obter mensagens em um bate-papo de grupo ou 1:1.</span><span class="sxs-lookup"><span data-stu-id="688c1-118">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="688c1-119">Obter mensagem no chat</span><span class="sxs-lookup"><span data-stu-id="688c1-119">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="688c1-120">chatMessage</span><span class="sxs-lookup"><span data-stu-id="688c1-120">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="688c1-121">Obter uma única mensagem em um chat.</span><span class="sxs-lookup"><span data-stu-id="688c1-121">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="688c1-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="688c1-122">Properties</span></span>

| <span data-ttu-id="688c1-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="688c1-123">Property</span></span>     | <span data-ttu-id="688c1-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="688c1-124">Type</span></span>   |<span data-ttu-id="688c1-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="688c1-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="688c1-126">id</span><span class="sxs-lookup"><span data-stu-id="688c1-126">id</span></span>| <span data-ttu-id="688c1-127">String</span><span class="sxs-lookup"><span data-stu-id="688c1-127">String</span></span>| <span data-ttu-id="688c1-128">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="688c1-128">The chat's unique identifier.</span></span> <span data-ttu-id="688c1-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="688c1-129">Read-only.</span></span>|
| <span data-ttu-id="688c1-130">topic</span><span class="sxs-lookup"><span data-stu-id="688c1-130">topic</span></span>| <span data-ttu-id="688c1-131">String</span><span class="sxs-lookup"><span data-stu-id="688c1-131">String</span></span>|  <span data-ttu-id="688c1-132">Opcion Assunto ou tópico do chat.</span><span class="sxs-lookup"><span data-stu-id="688c1-132">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="688c1-133">Disponível apenas para bate-papos de grupo.</span><span class="sxs-lookup"><span data-stu-id="688c1-133">Only available for group chats.</span></span>|
| <span data-ttu-id="688c1-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="688c1-134">createdDateTime</span></span>| <span data-ttu-id="688c1-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="688c1-135">dateTimeOffset</span></span>|  <span data-ttu-id="688c1-136">Data e hora em que o chat foi criado.</span><span class="sxs-lookup"><span data-stu-id="688c1-136">Date and time at which the chat was created.</span></span> <span data-ttu-id="688c1-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="688c1-137">Read-only.</span></span>|
| <span data-ttu-id="688c1-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="688c1-138">lastUpdatedDateTime</span></span>| <span data-ttu-id="688c1-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="688c1-139">dateTimeOffset</span></span>|  <span data-ttu-id="688c1-140">Data e hora em que o chat foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="688c1-140">Date and time at which the chat was updated.</span></span> <span data-ttu-id="688c1-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="688c1-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="688c1-142">Relações</span><span class="sxs-lookup"><span data-stu-id="688c1-142">Relationships</span></span>
| <span data-ttu-id="688c1-143">Relação</span><span class="sxs-lookup"><span data-stu-id="688c1-143">Relationship</span></span> | <span data-ttu-id="688c1-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="688c1-144">Type</span></span>   |<span data-ttu-id="688c1-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="688c1-145">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="688c1-146">messages</span><span class="sxs-lookup"><span data-stu-id="688c1-146">messages</span></span> | <span data-ttu-id="688c1-147">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="688c1-147">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="688c1-148">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="688c1-148">A collection of all the messages in the chat.</span></span> <span data-ttu-id="688c1-149">Anulável.</span><span class="sxs-lookup"><span data-stu-id="688c1-149">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="688c1-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="688c1-150">JSON representation</span></span>

<span data-ttu-id="688c1-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="688c1-151">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="688c1-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="688c1-152">See also</span></span>

- [<span data-ttu-id="688c1-153">channel</span><span class="sxs-lookup"><span data-stu-id="688c1-153">channel</span></span>](channel.md)
- [<span data-ttu-id="688c1-154">chatMessage</span><span class="sxs-lookup"><span data-stu-id="688c1-154">chatMessage</span></span>](chatmessage.md)

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
