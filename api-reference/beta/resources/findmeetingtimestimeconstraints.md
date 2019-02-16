---
title: tipo de recurso findMeetingTimesTimeConstraints
description: Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e5790faf49fea03040dca05d457fededf5fdd683
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057332"
---
# <a name="findmeetingtimestimeconstraints-resource-type"></a><span data-ttu-id="b270e-103">tipo de recurso findMeetingTimesTimeConstraints</span><span class="sxs-lookup"><span data-stu-id="b270e-103">findMeetingTimesTimeConstraints resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b270e-104">Restringe as sugestões de horário de reunião para a natureza da atividade e determinados intervalos de tempo. |</span><span class="sxs-lookup"><span data-stu-id="b270e-104">Restricts meeting time suggestions to the nature of activity and certain ranges of time.|</span></span>

## <a name="json-representation"></a><span data-ttu-id="b270e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b270e-105">JSON representation</span></span>

<span data-ttu-id="b270e-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b270e-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.findMeetingTimesTimeConstraints"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="b270e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b270e-107">Properties</span></span>
| <span data-ttu-id="b270e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b270e-108">Property</span></span>     | <span data-ttu-id="b270e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b270e-109">Type</span></span>   |<span data-ttu-id="b270e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b270e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b270e-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="b270e-111">activityDomain</span></span>|<span data-ttu-id="b270e-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="b270e-112">activityDomain</span></span>|<span data-ttu-id="b270e-p101">A natureza da atividade, opcional. Os valores possíveis são: `work`, `personal`, `unrestricted` ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b270e-p101">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="b270e-115">intervalos de tempo</span><span class="sxs-lookup"><span data-stu-id="b270e-115">timeslots</span></span>|<span data-ttu-id="b270e-116">coleção [searchWindowTimeSlot](searchwindowtimeslot.md)</span><span class="sxs-lookup"><span data-stu-id="b270e-116">[searchWindowTimeSlot](searchwindowtimeslot.md) collection</span></span>|<span data-ttu-id="b270e-117">Uma matriz de intervalos de tempo para procurar possíveis tempos de reunião.</span><span class="sxs-lookup"><span data-stu-id="b270e-117">An array of time ranges to look into for possible meeting times.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "findMeetingTimesTimeConstraints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/findmeetingtimestimeconstraints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->