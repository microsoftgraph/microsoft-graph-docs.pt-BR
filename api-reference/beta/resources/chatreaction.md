---
title: tipo de recurso de chatMessageReaction
description: 'Representa uma reação a uma entidade chatMessage. '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810063"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="739b5-103">tipo de recurso de chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="739b5-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="739b5-104">Representa uma reação a uma entidade [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="739b5-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="739b5-105">Uma entidade do tipo `chatMessageReaction` é retornado como parte de [receber mensagens de canal](../api/channel-get-message.md) API, como parte da entidade [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="739b5-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel messages](../api/channel-get-message.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="739b5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="739b5-106">Properties</span></span>
| <span data-ttu-id="739b5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="739b5-107">Property</span></span>     | <span data-ttu-id="739b5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="739b5-108">Type</span></span>   |<span data-ttu-id="739b5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="739b5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="739b5-110">reactionType</span><span class="sxs-lookup"><span data-stu-id="739b5-110">reactionType</span></span>|<span data-ttu-id="739b5-111">string</span><span class="sxs-lookup"><span data-stu-id="739b5-111">string</span></span>| <span data-ttu-id="739b5-112">O tipo de reação.</span><span class="sxs-lookup"><span data-stu-id="739b5-112">The type of reaction.</span></span> <span data-ttu-id="739b5-113">Valores planejados incluem:</span><span class="sxs-lookup"><span data-stu-id="739b5-113">Planned values include:</span></span> <br><ul><li><span data-ttu-id="739b5-114">Como - como uma mensagem, conteúdo fica em branco nesse caso.</span><span class="sxs-lookup"><span data-stu-id="739b5-114">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="739b5-115">Emoji - Emoji reação.</span><span class="sxs-lookup"><span data-stu-id="739b5-115">Emoji - Emoji reaction.</span></span> <span data-ttu-id="739b5-116">Conteúdo é definido como o valor unicode do emoji.</span><span class="sxs-lookup"><span data-stu-id="739b5-116">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="739b5-117">Rótulo - o conteúdo é definido como a cadeia de caracteres no rótulo.</span><span class="sxs-lookup"><span data-stu-id="739b5-117">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="739b5-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="739b5-118">createdDateTime</span></span>|<span data-ttu-id="739b5-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="739b5-119">dateTimeOffset</span></span>|<span data-ttu-id="739b5-120">Carimbo de hora UTC da mensagem raiz no formato ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="739b5-120">UTC timestamp of the root message in ISO-8601 format.</span></span>|
|<span data-ttu-id="739b5-121">user</span><span class="sxs-lookup"><span data-stu-id="739b5-121">user</span></span>|<span data-ttu-id="739b5-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="739b5-122">identitySet</span></span>|<span data-ttu-id="739b5-123">O usuário que reacted à mensagem.</span><span class="sxs-lookup"><span data-stu-id="739b5-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="739b5-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="739b5-124">JSON representation</span></span>

<span data-ttu-id="739b5-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="739b5-125">The following is a JSON representation of the resource.</span></span>

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
