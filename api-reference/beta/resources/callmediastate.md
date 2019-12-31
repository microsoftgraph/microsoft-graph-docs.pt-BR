---
title: tipo de recurso callMediaState
description: Representa o estado de mídia de uma chamada.
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 14342a6657392dcfd16d32d1b6ce8d5bbf46ddf7
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913321"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="adb75-103">tipo de recurso callMediaState</span><span class="sxs-lookup"><span data-stu-id="adb75-103">callMediaState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adb75-104">Representa o estado de mídia de uma [chamada](call.md).</span><span class="sxs-lookup"><span data-stu-id="adb75-104">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="adb75-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="adb75-105">Properties</span></span>

| <span data-ttu-id="adb75-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="adb75-106">Property</span></span>            | <span data-ttu-id="adb75-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="adb75-107">Type</span></span>    | <span data-ttu-id="adb75-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="adb75-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="adb75-109">audio</span><span class="sxs-lookup"><span data-stu-id="adb75-109">audio</span></span>           | <span data-ttu-id="adb75-110">String</span><span class="sxs-lookup"><span data-stu-id="adb75-110">String</span></span>  | <span data-ttu-id="adb75-111">O estado da mídia de áudio.</span><span class="sxs-lookup"><span data-stu-id="adb75-111">The audio media state.</span></span> <span data-ttu-id="adb75-112">Os valores possíveis são: `active` e `inactive`.</span><span class="sxs-lookup"><span data-stu-id="adb75-112">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="adb75-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="adb75-113">JSON representation</span></span>

<span data-ttu-id="adb75-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="adb75-114">The following is a JSON representation of the resource.</span></span>

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
