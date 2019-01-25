---
title: tipo de recurso de noMediaConfig
description: Configuração de mídia para não indicando nenhuma mídia.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8d564493889cc367ecdb697ce4031c40a4cbbbef
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526869"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="fd8d8-103">tipo de recurso de noMediaConfig</span><span class="sxs-lookup"><span data-stu-id="fd8d8-103">noMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd8d8-104">Configuração de mídia para não indicando nenhuma mídia.</span><span class="sxs-lookup"><span data-stu-id="fd8d8-104">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="fd8d8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd8d8-105">Properties</span></span>

| <span data-ttu-id="fd8d8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd8d8-106">Property</span></span>       | <span data-ttu-id="fd8d8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd8d8-107">Type</span></span>    | <span data-ttu-id="fd8d8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd8d8-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fd8d8-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="fd8d8-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="fd8d8-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="fd8d8-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="fd8d8-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd8d8-111">JSON representation</span></span>

<span data-ttu-id="fd8d8-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd8d8-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.noMediaConfig"
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
  "description": "noMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/nomediaconfig.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
