---
title: tipo de recurso chatMessageReaction
description: 'Representa uma reação a uma entidade chat. '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dd1eac9a4630e097f06cf99f30d371de9e32eb5f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991489"
---
# <a name="chatmessagereaction-resource-type"></a><span data-ttu-id="43c9d-103">tipo de recurso chatMessageReaction</span><span class="sxs-lookup"><span data-stu-id="43c9d-103">chatMessageReaction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43c9d-104">Representa uma reação a uma entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="43c9d-104">Represents a reaction to a [chatMessage](chatmessage.md) entity.</span></span> 

<span data-ttu-id="43c9d-105">Uma entidade do tipo `chatMessageReaction` é retornada como parte da API [obter mensagem de canal](../api/channel-get-message.md) , como parte da entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="43c9d-105">An entity of type `chatMessageReaction` is returned as part of the [Get channel message](../api/channel-get-message.md) API, as a part of the [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="43c9d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43c9d-106">Properties</span></span>

| <span data-ttu-id="43c9d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43c9d-107">Property</span></span>     | <span data-ttu-id="43c9d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="43c9d-108">Type</span></span>        | <span data-ttu-id="43c9d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="43c9d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="43c9d-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43c9d-110">createdDateTime</span></span>|<span data-ttu-id="43c9d-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43c9d-111">DateTimeOffset</span></span>|<span data-ttu-id="43c9d-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="43c9d-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="43c9d-114">reactiontype</span><span class="sxs-lookup"><span data-stu-id="43c9d-114">reactionType</span></span>|<span data-ttu-id="43c9d-115">String</span><span class="sxs-lookup"><span data-stu-id="43c9d-115">String</span></span>|<span data-ttu-id="43c9d-116">Os valores com `like`suporte `angry`são `sad`, `laugh` `heart`,, `surprised`,.</span><span class="sxs-lookup"><span data-stu-id="43c9d-116">Supported values are `like`, `angry`, `sad`, `laugh`, `heart`, `surprised`.</span></span> |
|<span data-ttu-id="43c9d-117">user</span><span class="sxs-lookup"><span data-stu-id="43c9d-117">user</span></span>|[<span data-ttu-id="43c9d-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="43c9d-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="43c9d-119">O usuário que reajam à mensagem.</span><span class="sxs-lookup"><span data-stu-id="43c9d-119">The user who reacted to the message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43c9d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43c9d-120">JSON representation</span></span>

<span data-ttu-id="43c9d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43c9d-121">The following is a JSON representation of the resource.</span></span>

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
