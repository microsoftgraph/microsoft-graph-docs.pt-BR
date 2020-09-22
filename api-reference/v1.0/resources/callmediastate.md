---
title: tipo de recurso callMediaState
description: Representa o estado de mídia de uma chamada.
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 24dde1de6248413a7fe7753492b40995f994e66d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009370"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="8873c-103">tipo de recurso callMediaState</span><span class="sxs-lookup"><span data-stu-id="8873c-103">callMediaState resource type</span></span>

<span data-ttu-id="8873c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8873c-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="8873c-105">Representa o estado de mídia de uma [chamada](call.md).</span><span class="sxs-lookup"><span data-stu-id="8873c-105">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8873c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8873c-106">Properties</span></span>

| <span data-ttu-id="8873c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8873c-107">Property</span></span>            | <span data-ttu-id="8873c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8873c-108">Type</span></span>    | <span data-ttu-id="8873c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8873c-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="8873c-110">audio</span><span class="sxs-lookup"><span data-stu-id="8873c-110">audio</span></span>           | <span data-ttu-id="8873c-111">String</span><span class="sxs-lookup"><span data-stu-id="8873c-111">String</span></span>  | <span data-ttu-id="8873c-112">O estado da mídia de áudio.</span><span class="sxs-lookup"><span data-stu-id="8873c-112">The audio media state.</span></span> <span data-ttu-id="8873c-113">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="8873c-113">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8873c-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8873c-114">JSON representation</span></span>

<span data-ttu-id="8873c-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8873c-115">The following is a JSON representation of the resource.</span></span>

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

