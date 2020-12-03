---
title: tipo de recurso chat
description: Um chat é uma coleção de chatMessages entre um ou mais participantes.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f9cc43442e077dfe245fa8422b954859bf1c569
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564037"
---
# <a name="chat-resource-type"></a><span data-ttu-id="08daf-103">tipo de recurso chat</span><span class="sxs-lookup"><span data-stu-id="08daf-103">chat resource type</span></span>

<span data-ttu-id="08daf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08daf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08daf-105">Um chat é uma coleção de [chatMessages](chatmessage.md) entre um ou mais participantes.</span><span class="sxs-lookup"><span data-stu-id="08daf-105">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="08daf-106">Os participantes podem ser usuários ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="08daf-106">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="08daf-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="08daf-107">Methods</span></span>

|  <span data-ttu-id="08daf-108">Método</span><span class="sxs-lookup"><span data-stu-id="08daf-108">Method</span></span>       |  <span data-ttu-id="08daf-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="08daf-109">Return Type</span></span>  | <span data-ttu-id="08daf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="08daf-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08daf-111">Obter chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="08daf-111">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="08daf-112">chat</span><span class="sxs-lookup"><span data-stu-id="08daf-112">chat</span></span>](chat.md)| <span data-ttu-id="08daf-113">Obter um chat entre o usuário e o aplicativo</span><span class="sxs-lookup"><span data-stu-id="08daf-113">Get one-on-one chat between user and the app</span></span> | 

><span data-ttu-id="08daf-114">**Observação:** Ao usar permissões de aplicativo, certifique-se de saber como você vai obter a ID de chat.</span><span class="sxs-lookup"><span data-stu-id="08daf-114">**Note:** When using application permissions, be sure you know how you're going to get the chat ID.</span></span> <span data-ttu-id="08daf-115">Como a lista de chats com permissões de aplicativo não é suportada, nem todos os cenários são possíveis.</span><span class="sxs-lookup"><span data-stu-id="08daf-115">Because listing chats with application permissions is not supported, not all scenarios are possible.</span></span> <span data-ttu-id="08daf-116">É possível obter IDs de chat com permissões delegadas e de notificações de [alteração para o/chats/getAllMessages](../api/subscription-post-subscriptions.md) com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08daf-116">It is possible to get chat IDs with delegated permissions, and from [change notifications for /chats/getAllMessages](../api/subscription-post-subscriptions.md) with application permissions.</span></span>

## <a name="properties"></a><span data-ttu-id="08daf-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08daf-117">Properties</span></span>

| <span data-ttu-id="08daf-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08daf-118">Property</span></span>   | <span data-ttu-id="08daf-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="08daf-119">Type</span></span> |<span data-ttu-id="08daf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="08daf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08daf-121">id</span><span class="sxs-lookup"><span data-stu-id="08daf-121">id</span></span>| <span data-ttu-id="08daf-122">String</span><span class="sxs-lookup"><span data-stu-id="08daf-122">String</span></span>| <span data-ttu-id="08daf-123">O identificador exclusivo do chat.</span><span class="sxs-lookup"><span data-stu-id="08daf-123">The chat's unique identifier.</span></span> <span data-ttu-id="08daf-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="08daf-124">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="08daf-125">Relações</span><span class="sxs-lookup"><span data-stu-id="08daf-125">Relationships</span></span>

| <span data-ttu-id="08daf-126">Relação</span><span class="sxs-lookup"><span data-stu-id="08daf-126">Relationship</span></span> | <span data-ttu-id="08daf-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="08daf-127">Type</span></span> |<span data-ttu-id="08daf-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="08daf-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08daf-129">messages</span><span class="sxs-lookup"><span data-stu-id="08daf-129">messages</span></span> | <span data-ttu-id="08daf-130">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="08daf-130">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="08daf-131">Uma coleção de todas as mensagens no chat.</span><span class="sxs-lookup"><span data-stu-id="08daf-131">A collection of all the messages in the chat.</span></span> <span data-ttu-id="08daf-132">Anulável.</span><span class="sxs-lookup"><span data-stu-id="08daf-132">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08daf-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08daf-133">JSON representation</span></span>

<span data-ttu-id="08daf-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08daf-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
}
```

## <a name="see-also"></a><span data-ttu-id="08daf-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="08daf-135">See also</span></span>

- [<span data-ttu-id="08daf-136">channel</span><span class="sxs-lookup"><span data-stu-id="08daf-136">channel</span></span>](channel.md)
- [<span data-ttu-id="08daf-137">chatMessage</span><span class="sxs-lookup"><span data-stu-id="08daf-137">chatMessage</span></span>](chatmessage.md)

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


