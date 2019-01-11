---
title: tipo de recurso de serviceHostedMediaConfig
description: O tipo de serviceHostedMediaConfig.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: ec2ff24ef0bb45a9b49ecf2d0dc5e7419318b5af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828697"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="e111f-103">tipo de recurso de serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="e111f-103">serviceHostedMediaConfig resource type</span></span>

> <span data-ttu-id="e111f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e111f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e111f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e111f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e111f-106">O tipo de serviceHostedMediaConfig.</span><span class="sxs-lookup"><span data-stu-id="e111f-106">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="e111f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e111f-107">Properties</span></span>

| <span data-ttu-id="e111f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e111f-108">Property</span></span>                    | <span data-ttu-id="e111f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e111f-109">Type</span></span>                                                        | <span data-ttu-id="e111f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e111f-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="e111f-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="e111f-111">preFetchMedia</span></span>               | <span data-ttu-id="e111f-112">coleção [mediaInfo](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="e111f-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="e111f-113">A lista de mídia para buscar previamente.</span><span class="sxs-lookup"><span data-stu-id="e111f-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="e111f-114">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="e111f-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="e111f-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="e111f-115">Boolean</span></span>                                                     | <span data-ttu-id="e111f-116">Remova self participante do grupo de áudio padrão.</span><span class="sxs-lookup"><span data-stu-id="e111f-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e111f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e111f-117">JSON representation</span></span>

<span data-ttu-id="e111f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e111f-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="e111f-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e111f-119">Example</span></span>

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
