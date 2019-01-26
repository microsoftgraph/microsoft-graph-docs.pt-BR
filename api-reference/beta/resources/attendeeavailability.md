---
title: Tipo de recurso attendeeAvailability
description: O tipo e a disponibilidade dos participantes.
localization_priority: Normal
ms.openlocfilehash: 37b344f110557d6e04129a2b93592009635bddcf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576280"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="66f31-103">Tipo de recurso attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="66f31-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66f31-104">O tipo e a disponibilidade dos participantes.</span><span class="sxs-lookup"><span data-stu-id="66f31-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66f31-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66f31-105">JSON representation</span></span>

<span data-ttu-id="66f31-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="66f31-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="66f31-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66f31-107">Properties</span></span>
| <span data-ttu-id="66f31-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66f31-108">Property</span></span>     | <span data-ttu-id="66f31-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="66f31-109">Type</span></span>   |<span data-ttu-id="66f31-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="66f31-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66f31-111">attendee</span><span class="sxs-lookup"><span data-stu-id="66f31-111">attendee</span></span>|[<span data-ttu-id="66f31-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="66f31-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="66f31-113">O tipo de participante, ou seja, se é um recurso ou uma pessoa e, no caso de uma pessoa, se é obrigatório ou opcional.</span><span class="sxs-lookup"><span data-stu-id="66f31-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="66f31-114">availability</span><span class="sxs-lookup"><span data-stu-id="66f31-114">availability</span></span>|<span data-ttu-id="66f31-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="66f31-115">freeBusyStatus</span></span>| <span data-ttu-id="66f31-116">O status de disponibilidade do participante.</span><span class="sxs-lookup"><span data-stu-id="66f31-116">The availability status of the attendee.</span></span> <span data-ttu-id="66f31-117">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="66f31-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

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
