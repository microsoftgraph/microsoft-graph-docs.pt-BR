---
title: tipo de recurso mediaConfig
description: A configuração de mídia usada para se conectar a uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f42f83923922cdf868dfa39ea3618f7fed2a37c6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006673"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="6a205-103">tipo de recurso mediaConfig</span><span class="sxs-lookup"><span data-stu-id="6a205-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a205-104">A configuração de mídia usada para se conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="6a205-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="6a205-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a205-105">Properties</span></span>

| <span data-ttu-id="6a205-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a205-106">Property</span></span>       | <span data-ttu-id="6a205-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a205-107">Type</span></span>    | <span data-ttu-id="6a205-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a205-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6a205-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="6a205-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="6a205-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a205-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="6a205-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a205-111">JSON representation</span></span>

<span data-ttu-id="6a205-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a205-112">The following is a JSON representation of the resource.</span></span>

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
