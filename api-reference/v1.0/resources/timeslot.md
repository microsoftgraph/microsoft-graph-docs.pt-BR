---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 378a7ac71058ec80c9ce20ee0959c1dc5c3ce091
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474680"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="28316-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="28316-103">timeSlot resource type</span></span>

<span data-ttu-id="28316-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28316-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28316-105">Representa um intervalo de tempo para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="28316-105">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="28316-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28316-106">JSON representation</span></span>

<span data-ttu-id="28316-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="28316-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="28316-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28316-108">Properties</span></span>
| <span data-ttu-id="28316-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28316-109">Property</span></span>     | <span data-ttu-id="28316-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="28316-110">Type</span></span>   |<span data-ttu-id="28316-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="28316-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28316-112">end</span><span class="sxs-lookup"><span data-stu-id="28316-112">end</span></span>|[<span data-ttu-id="28316-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="28316-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="28316-114">A data, hora e fuso horário que um período começa.</span><span class="sxs-lookup"><span data-stu-id="28316-114">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="28316-115">iniciar</span><span class="sxs-lookup"><span data-stu-id="28316-115">start</span></span>|[<span data-ttu-id="28316-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="28316-116">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="28316-117">A data, hora e fuso horário que um período termina.</span><span class="sxs-lookup"><span data-stu-id="28316-117">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

