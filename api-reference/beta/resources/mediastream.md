---
title: tipo de recurso mediaStream
description: Contém informações sobre o canal de mídia.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 37ed8ce10f62888a7bf1be67f489c6b8a0b95c76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971731"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="faa4b-103">tipo de recurso mediaStream</span><span class="sxs-lookup"><span data-stu-id="faa4b-103">mediaStream resource type</span></span>

<span data-ttu-id="faa4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="faa4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="faa4b-105">Contém informações sobre o canal de mídia.</span><span class="sxs-lookup"><span data-stu-id="faa4b-105">Contains information about the media channel.</span></span>

## <a name="properties"></a><span data-ttu-id="faa4b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="faa4b-106">Properties</span></span>

| <span data-ttu-id="faa4b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faa4b-107">Property</span></span>    | <span data-ttu-id="faa4b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="faa4b-108">Type</span></span>    | <span data-ttu-id="faa4b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="faa4b-109">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="faa4b-110">direction</span><span class="sxs-lookup"><span data-stu-id="faa4b-110">direction</span></span>   | <span data-ttu-id="faa4b-111">String</span><span class="sxs-lookup"><span data-stu-id="faa4b-111">String</span></span>  | <span data-ttu-id="faa4b-112">A direção.</span><span class="sxs-lookup"><span data-stu-id="faa4b-112">The direction.</span></span> <span data-ttu-id="faa4b-113">Os valores possíveis são:,,, `inactive` `sendOnly` `receiveOnly` `sendReceive` .</span><span class="sxs-lookup"><span data-stu-id="faa4b-113">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="faa4b-114">rótulo</span><span class="sxs-lookup"><span data-stu-id="faa4b-114">label</span></span>       | <span data-ttu-id="faa4b-115">String</span><span class="sxs-lookup"><span data-stu-id="faa4b-115">String</span></span>  | <span data-ttu-id="faa4b-116">O rótulo do fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="faa4b-116">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="faa4b-117">mediaType</span><span class="sxs-lookup"><span data-stu-id="faa4b-117">mediaType</span></span>   | <span data-ttu-id="faa4b-118">String</span><span class="sxs-lookup"><span data-stu-id="faa4b-118">String</span></span>  | <span data-ttu-id="faa4b-119">O tipo de mídia.</span><span class="sxs-lookup"><span data-stu-id="faa4b-119">The media type.</span></span> <span data-ttu-id="faa4b-120">O valor possível é `unknown` , `audio` , `video` , `videoBasedScreenSharing` , `data` .</span><span class="sxs-lookup"><span data-stu-id="faa4b-120">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="faa4b-121">serverMuted</span><span class="sxs-lookup"><span data-stu-id="faa4b-121">serverMuted</span></span> | <span data-ttu-id="faa4b-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="faa4b-122">Boolean</span></span> | <span data-ttu-id="faa4b-123">Indica se a mídia está com mudo ativado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="faa4b-123">Indicates whether the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="faa4b-124">sourceId</span><span class="sxs-lookup"><span data-stu-id="faa4b-124">sourceId</span></span>    | <span data-ttu-id="faa4b-125">String</span><span class="sxs-lookup"><span data-stu-id="faa4b-125">String</span></span>  | <span data-ttu-id="faa4b-126">A ID da fonte.</span><span class="sxs-lookup"><span data-stu-id="faa4b-126">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="faa4b-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="faa4b-127">JSON representation</span></span>

<span data-ttu-id="faa4b-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="faa4b-128">The following is a JSON representation of the resource.</span></span>

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


