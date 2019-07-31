---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8843b8418bff068564e5716d715a9ad11579f01b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007533"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="de095-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="de095-103">timeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de095-104">Representa um intervalo de tempo para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="de095-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="de095-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de095-105">JSON representation</span></span>

<span data-ttu-id="de095-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="de095-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="de095-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de095-107">Properties</span></span>
| <span data-ttu-id="de095-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de095-108">Property</span></span>     | <span data-ttu-id="de095-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="de095-109">Type</span></span>   |<span data-ttu-id="de095-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="de095-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de095-111">end</span><span class="sxs-lookup"><span data-stu-id="de095-111">end</span></span>|[<span data-ttu-id="de095-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="de095-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="de095-113">A data, a hora e o fuso horário em que um período começa.</span><span class="sxs-lookup"><span data-stu-id="de095-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="de095-114">iniciar</span><span class="sxs-lookup"><span data-stu-id="de095-114">start</span></span>|[<span data-ttu-id="de095-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="de095-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="de095-116">A data, a hora e o fuso horário que um período termina.</span><span class="sxs-lookup"><span data-stu-id="de095-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
