---
title: tipo de recurso serviceHostedMediaConfig
description: A mídia que está hospedada remotamente.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 405f6b40260908d7492a3b02c8535588c8475ca8
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870086"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="cf81d-103">tipo de recurso serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="cf81d-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf81d-104">A mídia que está hospedada remotamente.</span><span class="sxs-lookup"><span data-stu-id="cf81d-104">The media that's hosted remotely.</span></span> <span data-ttu-id="cf81d-105">Isso é herdado de [mediaConfig](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="cf81d-105">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cf81d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf81d-106">Properties</span></span>

| <span data-ttu-id="cf81d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf81d-107">Property</span></span>                    | <span data-ttu-id="cf81d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf81d-108">Type</span></span>                                                        | <span data-ttu-id="cf81d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf81d-109">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="cf81d-110">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="cf81d-110">preFetchMedia</span></span>               | <span data-ttu-id="cf81d-111">coleção [mediaInfo](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="cf81d-111">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="cf81d-112">A lista de mídias a buscar previamente.</span><span class="sxs-lookup"><span data-stu-id="cf81d-112">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="cf81d-113">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="cf81d-113">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="cf81d-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf81d-114">Boolean</span></span>                                                     | <span data-ttu-id="cf81d-115">Remover o próprio participante do grupo de áudio padrão.</span><span class="sxs-lookup"><span data-stu-id="cf81d-115">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cf81d-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf81d-116">JSON representation</span></span>

<span data-ttu-id="cf81d-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf81d-117">The following is a JSON representation of the resource.</span></span>

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
