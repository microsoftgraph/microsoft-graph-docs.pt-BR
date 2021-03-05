---
title: Tipo de recurso timeConstraint
description: Restringe sugestões de hora de reunião a determinados horários e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo de abertura.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d79fc1630522c30abea6ac5ec6f51d0f5a15e437
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472101"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="2256c-103">Tipo de recurso timeConstraint</span><span class="sxs-lookup"><span data-stu-id="2256c-103">timeConstraint resource type</span></span>

<span data-ttu-id="2256c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2256c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2256c-105">Restringe sugestões de hora de reunião a determinados horários e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo de abertura.</span><span class="sxs-lookup"><span data-stu-id="2256c-105">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2256c-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2256c-106">JSON representation</span></span>
<span data-ttu-id="2256c-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2256c-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="2256c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2256c-108">Properties</span></span>
| <span data-ttu-id="2256c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2256c-109">Property</span></span>     | <span data-ttu-id="2256c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2256c-110">Type</span></span>   |<span data-ttu-id="2256c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2256c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2256c-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="2256c-112">activityDomain</span></span>|<span data-ttu-id="2256c-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="2256c-113">activityDomain</span></span>|<span data-ttu-id="2256c-114">A natureza da atividade, opcional.</span><span class="sxs-lookup"><span data-stu-id="2256c-114">The nature of the activity, optional.</span></span> <span data-ttu-id="2256c-115">Os valores possíveis são: `work` `personal` , , ou `unrestricted` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="2256c-115">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="2256c-116">intervalos de tempo</span><span class="sxs-lookup"><span data-stu-id="2256c-116">timeslots</span></span>|<span data-ttu-id="2256c-117">Coleção [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="2256c-117">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="2256c-118">Uma matriz de períodos de tempo.</span><span class="sxs-lookup"><span data-stu-id="2256c-118">An array of time periods.</span></span>|

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


