---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ff02706768feed52eaf6b85294e496211d9d711f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519698"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="6171c-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="6171c-103">timeSlot resource type</span></span>

<span data-ttu-id="6171c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6171c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6171c-105">Representa um intervalo de tempo para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="6171c-105">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6171c-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6171c-106">JSON representation</span></span>

<span data-ttu-id="6171c-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6171c-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6171c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6171c-108">Properties</span></span>
| <span data-ttu-id="6171c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6171c-109">Property</span></span>     | <span data-ttu-id="6171c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6171c-110">Type</span></span>   |<span data-ttu-id="6171c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6171c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6171c-112">end</span><span class="sxs-lookup"><span data-stu-id="6171c-112">end</span></span>|[<span data-ttu-id="6171c-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6171c-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6171c-114">A data, a hora e o fuso horário em que um período começa.</span><span class="sxs-lookup"><span data-stu-id="6171c-114">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="6171c-115">iniciar</span><span class="sxs-lookup"><span data-stu-id="6171c-115">start</span></span>|[<span data-ttu-id="6171c-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6171c-116">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6171c-117">A data, a hora e o fuso horário que um período termina.</span><span class="sxs-lookup"><span data-stu-id="6171c-117">The date, time, and time zone that a period ends.</span></span>|

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
