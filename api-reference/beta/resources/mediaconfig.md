---
title: tipo de recurso de mediaConfig
description: A configuração de mídia usada para conectar a uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e4f6e940cd319d10cd3f03e3c94d0473164beb29
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515101"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="bcee9-103">tipo de recurso de mediaConfig</span><span class="sxs-lookup"><span data-stu-id="bcee9-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcee9-104">A configuração de mídia usada para conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="bcee9-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="bcee9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bcee9-105">Properties</span></span>

| <span data-ttu-id="bcee9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcee9-106">Property</span></span>       | <span data-ttu-id="bcee9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcee9-107">Type</span></span>    | <span data-ttu-id="bcee9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcee9-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bcee9-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="bcee9-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="bcee9-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="bcee9-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="bcee9-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bcee9-111">JSON representation</span></span>

<span data-ttu-id="bcee9-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bcee9-112">The following is a JSON representation of the resource.</span></span>

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
