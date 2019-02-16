---
title: tipo de recurso searchWindowTimeSlot
description: Um período de tempo.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 393e6a87f35f4ea6da5e7c4a4ccf37f52d90a8de
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057330"
---
# <a name="searchwindowtimeslot-resource-type"></a><span data-ttu-id="0576b-103">tipo de recurso searchWindowTimeSlot</span><span class="sxs-lookup"><span data-stu-id="0576b-103">searchWindowTimeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0576b-104">Um período de tempo para pesquisar em.</span><span class="sxs-lookup"><span data-stu-id="0576b-104">A time period to search within.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0576b-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0576b-105">JSON representation</span></span>

<span data-ttu-id="0576b-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0576b-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchWindowTimeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="0576b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0576b-107">Properties</span></span>
| <span data-ttu-id="0576b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0576b-108">Property</span></span>     | <span data-ttu-id="0576b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0576b-109">Type</span></span>   |<span data-ttu-id="0576b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0576b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0576b-111">end</span><span class="sxs-lookup"><span data-stu-id="0576b-111">end</span></span>|[<span data-ttu-id="0576b-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0576b-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0576b-113">A data, a hora e o fuso horário em que um período começa.</span><span class="sxs-lookup"><span data-stu-id="0576b-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="0576b-114">iniciar</span><span class="sxs-lookup"><span data-stu-id="0576b-114">start</span></span>|[<span data-ttu-id="0576b-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0576b-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0576b-116">A data, a hora e o fuso horário que um período termina.</span><span class="sxs-lookup"><span data-stu-id="0576b-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "searchWindowTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/searchwindowtimeslot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->