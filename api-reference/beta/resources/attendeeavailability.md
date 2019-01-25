---
title: Tipo de recurso attendeeAvailability
description: O tipo e a disponibilidade dos participantes.
localization_priority: Normal
ms.openlocfilehash: f831a88a14fc6ec970332208389e15a5adc49377
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508934"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="e2d08-103">Tipo de recurso attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="e2d08-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2d08-104">O tipo e a disponibilidade dos participantes.</span><span class="sxs-lookup"><span data-stu-id="e2d08-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2d08-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2d08-105">JSON representation</span></span>

<span data-ttu-id="e2d08-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e2d08-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="e2d08-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2d08-107">Properties</span></span>
| <span data-ttu-id="e2d08-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2d08-108">Property</span></span>     | <span data-ttu-id="e2d08-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2d08-109">Type</span></span>   |<span data-ttu-id="e2d08-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2d08-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2d08-111">attendee</span><span class="sxs-lookup"><span data-stu-id="e2d08-111">attendee</span></span>|[<span data-ttu-id="e2d08-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="e2d08-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="e2d08-113">O tipo de participante, ou seja, se é um recurso ou uma pessoa e, no caso de uma pessoa, se é obrigatório ou opcional.</span><span class="sxs-lookup"><span data-stu-id="e2d08-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="e2d08-114">availability</span><span class="sxs-lookup"><span data-stu-id="e2d08-114">availability</span></span>|<span data-ttu-id="e2d08-115">String</span><span class="sxs-lookup"><span data-stu-id="e2d08-115">String</span></span>| <span data-ttu-id="e2d08-p101">O status de disponibilidade do participante. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e2d08-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
