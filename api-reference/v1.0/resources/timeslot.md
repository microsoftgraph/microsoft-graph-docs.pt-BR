---
title: Tipo de recurso timeSlot
description: Um período de tempo.
ms.openlocfilehash: 43ce20e006f2a6946877a4ffd2bf730d45d6d1c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005444"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="bbe6e-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="bbe6e-103">timeSlot resource type</span></span>

<span data-ttu-id="bbe6e-104">Um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="bbe6e-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbe6e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbe6e-105">JSON representation</span></span>

<span data-ttu-id="bbe6e-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bbe6e-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="bbe6e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbe6e-107">Properties</span></span>
| <span data-ttu-id="bbe6e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbe6e-108">Property</span></span>     | <span data-ttu-id="bbe6e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbe6e-109">Type</span></span>   |<span data-ttu-id="bbe6e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbe6e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbe6e-111">end</span><span class="sxs-lookup"><span data-stu-id="bbe6e-111">end</span></span>|[<span data-ttu-id="bbe6e-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bbe6e-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="bbe6e-113">A hora em que um período inicia.</span><span class="sxs-lookup"><span data-stu-id="bbe6e-113">The time a period begins.</span></span>|
|<span data-ttu-id="bbe6e-114">iniciar</span><span class="sxs-lookup"><span data-stu-id="bbe6e-114">start</span></span>|[<span data-ttu-id="bbe6e-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bbe6e-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="bbe6e-116">A hora em que um período termina.</span><span class="sxs-lookup"><span data-stu-id="bbe6e-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->