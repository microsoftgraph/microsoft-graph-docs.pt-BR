---
title: tipo de recurso bookingWorkTimeSlot
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: dadeebfe65a8d502b8a401f551638c09f637625f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071653"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="add29-104">tipo de recurso bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="add29-104">bookingWorkTimeSlot resource type</span></span>

<span data-ttu-id="add29-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="add29-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="add29-106">As horas de início e de término do trabalho.</span><span class="sxs-lookup"><span data-stu-id="add29-106">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="add29-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="add29-107">Properties</span></span>
| <span data-ttu-id="add29-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="add29-108">Property</span></span>     | <span data-ttu-id="add29-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="add29-109">Type</span></span>   |<span data-ttu-id="add29-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="add29-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="add29-111">end</span><span class="sxs-lookup"><span data-stu-id="add29-111">end</span></span>|<span data-ttu-id="add29-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="add29-112">TimeOfDay</span></span>|<span data-ttu-id="add29-113">A hora do dia em que o trabalho é iniciado.</span><span class="sxs-lookup"><span data-stu-id="add29-113">The time of the day that work starts.</span></span> <span data-ttu-id="add29-114">Por exemplo, 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="add29-114">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="add29-115">iniciar</span><span class="sxs-lookup"><span data-stu-id="add29-115">start</span></span>|<span data-ttu-id="add29-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="add29-116">TimeOfDay</span></span>|<span data-ttu-id="add29-117">A hora do dia em que o trabalho é interrompido.</span><span class="sxs-lookup"><span data-stu-id="add29-117">The time of the day that work stops.</span></span> <span data-ttu-id="add29-118">Por exemplo, 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="add29-118">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="add29-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="add29-119">JSON representation</span></span>

<span data-ttu-id="add29-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="add29-120">The following is a JSON representation of the resource.</span></span>

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


