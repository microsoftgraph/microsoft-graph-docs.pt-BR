---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ee8746d1278f4c9422fa2803895a20c359d5f1e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555287"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="3d8ff-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="3d8ff-103">timeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d8ff-104">Representa um intervalo de tempo para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="3d8ff-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d8ff-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d8ff-105">JSON representation</span></span>

<span data-ttu-id="3d8ff-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3d8ff-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3d8ff-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d8ff-107">Properties</span></span>
| <span data-ttu-id="3d8ff-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d8ff-108">Property</span></span>     | <span data-ttu-id="3d8ff-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d8ff-109">Type</span></span>   |<span data-ttu-id="3d8ff-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d8ff-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d8ff-111">end</span><span class="sxs-lookup"><span data-stu-id="3d8ff-111">end</span></span>|[<span data-ttu-id="3d8ff-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3d8ff-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3d8ff-113">A data, a hora e o fuso horário em que um período começa.</span><span class="sxs-lookup"><span data-stu-id="3d8ff-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="3d8ff-114">iniciar</span><span class="sxs-lookup"><span data-stu-id="3d8ff-114">start</span></span>|[<span data-ttu-id="3d8ff-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3d8ff-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3d8ff-116">A data, a hora e o fuso horário que um período termina.</span><span class="sxs-lookup"><span data-stu-id="3d8ff-116">The date, time, and time zone that a period ends.</span></span>|

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
