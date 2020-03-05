---
title: tipo de recurso chatMessageReaction
description: 'Representa uma reação a uma entidade chat. '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: cb26a46a3669b721184399036fa80e4a6b291ec8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507688"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="27a8b-103">tipo de recurso chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="27a8b-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="27a8b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="27a8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27a8b-105">Representa uma reação a uma entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="27a8b-105">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="27a8b-106">Uma entidade do tipo `chatMessageReaction` é retornada como parte da API [obter mensagem de canal](../api/channel-get-message.md) , como parte da entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="27a8b-106">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="27a8b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27a8b-107">Properties</span></span>

| <span data-ttu-id="27a8b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27a8b-108">Property</span></span>     | <span data-ttu-id="27a8b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="27a8b-109">Type</span></span>        | <span data-ttu-id="27a8b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="27a8b-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="27a8b-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27a8b-111">createdDateTime</span></span>|<span data-ttu-id="27a8b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27a8b-112">DateTimeOffset</span></span>|<span data-ttu-id="27a8b-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="27a8b-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="27a8b-115">reactiontype</span><span class="sxs-lookup"><span data-stu-id="27a8b-115">reactionType</span></span>|<span data-ttu-id="27a8b-116">String</span><span class="sxs-lookup"><span data-stu-id="27a8b-116">String</span></span>|<span data-ttu-id="27a8b-117">Os valores com `like`suporte `angry`são `sad`, `laugh` `heart`,, `surprised`,.</span><span class="sxs-lookup"><span data-stu-id="27a8b-117">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="27a8b-118">user</span><span class="sxs-lookup"><span data-stu-id="27a8b-118">user</span></span>|[<span data-ttu-id="27a8b-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="27a8b-119">identitySet</span></span>](identityset.md)|<span data-ttu-id="27a8b-120">O usuário que reajam à mensagem.</span><span class="sxs-lookup"><span data-stu-id="27a8b-120">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27a8b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27a8b-121">JSON representation</span></span>

<span data-ttu-id="27a8b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27a8b-122">The following is a JSON representation of the resource.</span></span>

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
