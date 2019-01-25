---
title: tipo de recurso de mediaPrompt
description: O tipo de mediaPrompt.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b87af39d6d6ac4879aba44573b920a43d4f92145
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508528"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="23a6b-103">tipo de recurso de mediaPrompt</span><span class="sxs-lookup"><span data-stu-id="23a6b-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23a6b-104">O tipo de mediaPrompt.</span><span class="sxs-lookup"><span data-stu-id="23a6b-104">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="23a6b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23a6b-105">Properties</span></span>

| <span data-ttu-id="23a6b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23a6b-106">Property</span></span>    | <span data-ttu-id="23a6b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="23a6b-107">Type</span></span>                      | <span data-ttu-id="23a6b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="23a6b-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="23a6b-109">Loop</span><span class="sxs-lookup"><span data-stu-id="23a6b-109">loop</span></span>        | <span data-ttu-id="23a6b-110">Int32</span><span class="sxs-lookup"><span data-stu-id="23a6b-110">Int32</span></span>                     | <span data-ttu-id="23a6b-111">A contagem de loop.</span><span class="sxs-lookup"><span data-stu-id="23a6b-111">The loop count.</span></span> <span data-ttu-id="23a6b-112">o valor 0 indica para executar um loop indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="23a6b-112">0 value indicates to loop infinitely.</span></span> <span data-ttu-id="23a6b-113">O valor padrão é `1`.</span><span class="sxs-lookup"><span data-stu-id="23a6b-113">The default value is `1`.</span></span> |
| <span data-ttu-id="23a6b-114">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="23a6b-114">mediaInfo</span></span>   | [<span data-ttu-id="23a6b-115">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="23a6b-115">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="23a6b-116">As informações de mídia</span><span class="sxs-lookup"><span data-stu-id="23a6b-116">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="23a6b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23a6b-117">JSON representation</span></span>

<span data-ttu-id="23a6b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23a6b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "loop": 1024,
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="23a6b-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23a6b-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "mediaInfo": {
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  },
  "loop": 5
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediaprompt.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
