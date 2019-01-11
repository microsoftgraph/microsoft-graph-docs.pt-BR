---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
ms.openlocfilehash: 1f383a7feafbb3816ef838d8f0667eebdd42443f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877928"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="05223-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="05223-103">timeSlot resource type</span></span>

> <span data-ttu-id="05223-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="05223-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05223-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="05223-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05223-106">Um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="05223-106">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05223-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05223-107">JSON representation</span></span>

<span data-ttu-id="05223-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="05223-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="05223-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05223-109">Properties</span></span>
| <span data-ttu-id="05223-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05223-110">Property</span></span>     | <span data-ttu-id="05223-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="05223-111">Type</span></span>   |<span data-ttu-id="05223-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="05223-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05223-113">end</span><span class="sxs-lookup"><span data-stu-id="05223-113">end</span></span>|[<span data-ttu-id="05223-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="05223-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="05223-115">A hora em que um período inicia.</span><span class="sxs-lookup"><span data-stu-id="05223-115">The time a period begins.</span></span>|
|<span data-ttu-id="05223-116">iniciar</span><span class="sxs-lookup"><span data-stu-id="05223-116">start</span></span>|[<span data-ttu-id="05223-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="05223-117">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="05223-118">A hora em que um período termina.</span><span class="sxs-lookup"><span data-stu-id="05223-118">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
