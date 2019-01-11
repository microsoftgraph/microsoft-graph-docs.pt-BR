---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
ms.openlocfilehash: e01b8d0f34a21eb18bc92e8bcc4e1b8365541d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860561"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="341c9-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="341c9-103">timeSlot resource type</span></span>

<span data-ttu-id="341c9-104">Um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="341c9-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="341c9-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="341c9-105">JSON representation</span></span>

<span data-ttu-id="341c9-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="341c9-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="341c9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="341c9-107">Properties</span></span>
| <span data-ttu-id="341c9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="341c9-108">Property</span></span>     | <span data-ttu-id="341c9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="341c9-109">Type</span></span>   |<span data-ttu-id="341c9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="341c9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="341c9-111">end</span><span class="sxs-lookup"><span data-stu-id="341c9-111">end</span></span>|[<span data-ttu-id="341c9-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="341c9-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="341c9-113">A hora em que um período inicia.</span><span class="sxs-lookup"><span data-stu-id="341c9-113">The time a period begins.</span></span>|
|<span data-ttu-id="341c9-114">iniciar</span><span class="sxs-lookup"><span data-stu-id="341c9-114">start</span></span>|[<span data-ttu-id="341c9-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="341c9-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="341c9-116">A hora em que um período termina.</span><span class="sxs-lookup"><span data-stu-id="341c9-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
