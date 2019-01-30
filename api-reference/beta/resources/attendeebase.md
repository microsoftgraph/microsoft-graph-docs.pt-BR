---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
ms.openlocfilehash: bce1550c107f2114d02744091b5863360ab0bcea
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643437"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="3729c-103">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="3729c-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3729c-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="3729c-104">The type of attendee.</span></span>

<span data-ttu-id="3729c-105">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="3729c-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3729c-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3729c-106">JSON representation</span></span>

<span data-ttu-id="3729c-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3729c-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="3729c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3729c-108">Properties</span></span>
| <span data-ttu-id="3729c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3729c-109">Property</span></span>     | <span data-ttu-id="3729c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3729c-110">Type</span></span>   |<span data-ttu-id="3729c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3729c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3729c-112">type</span><span class="sxs-lookup"><span data-stu-id="3729c-112">type</span></span>|<span data-ttu-id="3729c-113">String</span><span class="sxs-lookup"><span data-stu-id="3729c-113">String</span></span>| <span data-ttu-id="3729c-p101">O tipo de participante. Os valores possíveis são: `required`, `optional`, `resource`. Atualmente, se o participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.</span><span class="sxs-lookup"><span data-stu-id="3729c-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="3729c-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3729c-117">emailAddress</span></span>|[<span data-ttu-id="3729c-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3729c-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="3729c-119">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="3729c-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeebase.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
