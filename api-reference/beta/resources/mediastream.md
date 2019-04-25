---
title: tipo de recurso mediaStream
description: O tipo mediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4867675da3427beb790beb240cd7bc0b86f04317
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581526"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="c3c4a-103">tipo de recurso mediaStream</span><span class="sxs-lookup"><span data-stu-id="c3c4a-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3c4a-104">O tipo mediaStream.</span><span class="sxs-lookup"><span data-stu-id="c3c4a-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="c3c4a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3c4a-105">Properties</span></span>

| <span data-ttu-id="c3c4a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3c4a-106">Property</span></span>    | <span data-ttu-id="c3c4a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3c4a-107">Type</span></span>    | <span data-ttu-id="c3c4a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3c4a-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="c3c4a-109">direction</span><span class="sxs-lookup"><span data-stu-id="c3c4a-109">direction</span></span>   | <span data-ttu-id="c3c4a-110">String</span><span class="sxs-lookup"><span data-stu-id="c3c4a-110">String</span></span>  | <span data-ttu-id="c3c4a-111">A direção.</span><span class="sxs-lookup"><span data-stu-id="c3c4a-111">The direction.</span></span> <span data-ttu-id="c3c4a-112">Os valores possíveis são `inactive`: `sendOnly` `receiveOnly`,, `sendReceive`,.</span><span class="sxs-lookup"><span data-stu-id="c3c4a-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="c3c4a-113">rótulo</span><span class="sxs-lookup"><span data-stu-id="c3c4a-113">label</span></span>       | <span data-ttu-id="c3c4a-114">String</span><span class="sxs-lookup"><span data-stu-id="c3c4a-114">String</span></span>  | <span data-ttu-id="c3c4a-115">O rótulo do fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="c3c4a-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="c3c4a-116">Mídia</span><span class="sxs-lookup"><span data-stu-id="c3c4a-116">mediaType</span></span>   | <span data-ttu-id="c3c4a-117">String</span><span class="sxs-lookup"><span data-stu-id="c3c4a-117">String</span></span>  | <span data-ttu-id="c3c4a-118">O tipo de mídia.</span><span class="sxs-lookup"><span data-stu-id="c3c4a-118">The media type.</span></span> <span data-ttu-id="c3c4a-119">O valor possível é `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="c3c4a-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="c3c4a-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="c3c4a-120">serverMuted</span></span> | <span data-ttu-id="c3c4a-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3c4a-121">Boolean</span></span> | <span data-ttu-id="c3c4a-122">Se a mídia estiver com mudo ativado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="c3c4a-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="c3c4a-123">sourceId</span><span class="sxs-lookup"><span data-stu-id="c3c4a-123">sourceId</span></span>    | <span data-ttu-id="c3c4a-124">String</span><span class="sxs-lookup"><span data-stu-id="c3c4a-124">String</span></span>  | <span data-ttu-id="c3c4a-125">A ID da fonte.</span><span class="sxs-lookup"><span data-stu-id="c3c4a-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="c3c4a-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3c4a-126">JSON representation</span></span>

<span data-ttu-id="c3c4a-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3c4a-127">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="c3c4a-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3c4a-128">Example</span></span>

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
