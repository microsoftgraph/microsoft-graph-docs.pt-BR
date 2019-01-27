---
title: tipo de recurso chatThread
description: Um chatThread é uma coleção de chatMessages no Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: a85b6aea6c48c9295fe88a7412fa7e6b96ee1d3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521338"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="1cc9a-103">tipo de recurso chatThread</span><span class="sxs-lookup"><span data-stu-id="1cc9a-103">chatThread resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cc9a-104">Um chatThread é uma coleção de [chatMessages](chatmessage.md) no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-104">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="1cc9a-105">Atualmente, os chatThreads podem ser[criados em canais](../api/channel-post-chatthreads.md).</span><span class="sxs-lookup"><span data-stu-id="1cc9a-105">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="1cc9a-106">Os lançamentos futuros da API terão suporte para leitura dos chatThreads existentes, além de chats diretos de leitura/escrita entre os usuários que estão fora do escopo da equipe ou do canal.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-106">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="1cc9a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1cc9a-107">Methods</span></span>

| <span data-ttu-id="1cc9a-108">Método</span><span class="sxs-lookup"><span data-stu-id="1cc9a-108">Method</span></span>       | <span data-ttu-id="1cc9a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1cc9a-109">Return Type</span></span>  |<span data-ttu-id="1cc9a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc9a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1cc9a-111">Criar thread</span><span class="sxs-lookup"><span data-stu-id="1cc9a-111">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="1cc9a-112">chatThread</span><span class="sxs-lookup"><span data-stu-id="1cc9a-112">chatThread</span></span>](chatthread.md) |<span data-ttu-id="1cc9a-113">Inicia uma nova thread no canal especificado, fornecendo a primeira mensagem.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-113">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="1cc9a-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cc9a-114">Properties</span></span>
| <span data-ttu-id="1cc9a-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cc9a-115">Property</span></span>     | <span data-ttu-id="1cc9a-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cc9a-116">Type</span></span>   |<span data-ttu-id="1cc9a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc9a-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cc9a-118">id</span><span class="sxs-lookup"><span data-stu-id="1cc9a-118">id</span></span>|<span data-ttu-id="1cc9a-119">String</span><span class="sxs-lookup"><span data-stu-id="1cc9a-119">String</span></span>| <span data-ttu-id="1cc9a-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-120">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cc9a-121">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="1cc9a-121">Relationships</span></span>
| <span data-ttu-id="1cc9a-122">Relação</span><span class="sxs-lookup"><span data-stu-id="1cc9a-122">Relationship</span></span> | <span data-ttu-id="1cc9a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cc9a-123">Type</span></span>   |<span data-ttu-id="1cc9a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc9a-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cc9a-125">rootMessage</span><span class="sxs-lookup"><span data-stu-id="1cc9a-125">rootMessage</span></span>|[<span data-ttu-id="1cc9a-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="1cc9a-126">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="1cc9a-127">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-127">Nullable.</span></span>|
|<span data-ttu-id="1cc9a-128">chatMessages</span><span class="sxs-lookup"><span data-stu-id="1cc9a-128">chatMessages</span></span>|<span data-ttu-id="1cc9a-129">coleção de [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="1cc9a-129">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="1cc9a-130">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-130">Nullable.</span></span>|

> <span data-ttu-id="1cc9a-131">Atualmente essas relações existem implicitamente, mas não podem ler ou escreveu.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-131">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="1cc9a-132">As versões Beta futuras da API oferecerão suporte para isso.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-132">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cc9a-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cc9a-133">JSON representation</span></span>

<span data-ttu-id="1cc9a-134">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1cc9a-134">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
