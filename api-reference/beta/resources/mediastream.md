---
title: tipo de recurso de mediaStream
description: O tipo de mediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 7e56448c2c6d284e7a5904f1b0af414166782907
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889611"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="b2a58-103">tipo de recurso de mediaStream</span><span class="sxs-lookup"><span data-stu-id="b2a58-103">mediaStream resource type</span></span>

> <span data-ttu-id="b2a58-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b2a58-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2a58-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b2a58-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2a58-106">O tipo de mediaStream.</span><span class="sxs-lookup"><span data-stu-id="b2a58-106">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="b2a58-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2a58-107">Properties</span></span>

| <span data-ttu-id="b2a58-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2a58-108">Property</span></span>    | <span data-ttu-id="b2a58-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2a58-109">Type</span></span>    | <span data-ttu-id="b2a58-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2a58-110">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="b2a58-111">direção</span><span class="sxs-lookup"><span data-stu-id="b2a58-111">direction</span></span>   | <span data-ttu-id="b2a58-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2a58-112">String</span></span>  | <span data-ttu-id="b2a58-113">A direção.</span><span class="sxs-lookup"><span data-stu-id="b2a58-113">The direction.</span></span> <span data-ttu-id="b2a58-114">Os valores possíveis são `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span><span class="sxs-lookup"><span data-stu-id="b2a58-114">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="b2a58-115">rótulo</span><span class="sxs-lookup"><span data-stu-id="b2a58-115">label</span></span>       | <span data-ttu-id="b2a58-116">String</span><span class="sxs-lookup"><span data-stu-id="b2a58-116">String</span></span>  | <span data-ttu-id="b2a58-117">O rótulo de fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="b2a58-117">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="b2a58-118">mediaType</span><span class="sxs-lookup"><span data-stu-id="b2a58-118">mediaType</span></span>   | <span data-ttu-id="b2a58-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2a58-119">String</span></span>  | <span data-ttu-id="b2a58-120">O tipo de mídia.</span><span class="sxs-lookup"><span data-stu-id="b2a58-120">The media type.</span></span> <span data-ttu-id="b2a58-121">Os valores possíveis são `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="b2a58-121">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="b2a58-122">serverMuted</span><span class="sxs-lookup"><span data-stu-id="b2a58-122">serverMuted</span></span> | <span data-ttu-id="b2a58-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2a58-123">Boolean</span></span> | <span data-ttu-id="b2a58-124">Se a mídia está sem som pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="b2a58-124">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="b2a58-125">sourceId</span><span class="sxs-lookup"><span data-stu-id="b2a58-125">sourceId</span></span>    | <span data-ttu-id="b2a58-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2a58-126">String</span></span>  | <span data-ttu-id="b2a58-127">A ID de origem.</span><span class="sxs-lookup"><span data-stu-id="b2a58-127">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="b2a58-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2a58-128">JSON representation</span></span>

<span data-ttu-id="b2a58-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2a58-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b2a58-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2a58-130">Example</span></span>

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
