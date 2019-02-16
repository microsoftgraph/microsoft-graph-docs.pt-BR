---
title: tipo de recurso attendeeDataModel
description: O tipo de participante.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e8659b88cae8b9d2a94177593da40b61363fa23b
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057333"
---
# <a name="attendeedatamodel-resource-type"></a><span data-ttu-id="46ea0-103">tipo de recurso attendeeDataModel</span><span class="sxs-lookup"><span data-stu-id="46ea0-103">attendeeDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46ea0-104">Representa uma pessoa ou um recurso que está sendo incluído em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="46ea0-104">Represents a person or resource who is being included in a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="46ea0-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46ea0-105">JSON representation</span></span>

<span data-ttu-id="46ea0-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="46ea0-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "type"
  ],
  "@odata.type": "microsoft.graph.attendeeDataModel"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="46ea0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46ea0-107">Properties</span></span>
| <span data-ttu-id="46ea0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46ea0-108">Property</span></span>     | <span data-ttu-id="46ea0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="46ea0-109">Type</span></span>   |<span data-ttu-id="46ea0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="46ea0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46ea0-111">type</span><span class="sxs-lookup"><span data-stu-id="46ea0-111">type</span></span>|<span data-ttu-id="46ea0-112">articipantetype</span><span class="sxs-lookup"><span data-stu-id="46ea0-112">attendeeType</span></span>| <span data-ttu-id="46ea0-113">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="46ea0-113">The type of attendee.</span></span> <span data-ttu-id="46ea0-114">Os valores possíveis são: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="46ea0-114">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="46ea0-115">No momento, se o participante for uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considerará que a `required` pessoa é do tipo.</span><span class="sxs-lookup"><span data-stu-id="46ea0-115">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `required` type.</span></span>|
|<span data-ttu-id="46ea0-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="46ea0-116">emailAddress</span></span>|[<span data-ttu-id="46ea0-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="46ea0-117">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="46ea0-118">Inclui o nome e endereço SMTP do participante.</span><span class="sxs-lookup"><span data-stu-id="46ea0-118">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeedatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->