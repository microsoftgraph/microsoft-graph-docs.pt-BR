---
title: tipo de recurso serviceHostedMediaConfig
description: O tipo serviceHostedMediaConfig.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 590eef4c572695188e609133f5bc852fd90c51f7
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865643"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="a9d74-103">tipo de recurso serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="a9d74-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="a9d74-104">A mídia que está hospedada remotamente.</span><span class="sxs-lookup"><span data-stu-id="a9d74-104">The media that's hosted remotely.</span></span> <span data-ttu-id="a9d74-105">Isso é herdado de [mediaConfig](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="a9d74-105">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a9d74-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9d74-106">Properties</span></span>

| <span data-ttu-id="a9d74-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9d74-107">Property</span></span>                    | <span data-ttu-id="a9d74-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9d74-108">Type</span></span>                                                        | <span data-ttu-id="a9d74-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9d74-109">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="a9d74-110">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="a9d74-110">preFetchMedia</span></span>               | <span data-ttu-id="a9d74-111">coleção [mediaInfo](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="a9d74-111">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="a9d74-112">A lista de mídias a buscar previamente.</span><span class="sxs-lookup"><span data-stu-id="a9d74-112">The list of media to pre-fetch.</span></span>                   |


## <a name="json-representation"></a><span data-ttu-id="a9d74-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9d74-113">JSON representation</span></span>

<span data-ttu-id="a9d74-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9d74-114">The following is a JSON representation of the resource.</span></span>

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
