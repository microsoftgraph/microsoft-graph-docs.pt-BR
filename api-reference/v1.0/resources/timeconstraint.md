---
title: Tipo de recurso timeConstraint
description: Restringe as sugestões de horário de reunião a determinadas horas e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo abertos.
localization_priority: Normal
ms.openlocfilehash: b6e239abbd0d9f7b4f83df4a60625a2f88131476
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456948"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="bcddc-103">Tipo de recurso timeConstraint</span><span class="sxs-lookup"><span data-stu-id="bcddc-103">timeConstraint resource type</span></span>

<span data-ttu-id="bcddc-104">Restringe as sugestões de horário de reunião a determinadas horas e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo abertos.</span><span class="sxs-lookup"><span data-stu-id="bcddc-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bcddc-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bcddc-105">JSON representation</span></span>

<span data-ttu-id="bcddc-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bcddc-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="bcddc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bcddc-107">Properties</span></span>
| <span data-ttu-id="bcddc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcddc-108">Property</span></span>     | <span data-ttu-id="bcddc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcddc-109">Type</span></span>   |<span data-ttu-id="bcddc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcddc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcddc-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="bcddc-111">activityDomain</span></span>|<span data-ttu-id="bcddc-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="bcddc-112">activityDomain</span></span>|<span data-ttu-id="bcddc-113">A natureza da atividade, opcional.</span><span class="sxs-lookup"><span data-stu-id="bcddc-113">The nature of the activity, optional.</span></span> <span data-ttu-id="bcddc-114">Os valores possíveis são: `work`, `personal`, `unrestricted`, ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="bcddc-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="bcddc-115">intervalos de tempo</span><span class="sxs-lookup"><span data-stu-id="bcddc-115">timeslots</span></span>|<span data-ttu-id="bcddc-116">Coleção [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="bcddc-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="bcddc-117">Uma matriz de períodos de tempo.</span><span class="sxs-lookup"><span data-stu-id="bcddc-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
