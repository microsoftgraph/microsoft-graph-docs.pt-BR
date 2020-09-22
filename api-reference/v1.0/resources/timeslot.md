---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 874b587db2bb9e2234fcacca9b3e3b0cf5c2f89b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090750"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="36bda-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="36bda-103">timeSlot resource type</span></span>

<span data-ttu-id="36bda-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36bda-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36bda-105">Representa um intervalo de tempo para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="36bda-105">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="36bda-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36bda-106">JSON representation</span></span>

<span data-ttu-id="36bda-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="36bda-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="36bda-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36bda-108">Properties</span></span>
| <span data-ttu-id="36bda-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36bda-109">Property</span></span>     | <span data-ttu-id="36bda-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="36bda-110">Type</span></span>   |<span data-ttu-id="36bda-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="36bda-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36bda-112">end</span><span class="sxs-lookup"><span data-stu-id="36bda-112">end</span></span>|[<span data-ttu-id="36bda-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="36bda-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="36bda-114">A data, a hora e o fuso horário em que um período começa.</span><span class="sxs-lookup"><span data-stu-id="36bda-114">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="36bda-115">iniciar</span><span class="sxs-lookup"><span data-stu-id="36bda-115">start</span></span>|[<span data-ttu-id="36bda-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="36bda-116">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="36bda-117">A data, a hora e o fuso horário que um período termina.</span><span class="sxs-lookup"><span data-stu-id="36bda-117">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

