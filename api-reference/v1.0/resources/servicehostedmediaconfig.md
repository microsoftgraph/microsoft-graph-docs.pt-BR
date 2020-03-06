---
title: tipo de recurso serviceHostedMediaConfig
description: O tipo serviceHostedMediaConfig.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7f43d529e2fc18ddf67876737c07a66c606db560
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533747"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="2874f-103">tipo de recurso serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="2874f-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="2874f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2874f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2874f-105">A mídia que está hospedada remotamente.</span><span class="sxs-lookup"><span data-stu-id="2874f-105">The media that's hosted remotely.</span></span> <span data-ttu-id="2874f-106">Isso é herdado de [mediaConfig](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="2874f-106">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2874f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2874f-107">Properties</span></span>

| <span data-ttu-id="2874f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2874f-108">Property</span></span>                    | <span data-ttu-id="2874f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2874f-109">Type</span></span>                                                        | <span data-ttu-id="2874f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2874f-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="2874f-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="2874f-111">preFetchMedia</span></span>               | <span data-ttu-id="2874f-112">coleção [mediaInfo](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="2874f-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="2874f-113">A lista de mídias a buscar previamente.</span><span class="sxs-lookup"><span data-stu-id="2874f-113">The list of media to pre-fetch.</span></span>                   |


## <a name="json-representation"></a><span data-ttu-id="2874f-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2874f-114">JSON representation</span></span>

<span data-ttu-id="2874f-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2874f-115">The following is a JSON representation of the resource.</span></span>

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
