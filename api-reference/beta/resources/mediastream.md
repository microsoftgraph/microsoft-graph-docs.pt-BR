---
title: tipo de recurso de mediaStream
description: O tipo de mediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd003bde0eca5fd21cb12c23d5c83699a6b79c8e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916961"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="a5a9f-103">tipo de recurso de mediaStream</span><span class="sxs-lookup"><span data-stu-id="a5a9f-103">mediaStream resource type</span></span>

> <span data-ttu-id="a5a9f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5a9f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5a9f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5a9f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5a9f-106">O tipo de mediaStream.</span><span class="sxs-lookup"><span data-stu-id="a5a9f-106">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="a5a9f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5a9f-107">Properties</span></span>

| <span data-ttu-id="a5a9f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5a9f-108">Property</span></span>    | <span data-ttu-id="a5a9f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5a9f-109">Type</span></span>    | <span data-ttu-id="a5a9f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5a9f-110">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="a5a9f-111">direção</span><span class="sxs-lookup"><span data-stu-id="a5a9f-111">direction</span></span>   | <span data-ttu-id="a5a9f-112">String</span><span class="sxs-lookup"><span data-stu-id="a5a9f-112">String</span></span>  | <span data-ttu-id="a5a9f-113">A direção.</span><span class="sxs-lookup"><span data-stu-id="a5a9f-113">The direction.</span></span> <span data-ttu-id="a5a9f-114">Os valores possíveis são `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span><span class="sxs-lookup"><span data-stu-id="a5a9f-114">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="a5a9f-115">rótulo</span><span class="sxs-lookup"><span data-stu-id="a5a9f-115">label</span></span>       | <span data-ttu-id="a5a9f-116">String</span><span class="sxs-lookup"><span data-stu-id="a5a9f-116">String</span></span>  | <span data-ttu-id="a5a9f-117">O rótulo de fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="a5a9f-117">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="a5a9f-118">mediaType</span><span class="sxs-lookup"><span data-stu-id="a5a9f-118">mediaType</span></span>   | <span data-ttu-id="a5a9f-119">String</span><span class="sxs-lookup"><span data-stu-id="a5a9f-119">String</span></span>  | <span data-ttu-id="a5a9f-120">O tipo de mídia.</span><span class="sxs-lookup"><span data-stu-id="a5a9f-120">The media type.</span></span> <span data-ttu-id="a5a9f-121">Os valores possíveis são `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="a5a9f-121">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="a5a9f-122">serverMuted</span><span class="sxs-lookup"><span data-stu-id="a5a9f-122">serverMuted</span></span> | <span data-ttu-id="a5a9f-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5a9f-123">Boolean</span></span> | <span data-ttu-id="a5a9f-124">Se a mídia está sem som pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="a5a9f-124">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="a5a9f-125">sourceId</span><span class="sxs-lookup"><span data-stu-id="a5a9f-125">sourceId</span></span>    | <span data-ttu-id="a5a9f-126">String</span><span class="sxs-lookup"><span data-stu-id="a5a9f-126">String</span></span>  | <span data-ttu-id="a5a9f-127">A ID de origem.</span><span class="sxs-lookup"><span data-stu-id="a5a9f-127">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="a5a9f-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5a9f-128">JSON representation</span></span>

<span data-ttu-id="a5a9f-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5a9f-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="a5a9f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5a9f-130">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
