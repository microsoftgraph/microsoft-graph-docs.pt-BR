---
title: tipo de recurso mediaConfig
description: Uma classe base abstrata que contém a configuração de mídia usada para se conectar a uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0f47ac0986107af16640208d64190da6138805d5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866711"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="c8edd-103">tipo de recurso mediaConfig</span><span class="sxs-lookup"><span data-stu-id="c8edd-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8edd-104">Uma classe base abstrata que contém a configuração de mídia usada para se conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="c8edd-104">An abstract base class that contains the media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="c8edd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8edd-105">Properties</span></span>

| <span data-ttu-id="c8edd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8edd-106">Property</span></span>       | <span data-ttu-id="c8edd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8edd-107">Type</span></span>    | <span data-ttu-id="c8edd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8edd-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c8edd-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="c8edd-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="c8edd-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="c8edd-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="c8edd-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8edd-111">JSON representation</span></span>

<span data-ttu-id="c8edd-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8edd-112">The following is a JSON representation of the resource.</span></span>

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
