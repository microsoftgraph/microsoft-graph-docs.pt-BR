---
title: Tipo de recurso timeConstraint
description: Restringe as sugestões de horário de reunião a determinadas horas e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo abertos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 680ada778ea64f982e9ed5fac11c935a6cce55d5
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2019
ms.locfileid: "30937760"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="3e796-103">Tipo de recurso timeConstraint</span><span class="sxs-lookup"><span data-stu-id="3e796-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e796-104">Restringe as sugestões de horário de reunião a determinadas horas e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo abertos.</span><span class="sxs-lookup"><span data-stu-id="3e796-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3e796-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e796-105">JSON representation</span></span>
<span data-ttu-id="3e796-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3e796-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="3e796-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e796-107">Properties</span></span>
| <span data-ttu-id="3e796-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e796-108">Property</span></span>     | <span data-ttu-id="3e796-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e796-109">Type</span></span>   |<span data-ttu-id="3e796-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e796-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e796-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="3e796-111">activityDomain</span></span>|<span data-ttu-id="3e796-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="3e796-112">activityDomain</span></span>|<span data-ttu-id="3e796-113">A natureza da atividade, opcional.</span><span class="sxs-lookup"><span data-stu-id="3e796-113">The nature of the activity, optional.</span></span> <span data-ttu-id="3e796-114">Os valores possíveis são `work`: `personal`, `unrestricted`,, `unknown`ou.</span><span class="sxs-lookup"><span data-stu-id="3e796-114">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="3e796-115">intervalos de tempo</span><span class="sxs-lookup"><span data-stu-id="3e796-115">timeslots</span></span>|<span data-ttu-id="3e796-116">Coleção [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="3e796-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="3e796-117">Uma matriz de períodos de tempo.</span><span class="sxs-lookup"><span data-stu-id="3e796-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeconstraint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->