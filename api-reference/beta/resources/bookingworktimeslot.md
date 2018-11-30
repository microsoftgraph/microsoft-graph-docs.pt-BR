---
title: tipo de recurso de bookingWorkTimeSlot
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 61436ca3e94ab15c44fc1898827a3de511c8ee94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036082"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="6b233-104">tipo de recurso de bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="6b233-104">bookingWorkTimeSlot resource type</span></span>

 > <span data-ttu-id="6b233-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6b233-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b233-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6b233-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="6b233-107">Os horários de início e término para trabalho.</span><span class="sxs-lookup"><span data-stu-id="6b233-107">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="6b233-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b233-108">Properties</span></span>
| <span data-ttu-id="6b233-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b233-109">Property</span></span>     | <span data-ttu-id="6b233-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b233-110">Type</span></span>   |<span data-ttu-id="6b233-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b233-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b233-112">end</span><span class="sxs-lookup"><span data-stu-id="6b233-112">end</span></span>|<span data-ttu-id="6b233-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6b233-113">TimeOfDay</span></span>|<span data-ttu-id="6b233-114">A hora do dia em que trabalham inicia.</span><span class="sxs-lookup"><span data-stu-id="6b233-114">The time of the day that work starts.</span></span> <span data-ttu-id="6b233-115">Por exemplo, 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="6b233-115">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="6b233-116">start</span><span class="sxs-lookup"><span data-stu-id="6b233-116">start</span></span>|<span data-ttu-id="6b233-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6b233-117">TimeOfDay</span></span>|<span data-ttu-id="6b233-118">A hora do dia em que trabalham paradas.</span><span class="sxs-lookup"><span data-stu-id="6b233-118">The time of the day that work stops.</span></span> <span data-ttu-id="6b233-119">Por exemplo, 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="6b233-119">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b233-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b233-120">JSON representation</span></span>

<span data-ttu-id="6b233-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b233-121">The following is a JSON representation of the resource.</span></span>

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