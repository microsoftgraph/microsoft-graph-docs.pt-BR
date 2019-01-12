---
title: tipo de recurso de bookingWorkTimeSlot
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 33dd856d678d2cf1ba9da2a747c0bd46f2fd4932
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968481"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="1e5f1-104">tipo de recurso de bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="1e5f1-104">bookingWorkTimeSlot resource type</span></span>

 > <span data-ttu-id="1e5f1-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1e5f1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e5f1-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1e5f1-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="1e5f1-107">Os horários de início e término para trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e5f1-107">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="1e5f1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e5f1-108">Properties</span></span>
| <span data-ttu-id="1e5f1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e5f1-109">Property</span></span>     | <span data-ttu-id="1e5f1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e5f1-110">Type</span></span>   |<span data-ttu-id="1e5f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e5f1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e5f1-112">end</span><span class="sxs-lookup"><span data-stu-id="1e5f1-112">end</span></span>|<span data-ttu-id="1e5f1-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1e5f1-113">TimeOfDay</span></span>|<span data-ttu-id="1e5f1-114">A hora do dia em que trabalham inicia.</span><span class="sxs-lookup"><span data-stu-id="1e5f1-114">The time of the day that work starts.</span></span> <span data-ttu-id="1e5f1-115">Por exemplo, 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="1e5f1-115">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="1e5f1-116">start</span><span class="sxs-lookup"><span data-stu-id="1e5f1-116">start</span></span>|<span data-ttu-id="1e5f1-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1e5f1-117">TimeOfDay</span></span>|<span data-ttu-id="1e5f1-118">A hora do dia em que trabalham paradas.</span><span class="sxs-lookup"><span data-stu-id="1e5f1-118">The time of the day that work stops.</span></span> <span data-ttu-id="1e5f1-119">Por exemplo, 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="1e5f1-119">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e5f1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e5f1-120">JSON representation</span></span>

<span data-ttu-id="1e5f1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e5f1-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkTimeSlot"
}-->

```json
{
  "end": "String (timestamp)",
  "start": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
