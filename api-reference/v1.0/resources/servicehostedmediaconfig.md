---
title: tipo de recurso serviceHostedMediaConfig
description: O tipo serviceHostedMediaConfig.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 35d5754071aa388e300042b9977fd759a38a6b74
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912948"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="62a72-103">tipo de recurso serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="62a72-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="62a72-104">A mídia que está hospedada remotamente.</span><span class="sxs-lookup"><span data-stu-id="62a72-104">The media that's hosted remotely.</span></span> <span data-ttu-id="62a72-105">Isso é herdado de [mediaConfig](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="62a72-105">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="62a72-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62a72-106">Properties</span></span>

| <span data-ttu-id="62a72-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62a72-107">Property</span></span>                    | <span data-ttu-id="62a72-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="62a72-108">Type</span></span>                                                        | <span data-ttu-id="62a72-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="62a72-109">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="62a72-110">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="62a72-110">preFetchMedia</span></span>               | <span data-ttu-id="62a72-111">coleção [mediaInfo](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="62a72-111">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="62a72-112">A lista de mídias a buscar previamente.</span><span class="sxs-lookup"><span data-stu-id="62a72-112">The list of media to pre-fetch.</span></span>                   |


## <a name="json-representation"></a><span data-ttu-id="62a72-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62a72-113">JSON representation</span></span>

<span data-ttu-id="62a72-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62a72-114">The following is a JSON representation of the resource.</span></span>

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
