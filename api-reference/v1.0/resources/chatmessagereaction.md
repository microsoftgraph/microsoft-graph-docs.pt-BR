---
title: Tipo de recurso chatMessageReaction
description: 'Representa uma reação a uma entidade chatMessage. '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: e696069b9913b89fafea178c7cf95e099e288c46
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582873"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="83653-103">Tipo de recurso chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="83653-103">chatMessageReaction resource type</span></span>

<span data-ttu-id="83653-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83653-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83653-105">Representa uma reação a uma [entidade chatMessage.](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="83653-105">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="83653-106">Uma entidade de tipo é retornada como parte da API de mensagem get `chatMessageReaction` [channel,](../api/chatmessage-get.md) como parte da [entidade chatMessage.](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="83653-106">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/chatmessage-get.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="83653-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83653-107">Properties</span></span>

| <span data-ttu-id="83653-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83653-108">Property</span></span>     | <span data-ttu-id="83653-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="83653-109">Type</span></span>        | <span data-ttu-id="83653-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="83653-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="83653-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83653-111">createdDateTime</span></span>|<span data-ttu-id="83653-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83653-112">DateTimeOffset</span></span>|<span data-ttu-id="83653-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="83653-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="83653-114">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="83653-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="83653-115">reactionType</span><span class="sxs-lookup"><span data-stu-id="83653-115">reactionType</span></span>|<span data-ttu-id="83653-116">String</span><span class="sxs-lookup"><span data-stu-id="83653-116">String</span></span>|<span data-ttu-id="83653-117">Os valores suportados `like` são , , , , , `angry` `sad` `laugh` `heart` `surprised` .</span><span class="sxs-lookup"><span data-stu-id="83653-117">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="83653-118">usuário</span><span class="sxs-lookup"><span data-stu-id="83653-118">user</span></span>|[<span data-ttu-id="83653-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="83653-119">identitySet</span></span>](identityset.md)|<span data-ttu-id="83653-120">O usuário que reagia à mensagem.</span><span class="sxs-lookup"><span data-stu-id="83653-120">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83653-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83653-121">JSON representation</span></span>

<span data-ttu-id="83653-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83653-122">The following is a JSON representation of the resource.</span></span>

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


