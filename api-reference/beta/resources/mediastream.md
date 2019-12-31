---
title: tipo de recurso mediaStream
description: Contém informações sobre o canal de mídia.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0274cdb1c35307e91e31c0b357ecf9a16e2d3f19
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913076"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="c8b71-103">tipo de recurso mediaStream</span><span class="sxs-lookup"><span data-stu-id="c8b71-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8b71-104">Contém informações sobre o canal de mídia.</span><span class="sxs-lookup"><span data-stu-id="c8b71-104">Contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="c8b71-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8b71-105">Properties</span></span>

| <span data-ttu-id="c8b71-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8b71-106">Property</span></span>    | <span data-ttu-id="c8b71-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8b71-107">Type</span></span>    | <span data-ttu-id="c8b71-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8b71-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="c8b71-109">direction</span><span class="sxs-lookup"><span data-stu-id="c8b71-109">direction</span></span>   | <span data-ttu-id="c8b71-110">String</span><span class="sxs-lookup"><span data-stu-id="c8b71-110">String</span></span>  | <span data-ttu-id="c8b71-111">A direção.</span><span class="sxs-lookup"><span data-stu-id="c8b71-111">The direction.</span></span> <span data-ttu-id="c8b71-112">Os valores possíveis são `inactive`: `sendOnly` `receiveOnly`,, `sendReceive`,.</span><span class="sxs-lookup"><span data-stu-id="c8b71-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="c8b71-113">rótulo</span><span class="sxs-lookup"><span data-stu-id="c8b71-113">label</span></span>       | <span data-ttu-id="c8b71-114">String</span><span class="sxs-lookup"><span data-stu-id="c8b71-114">String</span></span>  | <span data-ttu-id="c8b71-115">O rótulo do fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="c8b71-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="c8b71-116">Mídia</span><span class="sxs-lookup"><span data-stu-id="c8b71-116">mediaType</span></span>   | <span data-ttu-id="c8b71-117">String</span><span class="sxs-lookup"><span data-stu-id="c8b71-117">String</span></span>  | <span data-ttu-id="c8b71-118">O tipo de mídia.</span><span class="sxs-lookup"><span data-stu-id="c8b71-118">The media type.</span></span> <span data-ttu-id="c8b71-119">O valor possível é `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="c8b71-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="c8b71-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="c8b71-120">serverMuted</span></span> | <span data-ttu-id="c8b71-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="c8b71-121">Boolean</span></span> | <span data-ttu-id="c8b71-122">Indica se a mídia está com mudo ativado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="c8b71-122">Indicates whether the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="c8b71-123">sourceId</span><span class="sxs-lookup"><span data-stu-id="c8b71-123">sourceId</span></span>    | <span data-ttu-id="c8b71-124">String</span><span class="sxs-lookup"><span data-stu-id="c8b71-124">String</span></span>  | <span data-ttu-id="c8b71-125">A ID da fonte.</span><span class="sxs-lookup"><span data-stu-id="c8b71-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="c8b71-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8b71-126">JSON representation</span></span>

<span data-ttu-id="c8b71-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8b71-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted",
    "label"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
