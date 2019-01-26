---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
ms.openlocfilehash: 6ec80f5505cb3dd742a2690ebb3cd5374635770d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572735"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="029c0-103">Tipo de recurso attendeeBase</span><span class="sxs-lookup"><span data-stu-id="029c0-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="029c0-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="029c0-104">The type of attendee.</span></span>

<span data-ttu-id="029c0-105">Derivado do [destinatário](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="029c0-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="029c0-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="029c0-106">JSON representation</span></span>

<span data-ttu-id="029c0-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="029c0-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
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
## <a name="properties"></a><span data-ttu-id="029c0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="029c0-108">Properties</span></span>
| <span data-ttu-id="029c0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="029c0-109">Property</span></span>     | <span data-ttu-id="029c0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="029c0-110">Type</span></span>   |<span data-ttu-id="029c0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="029c0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="029c0-112">type</span><span class="sxs-lookup"><span data-stu-id="029c0-112">type</span></span>|<span data-ttu-id="029c0-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="029c0-113">attendeeType</span></span>| <span data-ttu-id="029c0-114">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="029c0-114">The type of attendee.</span></span> <span data-ttu-id="029c0-115">Os valores possíveis são: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="029c0-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="029c0-116">Se o nome do participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera atualmente a pessoa é do `Required` tipo.</span><span class="sxs-lookup"><span data-stu-id="029c0-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="029c0-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="029c0-117">emailAddress</span></span>|[<span data-ttu-id="029c0-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="029c0-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="029c0-119">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="029c0-119">Includes the name and SMTP address of the attendee.</span></span>|

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
