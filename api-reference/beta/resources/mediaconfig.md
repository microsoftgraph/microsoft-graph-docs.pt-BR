---
title: tipo de recurso de mediaConfig
description: A configuração de mídia usada para conectar a uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e4f6e940cd319d10cd3f03e3c94d0473164beb29
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642615"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="3d53d-103">tipo de recurso de mediaConfig</span><span class="sxs-lookup"><span data-stu-id="3d53d-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d53d-104">A configuração de mídia usada para conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="3d53d-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="3d53d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d53d-105">Properties</span></span>

| <span data-ttu-id="3d53d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d53d-106">Property</span></span>       | <span data-ttu-id="3d53d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d53d-107">Type</span></span>    | <span data-ttu-id="3d53d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d53d-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3d53d-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="3d53d-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="3d53d-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="3d53d-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="3d53d-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d53d-111">JSON representation</span></span>

<span data-ttu-id="3d53d-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d53d-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
  ],
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediaconfig.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
