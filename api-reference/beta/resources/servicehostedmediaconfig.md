---
title: tipo de recurso de serviceHostedMediaConfig
description: O tipo de serviceHostedMediaConfig.
author: VinodRavichandran
ms.openlocfilehash: 544c1d3bce934064092e0f9c74b888686e49d426
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380314"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="9d40b-103">tipo de recurso de serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="9d40b-103">serviceHostedMediaConfig resource type</span></span>

> <span data-ttu-id="9d40b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9d40b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d40b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9d40b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d40b-106">O tipo de serviceHostedMediaConfig.</span><span class="sxs-lookup"><span data-stu-id="9d40b-106">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="9d40b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d40b-107">Properties</span></span>

| <span data-ttu-id="9d40b-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="9d40b-108">Property</span></span>                    | <span data-ttu-id="9d40b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d40b-109">Type</span></span>                                                        | <span data-ttu-id="9d40b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d40b-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="9d40b-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="9d40b-111">preFetchMedia</span></span>               | <span data-ttu-id="9d40b-112">coleção [mediaInfo](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="9d40b-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="9d40b-113">A lista de mídia para buscar previamente.</span><span class="sxs-lookup"><span data-stu-id="9d40b-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="9d40b-114">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="9d40b-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="9d40b-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="9d40b-115">Boolean</span></span>                                                     | <span data-ttu-id="9d40b-116">Remova self participante do grupo de áudio padrão.</span><span class="sxs-lookup"><span data-stu-id="9d40b-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9d40b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d40b-117">JSON representation</span></span>

<span data-ttu-id="9d40b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d40b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "#microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

## <a name="example"></a><span data-ttu-id="9d40b-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d40b-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [
    {
      "uri": "https://cdn.contoso.com/beep.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
    },
    {
      "uri": "https://cdn.contoso.com/cool.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
    }
  ],
  "removeFromDefaultAudioGroup": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
