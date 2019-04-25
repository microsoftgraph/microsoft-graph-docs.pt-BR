---
title: Tipo de recurso timeConstraint
description: Restringe as sugestões de horário de reunião a determinadas horas e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo abertos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 680ada778ea64f982e9ed5fac11c935a6cce55d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582850"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="02dbe-103">Tipo de recurso timeConstraint</span><span class="sxs-lookup"><span data-stu-id="02dbe-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02dbe-104">Restringe as sugestões de horário de reunião a determinadas horas e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo abertos.</span><span class="sxs-lookup"><span data-stu-id="02dbe-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="02dbe-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02dbe-105">JSON representation</span></span>
<span data-ttu-id="02dbe-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="02dbe-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="02dbe-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02dbe-107">Properties</span></span>
| <span data-ttu-id="02dbe-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02dbe-108">Property</span></span>     | <span data-ttu-id="02dbe-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="02dbe-109">Type</span></span>   |<span data-ttu-id="02dbe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="02dbe-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02dbe-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="02dbe-111">activityDomain</span></span>|<span data-ttu-id="02dbe-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="02dbe-112">activityDomain</span></span>|<span data-ttu-id="02dbe-113">A natureza da atividade, opcional.</span><span class="sxs-lookup"><span data-stu-id="02dbe-113">The nature of the activity, optional.</span></span> <span data-ttu-id="02dbe-114">Os valores possíveis são `work`: `personal`, `unrestricted`,, `unknown`ou.</span><span class="sxs-lookup"><span data-stu-id="02dbe-114">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="02dbe-115">intervalos de tempo</span><span class="sxs-lookup"><span data-stu-id="02dbe-115">timeslots</span></span>|<span data-ttu-id="02dbe-116">Coleção [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="02dbe-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="02dbe-117">Uma matriz de períodos de tempo.</span><span class="sxs-lookup"><span data-stu-id="02dbe-117">An array of time periods.</span></span>|

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