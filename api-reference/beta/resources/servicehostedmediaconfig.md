---
title: tipo de recurso serviceHostedMediaConfig
description: O tipo serviceHostedMediaConfig.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: edefba3e415a50322022e4549fbecbd37da6d1da
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006540"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="ffc03-103">tipo de recurso serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="ffc03-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffc03-104">O tipo serviceHostedMediaConfig.</span><span class="sxs-lookup"><span data-stu-id="ffc03-104">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="ffc03-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ffc03-105">Properties</span></span>

| <span data-ttu-id="ffc03-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffc03-106">Property</span></span>                    | <span data-ttu-id="ffc03-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffc03-107">Type</span></span>                                                        | <span data-ttu-id="ffc03-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffc03-108">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="ffc03-109">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="ffc03-109">preFetchMedia</span></span>               | <span data-ttu-id="ffc03-110">coleção [mediaInfo](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="ffc03-110">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="ffc03-111">A lista de mídias a buscar previamente.</span><span class="sxs-lookup"><span data-stu-id="ffc03-111">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="ffc03-112">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="ffc03-112">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="ffc03-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffc03-113">Boolean</span></span>                                                     | <span data-ttu-id="ffc03-114">Remover o próprio participante do grupo de áudio padrão.</span><span class="sxs-lookup"><span data-stu-id="ffc03-114">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ffc03-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ffc03-115">JSON representation</span></span>

<span data-ttu-id="ffc03-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ffc03-116">The following is a JSON representation of the resource.</span></span>

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
