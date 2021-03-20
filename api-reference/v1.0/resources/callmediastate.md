---
title: tipo de recurso callMediaState
description: Representa o estado de mídia de uma chamada.
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: f8797aadf7e35000d799c4c8b879ef2ed6da6409
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952533"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="4aa3a-103">tipo de recurso callMediaState</span><span class="sxs-lookup"><span data-stu-id="4aa3a-103">callMediaState resource type</span></span>

<span data-ttu-id="4aa3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4aa3a-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="4aa3a-105">Representa o estado de mídia de uma [chamada](call.md).</span><span class="sxs-lookup"><span data-stu-id="4aa3a-105">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4aa3a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4aa3a-106">Properties</span></span>

| <span data-ttu-id="4aa3a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4aa3a-107">Property</span></span>            | <span data-ttu-id="4aa3a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4aa3a-108">Type</span></span>    | <span data-ttu-id="4aa3a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4aa3a-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="4aa3a-110">audio</span><span class="sxs-lookup"><span data-stu-id="4aa3a-110">audio</span></span>           | <span data-ttu-id="4aa3a-111">mediaState</span><span class="sxs-lookup"><span data-stu-id="4aa3a-111">mediaState</span></span>  | <span data-ttu-id="4aa3a-112">O estado da mídia de áudio.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-112">The audio media state.</span></span> <span data-ttu-id="4aa3a-113">Os valores possíveis são: `active`, `inactive`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-113">Possible values are: `active`, `inactive`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4aa3a-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4aa3a-114">JSON representation</span></span>

<span data-ttu-id="4aa3a-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-115">The following is a JSON representation of the resource.</span></span>

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

