---
title: tipo de recurso mediaStream
description: Contém informações sobre o canal de mídia.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8d6bce42c31e39f5b36e3beccdac2fc660f9cb30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522754"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="1877f-103">tipo de recurso mediaStream</span><span class="sxs-lookup"><span data-stu-id="1877f-103">mediaStream resource type</span></span>

<span data-ttu-id="1877f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1877f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1877f-105">Contém informações sobre o canal de mídia.</span><span class="sxs-lookup"><span data-stu-id="1877f-105">Contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="1877f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1877f-106">Properties</span></span>

| <span data-ttu-id="1877f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1877f-107">Property</span></span>    | <span data-ttu-id="1877f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1877f-108">Type</span></span>    | <span data-ttu-id="1877f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1877f-109">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="1877f-110">direction</span><span class="sxs-lookup"><span data-stu-id="1877f-110">direction</span></span>   | <span data-ttu-id="1877f-111">String</span><span class="sxs-lookup"><span data-stu-id="1877f-111">String</span></span>  | <span data-ttu-id="1877f-112">A direção.</span><span class="sxs-lookup"><span data-stu-id="1877f-112">The direction.</span></span> <span data-ttu-id="1877f-113">Os valores possíveis são `inactive`: `sendOnly` `receiveOnly`,, `sendReceive`,.</span><span class="sxs-lookup"><span data-stu-id="1877f-113">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="1877f-114">rótulo</span><span class="sxs-lookup"><span data-stu-id="1877f-114">label</span></span>       | <span data-ttu-id="1877f-115">String</span><span class="sxs-lookup"><span data-stu-id="1877f-115">String</span></span>  | <span data-ttu-id="1877f-116">O rótulo do fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="1877f-116">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="1877f-117">Mídia</span><span class="sxs-lookup"><span data-stu-id="1877f-117">mediaType</span></span>   | <span data-ttu-id="1877f-118">String</span><span class="sxs-lookup"><span data-stu-id="1877f-118">String</span></span>  | <span data-ttu-id="1877f-119">O tipo de mídia.</span><span class="sxs-lookup"><span data-stu-id="1877f-119">The media type.</span></span> <span data-ttu-id="1877f-120">O valor possível é `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="1877f-120">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="1877f-121">serverMuted</span><span class="sxs-lookup"><span data-stu-id="1877f-121">serverMuted</span></span> | <span data-ttu-id="1877f-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="1877f-122">Boolean</span></span> | <span data-ttu-id="1877f-123">Indica se a mídia está com mudo ativado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="1877f-123">Indicates whether the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="1877f-124">sourceId</span><span class="sxs-lookup"><span data-stu-id="1877f-124">sourceId</span></span>    | <span data-ttu-id="1877f-125">String</span><span class="sxs-lookup"><span data-stu-id="1877f-125">String</span></span>  | <span data-ttu-id="1877f-126">A ID da fonte.</span><span class="sxs-lookup"><span data-stu-id="1877f-126">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="1877f-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1877f-127">JSON representation</span></span>

<span data-ttu-id="1877f-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1877f-128">The following is a JSON representation of the resource.</span></span>

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
