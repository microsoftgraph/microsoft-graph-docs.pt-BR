---
title: tipo de recurso chatMessageReaction
description: 'Representa uma reação a uma entidade chat. '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: 953895b28b6bae6e17eead938565fde289c49ef7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2019
ms.locfileid: "31481381"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="81af6-103">tipo de recurso chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="81af6-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="81af6-104">Representa uma reação a uma entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="81af6-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="81af6-105">Uma entidade do tipo `chatMessageReaction` é retornada como parte da API [Get Channel messages](../api/channel-get-message.md) , como parte da entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="81af6-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel messages](../api/channel-get-message.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="81af6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81af6-106">Properties</span></span>
| <span data-ttu-id="81af6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81af6-107">Property</span></span>     | <span data-ttu-id="81af6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="81af6-108">Type</span></span>   |<span data-ttu-id="81af6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="81af6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81af6-110">reactiontype</span><span class="sxs-lookup"><span data-stu-id="81af6-110">reactionType</span></span>|<span data-ttu-id="81af6-111">string</span><span class="sxs-lookup"><span data-stu-id="81af6-111">string</span></span>| <span data-ttu-id="81af6-112">O tipo de reação.</span><span class="sxs-lookup"><span data-stu-id="81af6-112">The type of reaction.</span></span> <span data-ttu-id="81af6-113">Os valores planejados incluem:</span><span class="sxs-lookup"><span data-stu-id="81af6-113">Planned values include:</span></span> <br><ul><li><span data-ttu-id="81af6-114">Semelhante a uma mensagem, o conteúdo está em branco neste caso.</span><span class="sxs-lookup"><span data-stu-id="81af6-114">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="81af6-115">Emoji-reação de Emoji.</span><span class="sxs-lookup"><span data-stu-id="81af6-115">Emoji - Emoji reaction.</span></span> <span data-ttu-id="81af6-116">O conteúdo é definido para o valor Unicode do emoji.</span><span class="sxs-lookup"><span data-stu-id="81af6-116">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="81af6-117">Rótulo-o conteúdo é definido como a cadeia de caracteres no rótulo.</span><span class="sxs-lookup"><span data-stu-id="81af6-117">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="81af6-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81af6-118">createdDateTime</span></span>|<span data-ttu-id="81af6-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81af6-119">dateTimeOffset</span></span>|<span data-ttu-id="81af6-120">Carimbo de data/hora UTC da mensagem raiz no formato ISO-8601.</span><span class="sxs-lookup"><span data-stu-id="81af6-120">UTC timestamp of the root message in ISO-8601 format.</span></span>|
|<span data-ttu-id="81af6-121">user</span><span class="sxs-lookup"><span data-stu-id="81af6-121">user</span></span>|<span data-ttu-id="81af6-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="81af6-122">identitySet</span></span>|<span data-ttu-id="81af6-123">O usuário que reajam à mensagem.</span><span class="sxs-lookup"><span data-stu-id="81af6-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81af6-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81af6-124">JSON representation</span></span>

<span data-ttu-id="81af6-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81af6-125">The following is a JSON representation of the resource.</span></span>

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
