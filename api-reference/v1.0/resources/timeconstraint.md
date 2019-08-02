---
title: Tipo de recurso timeConstraint
description: Restringe as sugestões de horário de reunião a determinadas horas e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo abertos.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7da2a3a2c712cdbe1fc3fb961781e35099a565d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033611"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="493ec-103">Tipo de recurso timeConstraint</span><span class="sxs-lookup"><span data-stu-id="493ec-103">timeConstraint resource type</span></span>

<span data-ttu-id="493ec-104">Restringe as sugestões de horário de reunião a determinadas horas e dias da semana de acordo com a natureza especificada da atividade e os intervalos de tempo abertos.</span><span class="sxs-lookup"><span data-stu-id="493ec-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="493ec-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="493ec-105">JSON representation</span></span>

<span data-ttu-id="493ec-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="493ec-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="493ec-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="493ec-107">Properties</span></span>
| <span data-ttu-id="493ec-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="493ec-108">Property</span></span>     | <span data-ttu-id="493ec-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="493ec-109">Type</span></span>   |<span data-ttu-id="493ec-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="493ec-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="493ec-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="493ec-111">activityDomain</span></span>|<span data-ttu-id="493ec-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="493ec-112">activityDomain</span></span>|<span data-ttu-id="493ec-113">A natureza da atividade, opcional.</span><span class="sxs-lookup"><span data-stu-id="493ec-113">The nature of the activity, optional.</span></span> <span data-ttu-id="493ec-114">Os valores possíveis são: `work`, `personal`, `unrestricted`, ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="493ec-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="493ec-115">intervalos de tempo</span><span class="sxs-lookup"><span data-stu-id="493ec-115">timeslots</span></span>|<span data-ttu-id="493ec-116">Coleção [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="493ec-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="493ec-117">Uma matriz de períodos de tempo.</span><span class="sxs-lookup"><span data-stu-id="493ec-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
