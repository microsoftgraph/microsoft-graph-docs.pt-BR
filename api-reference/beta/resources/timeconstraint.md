---
title: Tipo de recurso timeConstraint
description: Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.
localization_priority: Normal
ms.openlocfilehash: 45469211aa4925834fd9d20da6a9905ac87d221e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577232"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="4335e-103">Tipo de recurso timeConstraint</span><span class="sxs-lookup"><span data-stu-id="4335e-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4335e-104">Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.</span><span class="sxs-lookup"><span data-stu-id="4335e-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4335e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4335e-105">JSON representation</span></span>

<span data-ttu-id="4335e-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4335e-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="4335e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4335e-107">Properties</span></span>
| <span data-ttu-id="4335e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4335e-108">Property</span></span>     | <span data-ttu-id="4335e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4335e-109">Type</span></span>   |<span data-ttu-id="4335e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4335e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4335e-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="4335e-111">activityDomain</span></span>|<span data-ttu-id="4335e-112">String</span><span class="sxs-lookup"><span data-stu-id="4335e-112">String</span></span>|<span data-ttu-id="4335e-p101">A natureza da atividade, opcional. Os valores possíveis são: `work`, `personal`, `unrestricted` ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4335e-p101">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="4335e-115">intervalos de tempo</span><span class="sxs-lookup"><span data-stu-id="4335e-115">timeslots</span></span>|<span data-ttu-id="4335e-116">Coleção [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="4335e-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="4335e-117">Uma matriz de períodos de tempo.</span><span class="sxs-lookup"><span data-stu-id="4335e-117">An array of time periods.</span></span>|

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
