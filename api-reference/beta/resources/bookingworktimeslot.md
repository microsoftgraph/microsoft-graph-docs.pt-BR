---
title: tipo de recurso de bookingWorkTimeSlot
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a193843617d5acc7e18d8a06993a1629b80762be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513785"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="e5604-104">tipo de recurso de bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="e5604-104">bookingWorkTimeSlot resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="e5604-105">Os horários de início e término para trabalho.</span><span class="sxs-lookup"><span data-stu-id="e5604-105">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="e5604-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5604-106">Properties</span></span>
| <span data-ttu-id="e5604-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5604-107">Property</span></span>     | <span data-ttu-id="e5604-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5604-108">Type</span></span>   |<span data-ttu-id="e5604-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5604-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5604-110">end</span><span class="sxs-lookup"><span data-stu-id="e5604-110">end</span></span>|<span data-ttu-id="e5604-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e5604-111">TimeOfDay</span></span>|<span data-ttu-id="e5604-112">A hora do dia em que trabalham inicia.</span><span class="sxs-lookup"><span data-stu-id="e5604-112">The time of the day that work starts.</span></span> <span data-ttu-id="e5604-113">Por exemplo, 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="e5604-113">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="e5604-114">start</span><span class="sxs-lookup"><span data-stu-id="e5604-114">start</span></span>|<span data-ttu-id="e5604-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e5604-115">TimeOfDay</span></span>|<span data-ttu-id="e5604-116">A hora do dia em que trabalham paradas.</span><span class="sxs-lookup"><span data-stu-id="e5604-116">The time of the day that work stops.</span></span> <span data-ttu-id="e5604-117">Por exemplo, 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="e5604-117">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5604-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5604-118">JSON representation</span></span>

<span data-ttu-id="e5604-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5604-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingworktimeslot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
