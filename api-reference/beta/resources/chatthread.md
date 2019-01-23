---
title: tipo de recurso chatThread
description: Um chatThread é uma coleção de chatMessages no Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: 19365109c2008d52d3597b3d23fc1baefa5cfd1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399602"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="e76d6-103">tipo de recurso chatThread</span><span class="sxs-lookup"><span data-stu-id="e76d6-103">chatThread resource type</span></span>

> <span data-ttu-id="e76d6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e76d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e76d6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e76d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e76d6-106">Um chatThread é uma coleção de [chatMessages](chatmessage.md) no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e76d6-106">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="e76d6-107">Atualmente, os chatThreads podem ser[criados em canais](../api/channel-post-chatthreads.md).</span><span class="sxs-lookup"><span data-stu-id="e76d6-107">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="e76d6-108">Os lançamentos futuros da API terão suporte para leitura dos chatThreads existentes, além de chats diretos de leitura/escrita entre os usuários que estão fora do escopo da equipe ou do canal.</span><span class="sxs-lookup"><span data-stu-id="e76d6-108">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="e76d6-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="e76d6-109">Methods</span></span>

| <span data-ttu-id="e76d6-110">Método</span><span class="sxs-lookup"><span data-stu-id="e76d6-110">Method</span></span>       | <span data-ttu-id="e76d6-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e76d6-111">Return Type</span></span>  |<span data-ttu-id="e76d6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e76d6-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e76d6-113">Criar thread</span><span class="sxs-lookup"><span data-stu-id="e76d6-113">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="e76d6-114">chatThread</span><span class="sxs-lookup"><span data-stu-id="e76d6-114">chatThread</span></span>](chatthread.md) |<span data-ttu-id="e76d6-115">Inicia uma nova thread no canal especificado, fornecendo a primeira mensagem.</span><span class="sxs-lookup"><span data-stu-id="e76d6-115">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="e76d6-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e76d6-116">Properties</span></span>
| <span data-ttu-id="e76d6-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e76d6-117">Property</span></span>     | <span data-ttu-id="e76d6-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e76d6-118">Type</span></span>   |<span data-ttu-id="e76d6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e76d6-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e76d6-120">id</span><span class="sxs-lookup"><span data-stu-id="e76d6-120">id</span></span>|<span data-ttu-id="e76d6-121">String</span><span class="sxs-lookup"><span data-stu-id="e76d6-121">String</span></span>| <span data-ttu-id="e76d6-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e76d6-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e76d6-123">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="e76d6-123">Relationships</span></span>
| <span data-ttu-id="e76d6-124">Relação</span><span class="sxs-lookup"><span data-stu-id="e76d6-124">Relationship</span></span> | <span data-ttu-id="e76d6-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e76d6-125">Type</span></span>   |<span data-ttu-id="e76d6-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e76d6-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e76d6-127">rootMessage</span><span class="sxs-lookup"><span data-stu-id="e76d6-127">rootMessage</span></span>|[<span data-ttu-id="e76d6-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e76d6-128">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="e76d6-129">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e76d6-129">Nullable.</span></span>|
|<span data-ttu-id="e76d6-130">chatMessages</span><span class="sxs-lookup"><span data-stu-id="e76d6-130">chatMessages</span></span>|<span data-ttu-id="e76d6-131">coleção de [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="e76d6-131">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="e76d6-132">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e76d6-132">Nullable.</span></span>|

> <span data-ttu-id="e76d6-133">Atualmente essas relações existem implicitamente, mas não podem ler ou escreveu.</span><span class="sxs-lookup"><span data-stu-id="e76d6-133">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="e76d6-134">As versões Beta futuras da API oferecerão suporte para isso.</span><span class="sxs-lookup"><span data-stu-id="e76d6-134">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e76d6-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e76d6-135">JSON representation</span></span>

<span data-ttu-id="e76d6-136">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e76d6-136">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatThread"
}-->

```json
{
  "id": "string (identifier)"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
