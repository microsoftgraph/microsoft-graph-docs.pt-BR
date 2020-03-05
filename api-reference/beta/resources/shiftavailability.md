---
title: tipo de recurso shiftAvailability
description: Disponibilidade do usuário a ser agendada para trabalho e seu padrão de recorrência.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8e06b64bc01be163149468c9090df2a8ea59497d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520622"
---
# <a name="shiftavailability-resource-type"></a><span data-ttu-id="5ba4e-103">tipo de recurso shiftAvailability</span><span class="sxs-lookup"><span data-stu-id="5ba4e-103">shiftAvailability resource type</span></span>

<span data-ttu-id="5ba4e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5ba4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ba4e-105">Disponibilidade do usuário a ser agendada para um [turno](shift.md) e seu padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="5ba4e-105">Availability of the user to be scheduled for a [shift](shift.md) and its recurrence pattern.</span></span>

## <a name="properties"></a><span data-ttu-id="5ba4e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ba4e-106">Properties</span></span>

| <span data-ttu-id="5ba4e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ba4e-107">Property</span></span>     | <span data-ttu-id="5ba4e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ba4e-108">Type</span></span>        | <span data-ttu-id="5ba4e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ba4e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5ba4e-110">recurrence</span><span class="sxs-lookup"><span data-stu-id="5ba4e-110">recurrence</span></span>|[<span data-ttu-id="5ba4e-111">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="5ba4e-111">patternedRecurrence</span></span>](patternedrecurrence.md)| <span data-ttu-id="5ba4e-112">Especifica o padrão de recorrência</span><span class="sxs-lookup"><span data-stu-id="5ba4e-112">Specifies the pattern for recurrence</span></span> |
|<span data-ttu-id="5ba4e-113">Intervalos</span><span class="sxs-lookup"><span data-stu-id="5ba4e-113">timeSlots</span></span>|<span data-ttu-id="5ba4e-114">coleção [timerange](timerange.md)</span><span class="sxs-lookup"><span data-stu-id="5ba4e-114">[timeRange](timerange.md) collection</span></span>|<span data-ttu-id="5ba4e-115">O (s) intervalo (s) de tempo preferido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="5ba4e-115">The time slot(s) preferred by the user.</span></span>|
|<span data-ttu-id="5ba4e-116">timeZone</span><span class="sxs-lookup"><span data-stu-id="5ba4e-116">timeZone</span></span>|<span data-ttu-id="5ba4e-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ba4e-117">String</span></span>|<span data-ttu-id="5ba4e-118">Especifica o fuso horário do horário indicado.</span><span class="sxs-lookup"><span data-stu-id="5ba4e-118">Specifies the time zone for the indicated time.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5ba4e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ba4e-119">JSON representation</span></span>

<span data-ttu-id="5ba4e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ba4e-120">The following is a JSON representation of the resource.</span></span>

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
