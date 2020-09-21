---
title: tipo de recurso serviceHostedMediaConfig
description: A mídia que está hospedada remotamente.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d006a4417401859c0c385f9537656993f985198d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023951"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="65a2f-103">tipo de recurso serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="65a2f-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="65a2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65a2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65a2f-105">A mídia que está hospedada remotamente.</span><span class="sxs-lookup"><span data-stu-id="65a2f-105">The media that's hosted remotely.</span></span> <span data-ttu-id="65a2f-106">Isso é herdado de [mediaConfig](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="65a2f-106">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="65a2f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65a2f-107">Properties</span></span>

| <span data-ttu-id="65a2f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65a2f-108">Property</span></span>                    | <span data-ttu-id="65a2f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="65a2f-109">Type</span></span>                                                        | <span data-ttu-id="65a2f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="65a2f-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="65a2f-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="65a2f-111">preFetchMedia</span></span>               | <span data-ttu-id="65a2f-112">coleção [mediaInfo](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="65a2f-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="65a2f-113">A lista de mídias a buscar previamente.</span><span class="sxs-lookup"><span data-stu-id="65a2f-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="65a2f-114">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="65a2f-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="65a2f-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="65a2f-115">Boolean</span></span>                                                     | <span data-ttu-id="65a2f-116">Remover o próprio participante do grupo de áudio padrão.</span><span class="sxs-lookup"><span data-stu-id="65a2f-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="65a2f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65a2f-117">JSON representation</span></span>

<span data-ttu-id="65a2f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65a2f-118">The following is a JSON representation of the resource.</span></span>

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


