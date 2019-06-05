---
title: tipo de recurso chatMessageReaction
description: 'Representa uma reação a uma entidade chat. '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 33fe5a881d05b2ac2bc86e97e11b00c3465a8c09
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709422"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="cfefd-103">tipo de recurso chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="cfefd-103">chatMessageReaction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfefd-104">Representa uma reação a uma entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="cfefd-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="cfefd-105">Uma entidade do tipo `chatMessageReaction` é retornada como parte da API [obter mensagem de canal](../api/channel-get-message.md) , como parte da entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="cfefd-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="cfefd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cfefd-106">Properties</span></span>

| <span data-ttu-id="cfefd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfefd-107">Property</span></span>     | <span data-ttu-id="cfefd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfefd-108">Type</span></span>        | <span data-ttu-id="cfefd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfefd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cfefd-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfefd-110">createdDateTime</span></span>|<span data-ttu-id="cfefd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfefd-111">DateTimeOffset</span></span>|<span data-ttu-id="cfefd-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cfefd-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cfefd-114">reactiontype</span><span class="sxs-lookup"><span data-stu-id="cfefd-114">reactionType</span></span>|<span data-ttu-id="cfefd-115">String</span><span class="sxs-lookup"><span data-stu-id="cfefd-115">String</span></span>|<span data-ttu-id="cfefd-116">Os valores planejados incluem:</span><span class="sxs-lookup"><span data-stu-id="cfefd-116">Planned values include:</span></span> <br><ul><li><span data-ttu-id="cfefd-117">Semelhante a uma mensagem, o conteúdo está em branco neste caso.</span><span class="sxs-lookup"><span data-stu-id="cfefd-117">Like - Like a message, content is blank in this case.</span></span></li><li><span data-ttu-id="cfefd-118">Emoji-reação de Emoji.</span><span class="sxs-lookup"><span data-stu-id="cfefd-118">Emoji - Emoji reaction.</span></span> <span data-ttu-id="cfefd-119">O conteúdo é definido para o valor Unicode do emoji.</span><span class="sxs-lookup"><span data-stu-id="cfefd-119">Content is set to unicode value of the emoji.</span></span></li><li><span data-ttu-id="cfefd-120">Rótulo-o conteúdo é definido como a cadeia de caracteres no rótulo.</span><span class="sxs-lookup"><span data-stu-id="cfefd-120">Label - Content is set to the string in the label.</span></span></li></ul>|
|<span data-ttu-id="cfefd-121">user</span><span class="sxs-lookup"><span data-stu-id="cfefd-121">user</span></span>|[<span data-ttu-id="cfefd-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="cfefd-122">identitySet</span></span>](identityset.md)|<span data-ttu-id="cfefd-123">O usuário que reajam à mensagem.</span><span class="sxs-lookup"><span data-stu-id="cfefd-123">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cfefd-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cfefd-124">JSON representation</span></span>

<span data-ttu-id="cfefd-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cfefd-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageReaction",
  "baseType": null
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "reactionType": "String",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageReaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
