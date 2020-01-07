---
title: tipo de recurso timerange
description: Um recurso de intervalo de tempo com um horário de início e de término.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0e91f08e9f421a348f5ec7c2ebf5e2f23d4e9377
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952311"
---
# <a name="timerange-resource-type"></a><span data-ttu-id="452a4-103">tipo de recurso timerange</span><span class="sxs-lookup"><span data-stu-id="452a4-103">timeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="452a4-104">Um recurso de intervalo de tempo com um horário de início e de término.</span><span class="sxs-lookup"><span data-stu-id="452a4-104">A time range resource with a start and end time.</span></span>

## <a name="properties"></a><span data-ttu-id="452a4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="452a4-105">Properties</span></span>

| <span data-ttu-id="452a4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="452a4-106">Property</span></span>     | <span data-ttu-id="452a4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="452a4-107">Type</span></span>        | <span data-ttu-id="452a4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="452a4-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="452a4-109">endTime</span><span class="sxs-lookup"><span data-stu-id="452a4-109">endTime</span></span>|<span data-ttu-id="452a4-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="452a4-110">TimeOfDay</span></span>|<span data-ttu-id="452a4-111">Hora de término do intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="452a4-111">End time for the time range.</span></span>|
|<span data-ttu-id="452a4-112">startTime</span><span class="sxs-lookup"><span data-stu-id="452a4-112">startTime</span></span>|<span data-ttu-id="452a4-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="452a4-113">TimeOfDay</span></span>|<span data-ttu-id="452a4-114">Hora de início do intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="452a4-114">Start time for the time range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="452a4-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="452a4-115">JSON representation</span></span>

<span data-ttu-id="452a4-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="452a4-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeRange",
  "baseType": null
}-->

```json
{
  "endTime": "String (timestamp)",
  "startTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->