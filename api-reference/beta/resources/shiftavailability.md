---
title: tipo de recurso shiftAvailability
description: Disponibilidade do usuário a ser agendada para trabalho e seu padrão de recorrência.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4a284774b76774da0420322f0cd2e092aec6ce83
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952283"
---
# <a name="shiftavailability-resource-type"></a><span data-ttu-id="09d9e-103">tipo de recurso shiftAvailability</span><span class="sxs-lookup"><span data-stu-id="09d9e-103">shiftAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09d9e-104">Disponibilidade do usuário a ser agendada para um [turno](shift.md) e seu padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="09d9e-104">Availability of the user to be scheduled for a [shift](shift.md) and its recurrence pattern.</span></span>

## <a name="properties"></a><span data-ttu-id="09d9e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09d9e-105">Properties</span></span>

| <span data-ttu-id="09d9e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09d9e-106">Property</span></span>     | <span data-ttu-id="09d9e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="09d9e-107">Type</span></span>        | <span data-ttu-id="09d9e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d9e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09d9e-109">recurrence</span><span class="sxs-lookup"><span data-stu-id="09d9e-109">recurrence</span></span>|[<span data-ttu-id="09d9e-110">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="09d9e-110">patternedRecurrence</span></span>](patternedrecurrence.md)| <span data-ttu-id="09d9e-111">Especifica o padrão de recorrência</span><span class="sxs-lookup"><span data-stu-id="09d9e-111">Specifies the pattern for recurrence</span></span> |
|<span data-ttu-id="09d9e-112">Intervalos</span><span class="sxs-lookup"><span data-stu-id="09d9e-112">timeSlots</span></span>|<span data-ttu-id="09d9e-113">coleção [timerange](timerange.md)</span><span class="sxs-lookup"><span data-stu-id="09d9e-113">[timeRange](timerange.md) collection</span></span>|<span data-ttu-id="09d9e-114">O (s) intervalo (s) de tempo preferido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="09d9e-114">The time slot(s) preferred by the user.</span></span>|
|<span data-ttu-id="09d9e-115">timeZone</span><span class="sxs-lookup"><span data-stu-id="09d9e-115">timeZone</span></span>|<span data-ttu-id="09d9e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09d9e-116">String</span></span>|<span data-ttu-id="09d9e-117">Especifica o fuso horário do horário indicado.</span><span class="sxs-lookup"><span data-stu-id="09d9e-117">Specifies the time zone for the indicated time.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="09d9e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09d9e-118">JSON representation</span></span>

<span data-ttu-id="09d9e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09d9e-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftAvailability",
  "baseType": null
}-->

```json
{
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "timeSlots": [{"@odata.type": "microsoft.graph.timeRange"}],
  "timeZone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
