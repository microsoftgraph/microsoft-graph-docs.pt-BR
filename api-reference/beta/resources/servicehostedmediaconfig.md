---
title: tipo de recurso de serviceHostedMediaConfig
description: O tipo de serviceHostedMediaConfig.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 127450b569a37f00a76696a749c269f55c15b7aa
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572448"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="d0d47-103">tipo de recurso de serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="d0d47-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0d47-104">O tipo de serviceHostedMediaConfig.</span><span class="sxs-lookup"><span data-stu-id="d0d47-104">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="d0d47-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0d47-105">Properties</span></span>

| <span data-ttu-id="d0d47-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0d47-106">Property</span></span>                    | <span data-ttu-id="d0d47-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0d47-107">Type</span></span>                                                        | <span data-ttu-id="d0d47-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0d47-108">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="d0d47-109">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="d0d47-109">preFetchMedia</span></span>               | <span data-ttu-id="d0d47-110">coleção [mediaInfo](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="d0d47-110">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="d0d47-111">A lista de mídia para buscar previamente.</span><span class="sxs-lookup"><span data-stu-id="d0d47-111">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="d0d47-112">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="d0d47-112">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="d0d47-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0d47-113">Boolean</span></span>                                                     | <span data-ttu-id="d0d47-114">Remova self participante do grupo de áudio padrão.</span><span class="sxs-lookup"><span data-stu-id="d0d47-114">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d0d47-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0d47-115">JSON representation</span></span>

<span data-ttu-id="d0d47-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0d47-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
   "baseType":"microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

## <a name="example"></a><span data-ttu-id="d0d47-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0d47-117">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/servicehostedmediaconfig.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
