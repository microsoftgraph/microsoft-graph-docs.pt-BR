---
title: tipo de recurso serviceHostedMediaConfig
description: A mídia que está hospedada remotamente.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 16db7e17e48ce8f257d9b6a1bfd296ca06bd0634
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520791"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="87265-103">tipo de recurso serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="87265-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="87265-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="87265-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87265-105">A mídia que está hospedada remotamente.</span><span class="sxs-lookup"><span data-stu-id="87265-105">The media that's hosted remotely.</span></span> <span data-ttu-id="87265-106">Isso é herdado de [mediaConfig](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="87265-106">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="87265-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87265-107">Properties</span></span>

| <span data-ttu-id="87265-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87265-108">Property</span></span>                    | <span data-ttu-id="87265-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="87265-109">Type</span></span>                                                        | <span data-ttu-id="87265-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="87265-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="87265-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="87265-111">preFetchMedia</span></span>               | <span data-ttu-id="87265-112">coleção [mediaInfo](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="87265-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="87265-113">A lista de mídias a buscar previamente.</span><span class="sxs-lookup"><span data-stu-id="87265-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="87265-114">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="87265-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="87265-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="87265-115">Boolean</span></span>                                                     | <span data-ttu-id="87265-116">Remover o próprio participante do grupo de áudio padrão.</span><span class="sxs-lookup"><span data-stu-id="87265-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87265-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87265-117">JSON representation</span></span>

<span data-ttu-id="87265-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87265-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
