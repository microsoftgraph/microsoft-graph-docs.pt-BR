---
title: tipo de recurso de chatMessageReaction
description: 'Representa uma reação a uma entidade chatMessage. '
ms.openlocfilehash: 1ad1f7948405a8891ec9aa13065b71108e9c47c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040849"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="37492-103">tipo de recurso de chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="37492-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="37492-104">Representa uma reação a uma entidade [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="37492-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="37492-105">Uma entidade do tipo `chatMessageReaction` é retornado como parte de [receber mensagens de canal](../api/channel-get-message.md) API, como parte da entidade [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="37492-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel messages](../api/channel-get-message.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="37492-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37492-106">Properties</span></span>
| <span data-ttu-id="37492-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37492-107">Property</span></span>     | <span data-ttu-id="37492-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="37492-108">Type</span></span>   |<span data-ttu-id="37492-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="37492-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37492-110">reactionType</span><span class="sxs-lookup"><span data-stu-id="37492-110">reactionType</span></span>|<span data-ttu-id="37492-111">string</span><span class="sxs-lookup"><span data-stu-id="37492-111">string</span></span>| <span data-ttu-id="37492-112">O tipo de reação.</span><span class="sxs-lookup"><span data-stu-id="37492-112">The type of reaction.</span></span> <span data-ttu-id="37492-113">Valores planejados incluem:</span><span class="sxs-lookup"><span data-stu-id="37492-113">Planned values include:</span></span> <br><ul><li><span data-ttu-id="37492-114">Como - como uma mensagem, conteúdo fica em branco nesse caso.</span><span class="sxs-lookup"><span data-stu-id="37492-114">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="37492-115">Emoji - Emoji reação.</span><span class="sxs-lookup"><span data-stu-id="37492-115">Emoji - Emoji reaction.</span></span> <span data-ttu-id="37492-116">Conteúdo é definido como o valor unicode do emoji.</span><span class="sxs-lookup"><span data-stu-id="37492-116">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="37492-117">Rótulo - o conteúdo é definido como a cadeia de caracteres no rótulo.</span><span class="sxs-lookup"><span data-stu-id="37492-117">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="37492-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37492-118">createdDateTime</span></span>|<span data-ttu-id="37492-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37492-119">dateTimeOffset</span></span>|<span data-ttu-id="37492-120">Carimbo de hora UTC da mensagem raiz no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="37492-120">UTC timestamp of the root message in ISO-8601 format.</span></span>|
|<span data-ttu-id="37492-121">user</span><span class="sxs-lookup"><span data-stu-id="37492-121">user</span></span>|<span data-ttu-id="37492-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="37492-122">identitySet</span></span>|<span data-ttu-id="37492-123">O usuário que reacted à mensagem.</span><span class="sxs-lookup"><span data-stu-id="37492-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37492-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37492-124">JSON representation</span></span>

<span data-ttu-id="37492-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37492-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "content"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageReaction"
}-->

```json
{
  "reactionType": "string ",
  "createdDateTime": "string (timestamp)",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message reaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
