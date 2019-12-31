---
title: tipo de recurso mediaStream
description: O tipo mediaStream.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ed564f4789a88092e34b8f8b4b0db8db63b48f2f
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913650"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="fe303-103">tipo de recurso mediaStream</span><span class="sxs-lookup"><span data-stu-id="fe303-103">mediaStream resource type</span></span>

<span data-ttu-id="fe303-104">Contém informações sobre o canal de mídia.</span><span class="sxs-lookup"><span data-stu-id="fe303-104">This contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="fe303-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe303-105">Properties</span></span>

| <span data-ttu-id="fe303-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe303-106">Property</span></span>    | <span data-ttu-id="fe303-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe303-107">Type</span></span>    | <span data-ttu-id="fe303-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe303-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="fe303-109">direction</span><span class="sxs-lookup"><span data-stu-id="fe303-109">direction</span></span>   | <span data-ttu-id="fe303-110">String</span><span class="sxs-lookup"><span data-stu-id="fe303-110">String</span></span>  | <span data-ttu-id="fe303-111">A direção.</span><span class="sxs-lookup"><span data-stu-id="fe303-111">The direction.</span></span> <span data-ttu-id="fe303-112">Os valores possíveis são `inactive`: `sendOnly` `receiveOnly`,, `sendReceive`,.</span><span class="sxs-lookup"><span data-stu-id="fe303-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="fe303-113">rótulo</span><span class="sxs-lookup"><span data-stu-id="fe303-113">label</span></span>       | <span data-ttu-id="fe303-114">String</span><span class="sxs-lookup"><span data-stu-id="fe303-114">String</span></span>  | <span data-ttu-id="fe303-115">O rótulo do fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="fe303-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="fe303-116">Mídia</span><span class="sxs-lookup"><span data-stu-id="fe303-116">mediaType</span></span>   | <span data-ttu-id="fe303-117">String</span><span class="sxs-lookup"><span data-stu-id="fe303-117">String</span></span>  | <span data-ttu-id="fe303-118">O tipo de mídia.</span><span class="sxs-lookup"><span data-stu-id="fe303-118">The media type.</span></span> <span data-ttu-id="fe303-119">O valor possível é `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="fe303-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="fe303-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="fe303-120">serverMuted</span></span> | <span data-ttu-id="fe303-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="fe303-121">Boolean</span></span> | <span data-ttu-id="fe303-122">Se a mídia estiver com mudo ativado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="fe303-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="fe303-123">sourceId</span><span class="sxs-lookup"><span data-stu-id="fe303-123">sourceId</span></span>    | <span data-ttu-id="fe303-124">String</span><span class="sxs-lookup"><span data-stu-id="fe303-124">String</span></span>  | <span data-ttu-id="fe303-125">A ID da fonte.</span><span class="sxs-lookup"><span data-stu-id="fe303-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="fe303-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe303-126">JSON representation</span></span>

<span data-ttu-id="fe303-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe303-127">The following is a JSON representation of the resource.</span></span>

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
