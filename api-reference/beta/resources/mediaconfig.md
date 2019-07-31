---
title: tipo de recurso mediaConfig
description: A configuração de mídia usada para se conectar a uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4d00470d517c4d701a028a1911efe02a6f441639
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009773"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="a3a19-103">tipo de recurso mediaConfig</span><span class="sxs-lookup"><span data-stu-id="a3a19-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3a19-104">A configuração de mídia usada para se conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="a3a19-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="a3a19-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3a19-105">Properties</span></span>

| <span data-ttu-id="a3a19-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3a19-106">Property</span></span>       | <span data-ttu-id="a3a19-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3a19-107">Type</span></span>    | <span data-ttu-id="a3a19-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3a19-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3a19-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="a3a19-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="a3a19-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="a3a19-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="a3a19-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3a19-111">JSON representation</span></span>

<span data-ttu-id="a3a19-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3a19-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
   ],
  "abstract": true,
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
