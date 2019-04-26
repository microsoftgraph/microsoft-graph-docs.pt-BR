---
title: tipo de recurso bookingWorkTimeSlot
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a6063b8ee5c1c40476f676c3a9846fa7d7aab421
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338773"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="d2e98-104">tipo de recurso bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="d2e98-104">bookingWorkTimeSlot resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="d2e98-105">As horas de início e de término do trabalho.</span><span class="sxs-lookup"><span data-stu-id="d2e98-105">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="d2e98-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2e98-106">Properties</span></span>
| <span data-ttu-id="d2e98-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2e98-107">Property</span></span>     | <span data-ttu-id="d2e98-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2e98-108">Type</span></span>   |<span data-ttu-id="d2e98-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2e98-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2e98-110">end</span><span class="sxs-lookup"><span data-stu-id="d2e98-110">end</span></span>|<span data-ttu-id="d2e98-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d2e98-111">TimeOfDay</span></span>|<span data-ttu-id="d2e98-112">A hora do dia em que o trabalho é iniciado.</span><span class="sxs-lookup"><span data-stu-id="d2e98-112">The time of the day that work starts.</span></span> <span data-ttu-id="d2e98-113">Por exemplo, 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="d2e98-113">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="d2e98-114">iniciar</span><span class="sxs-lookup"><span data-stu-id="d2e98-114">start</span></span>|<span data-ttu-id="d2e98-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d2e98-115">TimeOfDay</span></span>|<span data-ttu-id="d2e98-116">A hora do dia em que o trabalho é interrompido.</span><span class="sxs-lookup"><span data-stu-id="d2e98-116">The time of the day that work stops.</span></span> <span data-ttu-id="d2e98-117">Por exemplo, 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="d2e98-117">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2e98-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2e98-118">JSON representation</span></span>

<span data-ttu-id="d2e98-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2e98-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
