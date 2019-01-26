---
title: tipo de recurso de mediaConfig
description: A configuração de mídia usada para conectar a uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0b2d8b8063307660b0d4cce459e1906f0b0a99c5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573960"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="5080f-103">tipo de recurso de mediaConfig</span><span class="sxs-lookup"><span data-stu-id="5080f-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5080f-104">A configuração de mídia usada para conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="5080f-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="5080f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5080f-105">Properties</span></span>

| <span data-ttu-id="5080f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5080f-106">Property</span></span>       | <span data-ttu-id="5080f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5080f-107">Type</span></span>    | <span data-ttu-id="5080f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5080f-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5080f-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="5080f-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="5080f-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="5080f-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="5080f-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5080f-111">JSON representation</span></span>

<span data-ttu-id="5080f-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5080f-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
  ],
  "abstract": true,
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
