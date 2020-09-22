---
title: tipo de recurso serviceHostedMediaConfig
description: O tipo serviceHostedMediaConfig.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d4bdea6009dae0bd06ec9ffc00d00e417e7c22d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991842"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="df7c1-103">tipo de recurso serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="df7c1-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="df7c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df7c1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df7c1-105">A mídia que está hospedada remotamente.</span><span class="sxs-lookup"><span data-stu-id="df7c1-105">The media that's hosted remotely.</span></span> <span data-ttu-id="df7c1-106">Isso é herdado de [mediaConfig](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="df7c1-106">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="df7c1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df7c1-107">Properties</span></span>

| <span data-ttu-id="df7c1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df7c1-108">Property</span></span>                    | <span data-ttu-id="df7c1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="df7c1-109">Type</span></span>                                                        | <span data-ttu-id="df7c1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="df7c1-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="df7c1-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="df7c1-111">preFetchMedia</span></span>               | <span data-ttu-id="df7c1-112">coleção [mediaInfo](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="df7c1-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="df7c1-113">A lista de mídias a buscar previamente.</span><span class="sxs-lookup"><span data-stu-id="df7c1-113">The list of media to pre-fetch.</span></span>                   |


## <a name="json-representation"></a><span data-ttu-id="df7c1-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df7c1-114">JSON representation</span></span>

<span data-ttu-id="df7c1-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df7c1-115">The following is a JSON representation of the resource.</span></span>

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
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ]
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

