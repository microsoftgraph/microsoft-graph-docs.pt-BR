---
title: tipo de recurso callMediaState
description: Representa o estado de mídia de uma chamada.
author: VinodRavichandran
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 29402e813f6816ebea02ad2bb86c403408c2ff81
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006744"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="a6ac9-103">tipo de recurso callMediaState</span><span class="sxs-lookup"><span data-stu-id="a6ac9-103">callMediaState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6ac9-104">Representa o estado de mídia de uma [chamada](call.md).</span><span class="sxs-lookup"><span data-stu-id="a6ac9-104">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a6ac9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6ac9-105">Properties</span></span>

| <span data-ttu-id="a6ac9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6ac9-106">Property</span></span>            | <span data-ttu-id="a6ac9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6ac9-107">Type</span></span>    | <span data-ttu-id="a6ac9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6ac9-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="a6ac9-109">audio</span><span class="sxs-lookup"><span data-stu-id="a6ac9-109">audio</span></span>           | <span data-ttu-id="a6ac9-110">String</span><span class="sxs-lookup"><span data-stu-id="a6ac9-110">String</span></span>  | <span data-ttu-id="a6ac9-111">O estado da mídia de áudio.</span><span class="sxs-lookup"><span data-stu-id="a6ac9-111">The audio media state.</span></span> <span data-ttu-id="a6ac9-112">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="a6ac9-112">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6ac9-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6ac9-113">JSON representation</span></span>

<span data-ttu-id="a6ac9-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6ac9-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callMediaState"
}-->
```json
{
  "audio": "active | inactive",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callMediaState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
