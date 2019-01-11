---
title: Tipo de recurso attendeeAvailability
description: O tipo e a disponibilidade dos participantes.
localization_priority: Normal
ms.openlocfilehash: a6dee994fc5eb3786fc1a432adcb9333bdb56ec8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834745"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="7abee-103">Tipo de recurso attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="7abee-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="7abee-104">O tipo e a disponibilidade dos participantes.</span><span class="sxs-lookup"><span data-stu-id="7abee-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7abee-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7abee-105">JSON representation</span></span>

<span data-ttu-id="7abee-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7abee-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="7abee-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7abee-107">Properties</span></span>
| <span data-ttu-id="7abee-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7abee-108">Property</span></span>     | <span data-ttu-id="7abee-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7abee-109">Type</span></span>   |<span data-ttu-id="7abee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7abee-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7abee-111">attendee</span><span class="sxs-lookup"><span data-stu-id="7abee-111">attendee</span></span>|[<span data-ttu-id="7abee-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="7abee-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="7abee-113">O tipo de participante, ou seja, se é um recurso ou uma pessoa e, no caso de uma pessoa, se é obrigatório ou opcional.</span><span class="sxs-lookup"><span data-stu-id="7abee-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="7abee-114">availability</span><span class="sxs-lookup"><span data-stu-id="7abee-114">availability</span></span>|<span data-ttu-id="7abee-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="7abee-115">freeBusyStatus</span></span>| <span data-ttu-id="7abee-116">O status de disponibilidade do participante.</span><span class="sxs-lookup"><span data-stu-id="7abee-116">The availability status of the attendee.</span></span> <span data-ttu-id="7abee-117">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7abee-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
