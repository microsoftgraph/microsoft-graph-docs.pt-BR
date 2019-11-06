---
title: tipo de recurso mediaStream
description: O tipo mediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 63fad1d064c4ab967bba6df8bed6dbcdd20a3d69
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006652"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="49b39-103">tipo de recurso mediaStream</span><span class="sxs-lookup"><span data-stu-id="49b39-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49b39-104">O tipo mediaStream.</span><span class="sxs-lookup"><span data-stu-id="49b39-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="49b39-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49b39-105">Properties</span></span>

| <span data-ttu-id="49b39-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49b39-106">Property</span></span>    | <span data-ttu-id="49b39-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="49b39-107">Type</span></span>    | <span data-ttu-id="49b39-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="49b39-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="49b39-109">direction</span><span class="sxs-lookup"><span data-stu-id="49b39-109">direction</span></span>   | <span data-ttu-id="49b39-110">String</span><span class="sxs-lookup"><span data-stu-id="49b39-110">String</span></span>  | <span data-ttu-id="49b39-111">A direção.</span><span class="sxs-lookup"><span data-stu-id="49b39-111">The direction.</span></span> <span data-ttu-id="49b39-112">Os valores possíveis são `inactive`: `sendOnly` `receiveOnly`,, `sendReceive`,.</span><span class="sxs-lookup"><span data-stu-id="49b39-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="49b39-113">rótulo</span><span class="sxs-lookup"><span data-stu-id="49b39-113">label</span></span>       | <span data-ttu-id="49b39-114">String</span><span class="sxs-lookup"><span data-stu-id="49b39-114">String</span></span>  | <span data-ttu-id="49b39-115">O rótulo do fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="49b39-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="49b39-116">Mídia</span><span class="sxs-lookup"><span data-stu-id="49b39-116">mediaType</span></span>   | <span data-ttu-id="49b39-117">String</span><span class="sxs-lookup"><span data-stu-id="49b39-117">String</span></span>  | <span data-ttu-id="49b39-118">O tipo de mídia.</span><span class="sxs-lookup"><span data-stu-id="49b39-118">The media type.</span></span> <span data-ttu-id="49b39-119">O valor possível é `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="49b39-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="49b39-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="49b39-120">serverMuted</span></span> | <span data-ttu-id="49b39-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="49b39-121">Boolean</span></span> | <span data-ttu-id="49b39-122">Se a mídia estiver com mudo ativado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="49b39-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="49b39-123">sourceId</span><span class="sxs-lookup"><span data-stu-id="49b39-123">sourceId</span></span>    | <span data-ttu-id="49b39-124">String</span><span class="sxs-lookup"><span data-stu-id="49b39-124">String</span></span>  | <span data-ttu-id="49b39-125">A ID da fonte.</span><span class="sxs-lookup"><span data-stu-id="49b39-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="49b39-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49b39-126">JSON representation</span></span>

<span data-ttu-id="49b39-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49b39-127">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="49b39-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49b39-128">Example</span></span>

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
  "suppressions": []
}
-->
