---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
ms.openlocfilehash: 9a2469447bbf0fbb059b41f9bf2b546c341f9190
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517761"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="49c91-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="49c91-103">timeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49c91-104">Um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="49c91-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="49c91-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49c91-105">JSON representation</span></span>

<span data-ttu-id="49c91-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="49c91-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="49c91-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49c91-107">Properties</span></span>
| <span data-ttu-id="49c91-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49c91-108">Property</span></span>     | <span data-ttu-id="49c91-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="49c91-109">Type</span></span>   |<span data-ttu-id="49c91-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="49c91-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49c91-111">end</span><span class="sxs-lookup"><span data-stu-id="49c91-111">end</span></span>|[<span data-ttu-id="49c91-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="49c91-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="49c91-113">A hora em que um período inicia.</span><span class="sxs-lookup"><span data-stu-id="49c91-113">The time a period begins.</span></span>|
|<span data-ttu-id="49c91-114">iniciar</span><span class="sxs-lookup"><span data-stu-id="49c91-114">start</span></span>|[<span data-ttu-id="49c91-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="49c91-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="49c91-116">A hora em que um período termina.</span><span class="sxs-lookup"><span data-stu-id="49c91-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeslot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
