---
title: Tipo de recurso chatMessageReaction
description: 'Representa uma reação a uma entidade chatMessage. '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: 64e3e74102551a91f99120c7384a482f0b07e304
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208138"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="44296-103">Tipo de recurso chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="44296-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="44296-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44296-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44296-105">Representa uma reação a uma [entidade chatMessage.](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="44296-105">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="44296-106">Uma entidade de tipo é retornada como parte da API de mensagem get `chatMessageReaction` [channel,](../api/chatmessage-get.md) como parte da [entidade chatMessage.](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="44296-106">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/chatmessage-get.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="44296-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44296-107">Properties</span></span>

| <span data-ttu-id="44296-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44296-108">Property</span></span>     | <span data-ttu-id="44296-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="44296-109">Type</span></span>        | <span data-ttu-id="44296-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="44296-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="44296-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44296-111">createdDateTime</span></span>|<span data-ttu-id="44296-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44296-112">DateTimeOffset</span></span>|<span data-ttu-id="44296-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="44296-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="44296-114">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="44296-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="44296-115">reactionType</span><span class="sxs-lookup"><span data-stu-id="44296-115">reactionType</span></span>|<span data-ttu-id="44296-116">String</span><span class="sxs-lookup"><span data-stu-id="44296-116">String</span></span>|<span data-ttu-id="44296-117">Os valores suportados `like` são , , , , , `angry` `sad` `laugh` `heart` `surprised` .</span><span class="sxs-lookup"><span data-stu-id="44296-117">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="44296-118">user</span><span class="sxs-lookup"><span data-stu-id="44296-118">user</span></span>|[<span data-ttu-id="44296-119">chatMessageReactionIdentitySet</span><span class="sxs-lookup"><span data-stu-id="44296-119">chatMessageReactionIdentitySet</span></span>](chatmessagereactionidentityset.md)|<span data-ttu-id="44296-120">O usuário que reagia à mensagem.</span><span class="sxs-lookup"><span data-stu-id="44296-120">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44296-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44296-121">JSON representation</span></span>

<span data-ttu-id="44296-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44296-122">The following is a JSON representation of the resource.</span></span>

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
  "user": {"@odata.type": "microsoft.graph.chatMessageReactionIdentitySet"}
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


