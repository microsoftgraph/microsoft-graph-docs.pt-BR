---
title: tipo de recurso timerange
description: Um recurso de intervalo de tempo com um horário de início e de término.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e9edfd06ecd65d7e08d6701d1fc885dce9067689
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519705"
---
# <a name="timerange-resource-type"></a><span data-ttu-id="cf5db-103">tipo de recurso timerange</span><span class="sxs-lookup"><span data-stu-id="cf5db-103">timeRange resource type</span></span>

<span data-ttu-id="cf5db-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cf5db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf5db-105">Um recurso de intervalo de tempo com um horário de início e de término.</span><span class="sxs-lookup"><span data-stu-id="cf5db-105">A time range resource with a start and end time.</span></span>

## <a name="properties"></a><span data-ttu-id="cf5db-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf5db-106">Properties</span></span>

| <span data-ttu-id="cf5db-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf5db-107">Property</span></span>     | <span data-ttu-id="cf5db-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf5db-108">Type</span></span>        | <span data-ttu-id="cf5db-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf5db-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf5db-110">endTime</span><span class="sxs-lookup"><span data-stu-id="cf5db-110">endTime</span></span>|<span data-ttu-id="cf5db-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cf5db-111">TimeOfDay</span></span>|<span data-ttu-id="cf5db-112">Hora de término do intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="cf5db-112">End time for the time range.</span></span>|
|<span data-ttu-id="cf5db-113">startTime</span><span class="sxs-lookup"><span data-stu-id="cf5db-113">startTime</span></span>|<span data-ttu-id="cf5db-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cf5db-114">TimeOfDay</span></span>|<span data-ttu-id="cf5db-115">Hora de início do intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="cf5db-115">Start time for the time range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf5db-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf5db-116">JSON representation</span></span>

<span data-ttu-id="cf5db-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf5db-117">The following is a JSON representation of the resource.</span></span>

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