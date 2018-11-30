---
title: tipo de recurso de chatThread
description: Um chatThread é uma coleção de chatMessages em Teams da Microsoft.
ms.openlocfilehash: ef8f118ae4354a5e4197802708aecfa1fb6f8cb8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039964"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="6d3b4-103">tipo de recurso de chatThread</span><span class="sxs-lookup"><span data-stu-id="6d3b4-103">chatThread resource type</span></span>

> <span data-ttu-id="6d3b4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6d3b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d3b4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6d3b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d3b4-106">Um chatThread é uma coleção de [chatMessages](chatmessage.md) em Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6d3b4-106">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="6d3b4-107">Atualmente, chatThreads pode ser [criado no canais](../api/channel-post-chatthreads.md).</span><span class="sxs-lookup"><span data-stu-id="6d3b4-107">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="6d3b4-108">Versões de futuro API dará suporte a chatThreads existente, bem como leitura/gravação chats diretos entre os usuários que estão fora do escopo de uma equipe ou canal de leitura.</span><span class="sxs-lookup"><span data-stu-id="6d3b4-108">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="6d3b4-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="6d3b4-109">Methods</span></span>

| <span data-ttu-id="6d3b4-110">Método</span><span class="sxs-lookup"><span data-stu-id="6d3b4-110">Method</span></span>       | <span data-ttu-id="6d3b4-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6d3b4-111">Return Type</span></span>  |<span data-ttu-id="6d3b4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d3b4-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d3b4-113">Criar thread</span><span class="sxs-lookup"><span data-stu-id="6d3b4-113">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="6d3b4-114">chatThread</span><span class="sxs-lookup"><span data-stu-id="6d3b4-114">chatThread</span></span>](chatthread.md) |<span data-ttu-id="6d3b4-115">Inicie um novo segmento no canal especificado, fornecendo a primeira mensagem.</span><span class="sxs-lookup"><span data-stu-id="6d3b4-115">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d3b4-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d3b4-116">Properties</span></span>
| <span data-ttu-id="6d3b4-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d3b4-117">Property</span></span>     | <span data-ttu-id="6d3b4-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d3b4-118">Type</span></span>   |<span data-ttu-id="6d3b4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d3b4-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d3b4-120">id</span><span class="sxs-lookup"><span data-stu-id="6d3b4-120">id</span></span>|<span data-ttu-id="6d3b4-121">String</span><span class="sxs-lookup"><span data-stu-id="6d3b4-121">String</span></span>| <span data-ttu-id="6d3b4-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d3b4-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d3b4-123">Relações</span><span class="sxs-lookup"><span data-stu-id="6d3b4-123">Relationships</span></span>
| <span data-ttu-id="6d3b4-124">Relação</span><span class="sxs-lookup"><span data-stu-id="6d3b4-124">Relationship</span></span> | <span data-ttu-id="6d3b4-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d3b4-125">Type</span></span>   |<span data-ttu-id="6d3b4-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d3b4-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d3b4-127">rootMessage</span><span class="sxs-lookup"><span data-stu-id="6d3b4-127">rootMessage</span></span>|[<span data-ttu-id="6d3b4-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6d3b4-128">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="6d3b4-129">Anulável.</span><span class="sxs-lookup"><span data-stu-id="6d3b4-129">Nullable.</span></span>|
|<span data-ttu-id="6d3b4-130">chatMessages</span><span class="sxs-lookup"><span data-stu-id="6d3b4-130">chatMessages</span></span>|<span data-ttu-id="6d3b4-131">coleção [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="6d3b4-131">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="6d3b4-132">Anulável.</span><span class="sxs-lookup"><span data-stu-id="6d3b4-132">Nullable.</span></span>|

> <span data-ttu-id="6d3b4-133">Atualmente essas relações existe implicitamente, mas não pode ler ou gravados.</span><span class="sxs-lookup"><span data-stu-id="6d3b4-133">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="6d3b4-134">Versões beta futuras API dará suporte a isso.</span><span class="sxs-lookup"><span data-stu-id="6d3b4-134">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d3b4-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d3b4-135">JSON representation</span></span>

<span data-ttu-id="6d3b4-136">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6d3b4-136">Here is a JSON representation of the resource</span></span>

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
  "id": "string (identifier)",
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
