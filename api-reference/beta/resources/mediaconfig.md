---
title: tipo de recurso mediaConfig
description: Uma classe base abstrata que contém a configuração de mídia usada para se conectar a uma chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 61fe1dfcc4c2c9b686a61d22e55ddae3c80661be
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913300"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="7ec6d-103">tipo de recurso mediaConfig</span><span class="sxs-lookup"><span data-stu-id="7ec6d-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ec6d-104">Uma classe base abstrata que contém a configuração de mídia usada para se conectar a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="7ec6d-104">An abstract base class that contains the media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="7ec6d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ec6d-105">Properties</span></span>

| <span data-ttu-id="7ec6d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ec6d-106">Property</span></span>       | <span data-ttu-id="7ec6d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ec6d-107">Type</span></span>    | <span data-ttu-id="7ec6d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ec6d-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ec6d-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="7ec6d-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="7ec6d-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ec6d-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="7ec6d-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ec6d-111">JSON representation</span></span>

<span data-ttu-id="7ec6d-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ec6d-112">The following is a JSON representation of the resource.</span></span>

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
