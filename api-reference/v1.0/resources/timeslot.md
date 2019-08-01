---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5dbde12e63a5e48863f1353f4d4d22df5ba41091
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033590"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="9c64f-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="9c64f-103">timeSlot resource type</span></span>

<span data-ttu-id="9c64f-104">Representa um intervalo de tempo para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="9c64f-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c64f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c64f-105">JSON representation</span></span>

<span data-ttu-id="9c64f-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9c64f-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9c64f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c64f-107">Properties</span></span>
| <span data-ttu-id="9c64f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c64f-108">Property</span></span>     | <span data-ttu-id="9c64f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c64f-109">Type</span></span>   |<span data-ttu-id="9c64f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c64f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c64f-111">end</span><span class="sxs-lookup"><span data-stu-id="9c64f-111">end</span></span>|[<span data-ttu-id="9c64f-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9c64f-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9c64f-113">A data, a hora e o fuso horário em que um período começa.</span><span class="sxs-lookup"><span data-stu-id="9c64f-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="9c64f-114">iniciar</span><span class="sxs-lookup"><span data-stu-id="9c64f-114">start</span></span>|[<span data-ttu-id="9c64f-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9c64f-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9c64f-116">A data, a hora e o fuso horário que um período termina.</span><span class="sxs-lookup"><span data-stu-id="9c64f-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
