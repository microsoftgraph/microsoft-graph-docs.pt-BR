---
title: Tipo de recurso timeSlot
description: Um período de tempo.
ms.openlocfilehash: c1df6ea458bf6742dc20149e62d9760a8a6510e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039803"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="2bcfc-103">Tipo de recurso timeSlot</span><span class="sxs-lookup"><span data-stu-id="2bcfc-103">timeSlot resource type</span></span>

> <span data-ttu-id="2bcfc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2bcfc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bcfc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2bcfc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2bcfc-106">Um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="2bcfc-106">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bcfc-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2bcfc-107">JSON representation</span></span>

<span data-ttu-id="2bcfc-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2bcfc-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="2bcfc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2bcfc-109">Properties</span></span>
| <span data-ttu-id="2bcfc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bcfc-110">Property</span></span>     | <span data-ttu-id="2bcfc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bcfc-111">Type</span></span>   |<span data-ttu-id="2bcfc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bcfc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bcfc-113">end</span><span class="sxs-lookup"><span data-stu-id="2bcfc-113">end</span></span>|[<span data-ttu-id="2bcfc-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2bcfc-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2bcfc-115">A hora em que um período inicia.</span><span class="sxs-lookup"><span data-stu-id="2bcfc-115">The time a period begins.</span></span>|
|<span data-ttu-id="2bcfc-116">iniciar</span><span class="sxs-lookup"><span data-stu-id="2bcfc-116">start</span></span>|[<span data-ttu-id="2bcfc-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2bcfc-117">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2bcfc-118">A hora em que um período termina.</span><span class="sxs-lookup"><span data-stu-id="2bcfc-118">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->