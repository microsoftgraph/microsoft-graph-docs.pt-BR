---
title: tipo de recurso de mediaStream
description: O tipo de mediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4867675da3427beb790beb240cd7bc0b86f04317
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519959"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="b0285-103">tipo de recurso de mediaStream</span><span class="sxs-lookup"><span data-stu-id="b0285-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0285-104">O tipo de mediaStream.</span><span class="sxs-lookup"><span data-stu-id="b0285-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="b0285-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0285-105">Properties</span></span>

| <span data-ttu-id="b0285-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0285-106">Property</span></span>    | <span data-ttu-id="b0285-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0285-107">Type</span></span>    | <span data-ttu-id="b0285-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0285-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="b0285-109">Direction</span><span class="sxs-lookup"><span data-stu-id="b0285-109">direction</span></span>   | <span data-ttu-id="b0285-110">String</span><span class="sxs-lookup"><span data-stu-id="b0285-110">String</span></span>  | <span data-ttu-id="b0285-111">A direção.</span><span class="sxs-lookup"><span data-stu-id="b0285-111">The direction.</span></span> <span data-ttu-id="b0285-112">Os valores possíveis são `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span><span class="sxs-lookup"><span data-stu-id="b0285-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="b0285-113">rótulo</span><span class="sxs-lookup"><span data-stu-id="b0285-113">label</span></span>       | <span data-ttu-id="b0285-114">String</span><span class="sxs-lookup"><span data-stu-id="b0285-114">String</span></span>  | <span data-ttu-id="b0285-115">O rótulo de fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="b0285-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="b0285-116">MediaType</span><span class="sxs-lookup"><span data-stu-id="b0285-116">mediaType</span></span>   | <span data-ttu-id="b0285-117">String</span><span class="sxs-lookup"><span data-stu-id="b0285-117">String</span></span>  | <span data-ttu-id="b0285-118">O tipo de mídia.</span><span class="sxs-lookup"><span data-stu-id="b0285-118">The media type.</span></span> <span data-ttu-id="b0285-119">Os valores possíveis são `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="b0285-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="b0285-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="b0285-120">serverMuted</span></span> | <span data-ttu-id="b0285-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0285-121">Boolean</span></span> | <span data-ttu-id="b0285-122">Se a mídia está sem som pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="b0285-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="b0285-123">SourceId</span><span class="sxs-lookup"><span data-stu-id="b0285-123">sourceId</span></span>    | <span data-ttu-id="b0285-124">String</span><span class="sxs-lookup"><span data-stu-id="b0285-124">String</span></span>  | <span data-ttu-id="b0285-125">A ID de origem.</span><span class="sxs-lookup"><span data-stu-id="b0285-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="b0285-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0285-126">JSON representation</span></span>

<span data-ttu-id="b0285-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0285-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

## <a name="example"></a><span data-ttu-id="b0285-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0285-128">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediastream.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
