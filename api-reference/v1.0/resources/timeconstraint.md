---
title: Tipo de recurso timeConstraint
description: Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.
ms.openlocfilehash: 82ab18eb09201236f3227c7dd0660519092a3133
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004165"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="7f16d-103">Tipo de recurso timeConstraint</span><span class="sxs-lookup"><span data-stu-id="7f16d-103">timeConstraint resource type</span></span>

<span data-ttu-id="7f16d-104">Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.</span><span class="sxs-lookup"><span data-stu-id="7f16d-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f16d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f16d-105">JSON representation</span></span>

<span data-ttu-id="7f16d-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7f16d-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="7f16d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f16d-107">Properties</span></span>
| <span data-ttu-id="7f16d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f16d-108">Property</span></span>     | <span data-ttu-id="7f16d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f16d-109">Type</span></span>   |<span data-ttu-id="7f16d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f16d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f16d-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="7f16d-111">activityDomain</span></span>|<span data-ttu-id="7f16d-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="7f16d-112">activityDomain</span></span>|<span data-ttu-id="7f16d-113">A natureza da atividade, opcional.</span><span class="sxs-lookup"><span data-stu-id="7f16d-113">The nature of the activity, optional.</span></span> <span data-ttu-id="7f16d-114">Os valores possíveis são: `work`, `personal`, `unrestricted`, ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7f16d-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="7f16d-115">intervalos de tempo</span><span class="sxs-lookup"><span data-stu-id="7f16d-115">timeslots</span></span>|<span data-ttu-id="7f16d-116">Coleção [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="7f16d-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="7f16d-117">Uma matriz de períodos de tempo.</span><span class="sxs-lookup"><span data-stu-id="7f16d-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
