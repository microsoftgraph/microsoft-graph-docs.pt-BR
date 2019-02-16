---
title: tipo de recurso attendeeAvailabilityDataModel
description: O tipo e a disponibilidade dos participantes.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6d7436a640b4aaba0a9b71ef62ee91b3fe0d7cee
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057328"
---
# <a name="attendeeavailabilitydatamodel-resource-type"></a><span data-ttu-id="f4009-103">tipo de recurso attendeeAvailabilityDataModel</span><span class="sxs-lookup"><span data-stu-id="f4009-103">attendeeAvailabilityDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4009-104">Representa uma pessoa ou recurso e sua disponibilidade para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="f4009-104">Represents a person or resource and their availability for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4009-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4009-105">JSON representation</span></span>

<span data-ttu-id="f4009-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f4009-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeDataModel"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="f4009-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4009-107">Properties</span></span>
| <span data-ttu-id="f4009-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4009-108">Property</span></span>     | <span data-ttu-id="f4009-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4009-109">Type</span></span>   |<span data-ttu-id="f4009-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4009-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4009-111">attendee</span><span class="sxs-lookup"><span data-stu-id="f4009-111">attendee</span></span>|[<span data-ttu-id="f4009-112">attendeeDataModel</span><span class="sxs-lookup"><span data-stu-id="f4009-112">attendeeDataModel</span></span>](attendeedatamodel.md)|<span data-ttu-id="f4009-113">Representa uma pessoa ou um participante de recurso e se o participante é obrigatório ou opcional para a reunião.</span><span class="sxs-lookup"><span data-stu-id="f4009-113">Represents a person or resource attendee and whether the attendee is required or optional for the meeting.</span></span>|
|<span data-ttu-id="f4009-114">availability</span><span class="sxs-lookup"><span data-stu-id="f4009-114">availability</span></span>|<span data-ttu-id="f4009-115">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="f4009-115">availabilityStatus</span></span>| <span data-ttu-id="f4009-116">O status de disponibilidade do participante.</span><span class="sxs-lookup"><span data-stu-id="f4009-116">The availability status of the attendee.</span></span> <span data-ttu-id="f4009-117">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f4009-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailabilityDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailabilitydatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->