---
title: Tipo de recurso timeConstraint
description: Restringe as sugestões de horário de reunião a determinadas horas e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo abertos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4215b4350236956bfcad3bdf6f787b7f6c77f5dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075515"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="f3d21-103">Tipo de recurso timeConstraint</span><span class="sxs-lookup"><span data-stu-id="f3d21-103">timeConstraint resource type</span></span>

<span data-ttu-id="f3d21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3d21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3d21-105">Restringe as sugestões de horário de reunião a determinadas horas e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo abertos.</span><span class="sxs-lookup"><span data-stu-id="f3d21-105">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f3d21-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3d21-106">JSON representation</span></span>
<span data-ttu-id="f3d21-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f3d21-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}
```

## <a name="properties"></a><span data-ttu-id="f3d21-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3d21-108">Properties</span></span>
| <span data-ttu-id="f3d21-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3d21-109">Property</span></span>     | <span data-ttu-id="f3d21-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3d21-110">Type</span></span>   |<span data-ttu-id="f3d21-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3d21-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3d21-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="f3d21-112">activityDomain</span></span>|<span data-ttu-id="f3d21-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="f3d21-113">activityDomain</span></span>|<span data-ttu-id="f3d21-114">A natureza da atividade, opcional.</span><span class="sxs-lookup"><span data-stu-id="f3d21-114">The nature of the activity, optional.</span></span> <span data-ttu-id="f3d21-115">Os valores possíveis são: `work` , `personal` , `unrestricted` , ou `unknown` .</span><span class="sxs-lookup"><span data-stu-id="f3d21-115">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="f3d21-116">intervalos de tempo</span><span class="sxs-lookup"><span data-stu-id="f3d21-116">timeslots</span></span>|<span data-ttu-id="f3d21-117">Coleção [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="f3d21-117">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="f3d21-118">Uma matriz de períodos de tempo.</span><span class="sxs-lookup"><span data-stu-id="f3d21-118">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


