---
title: tipo de recurso callMediaState
description: Representa o estado de mídia de uma chamada.
author: VinodRavichandran
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 01e2e8017d89ddf96997d1d5bef729f9e9dc439d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871002"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="6e693-103">tipo de recurso callMediaState</span><span class="sxs-lookup"><span data-stu-id="6e693-103">callMediaState resource type</span></span>


<span data-ttu-id="6e693-104">Representa o estado de mídia de uma [chamada](call.md).</span><span class="sxs-lookup"><span data-stu-id="6e693-104">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6e693-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e693-105">Properties</span></span>

| <span data-ttu-id="6e693-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e693-106">Property</span></span>            | <span data-ttu-id="6e693-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e693-107">Type</span></span>    | <span data-ttu-id="6e693-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e693-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="6e693-109">audio</span><span class="sxs-lookup"><span data-stu-id="6e693-109">audio</span></span>           | <span data-ttu-id="6e693-110">String</span><span class="sxs-lookup"><span data-stu-id="6e693-110">String</span></span>  | <span data-ttu-id="6e693-111">O estado da mídia de áudio.</span><span class="sxs-lookup"><span data-stu-id="6e693-111">The audio media state.</span></span> <span data-ttu-id="6e693-112">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="6e693-112">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6e693-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e693-113">JSON representation</span></span>

<span data-ttu-id="6e693-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e693-114">The following is a JSON representation of the resource.</span></span>

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
