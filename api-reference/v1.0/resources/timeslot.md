---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7b09ae7f1c60a8348e9f22b856c65f326432e408
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936238"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="9bf35-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="9bf35-103">timeSlot resource type</span></span>

<span data-ttu-id="9bf35-104">Representa um intervalo de tempo para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="9bf35-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bf35-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bf35-105">JSON representation</span></span>

<span data-ttu-id="9bf35-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9bf35-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9bf35-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bf35-107">Properties</span></span>
| <span data-ttu-id="9bf35-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bf35-108">Property</span></span>     | <span data-ttu-id="9bf35-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bf35-109">Type</span></span>   |<span data-ttu-id="9bf35-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bf35-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bf35-111">end</span><span class="sxs-lookup"><span data-stu-id="9bf35-111">end</span></span>|[<span data-ttu-id="9bf35-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9bf35-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9bf35-113">A data, a hora e o fuso horário em que um período começa.</span><span class="sxs-lookup"><span data-stu-id="9bf35-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="9bf35-114">iniciar</span><span class="sxs-lookup"><span data-stu-id="9bf35-114">start</span></span>|[<span data-ttu-id="9bf35-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9bf35-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9bf35-116">A data, a hora e o fuso horário que um período termina.</span><span class="sxs-lookup"><span data-stu-id="9bf35-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
