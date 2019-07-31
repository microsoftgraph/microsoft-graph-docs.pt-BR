---
title: tipo de recurso mediaStream
description: O tipo mediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c39c4eb0754f327361fec04852293ef084b0c412
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966822"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="35640-103">tipo de recurso mediaStream</span><span class="sxs-lookup"><span data-stu-id="35640-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35640-104">O tipo mediaStream.</span><span class="sxs-lookup"><span data-stu-id="35640-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="35640-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35640-105">Properties</span></span>

| <span data-ttu-id="35640-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35640-106">Property</span></span>    | <span data-ttu-id="35640-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="35640-107">Type</span></span>    | <span data-ttu-id="35640-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="35640-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="35640-109">direction</span><span class="sxs-lookup"><span data-stu-id="35640-109">direction</span></span>   | <span data-ttu-id="35640-110">String</span><span class="sxs-lookup"><span data-stu-id="35640-110">String</span></span>  | <span data-ttu-id="35640-111">A direção.</span><span class="sxs-lookup"><span data-stu-id="35640-111">The direction.</span></span> <span data-ttu-id="35640-112">Os valores possíveis são `inactive`: `sendOnly` `receiveOnly`,, `sendReceive`,.</span><span class="sxs-lookup"><span data-stu-id="35640-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="35640-113">rótulo</span><span class="sxs-lookup"><span data-stu-id="35640-113">label</span></span>       | <span data-ttu-id="35640-114">String</span><span class="sxs-lookup"><span data-stu-id="35640-114">String</span></span>  | <span data-ttu-id="35640-115">O rótulo do fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="35640-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="35640-116">Mídia</span><span class="sxs-lookup"><span data-stu-id="35640-116">mediaType</span></span>   | <span data-ttu-id="35640-117">String</span><span class="sxs-lookup"><span data-stu-id="35640-117">String</span></span>  | <span data-ttu-id="35640-118">O tipo de mídia.</span><span class="sxs-lookup"><span data-stu-id="35640-118">The media type.</span></span> <span data-ttu-id="35640-119">O valor possível é `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="35640-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="35640-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="35640-120">serverMuted</span></span> | <span data-ttu-id="35640-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="35640-121">Boolean</span></span> | <span data-ttu-id="35640-122">Se a mídia estiver com mudo ativado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="35640-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="35640-123">sourceId</span><span class="sxs-lookup"><span data-stu-id="35640-123">sourceId</span></span>    | <span data-ttu-id="35640-124">String</span><span class="sxs-lookup"><span data-stu-id="35640-124">String</span></span>  | <span data-ttu-id="35640-125">A ID da fonte.</span><span class="sxs-lookup"><span data-stu-id="35640-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="35640-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35640-126">JSON representation</span></span>

<span data-ttu-id="35640-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35640-127">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="35640-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35640-128">Example</span></span>

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
