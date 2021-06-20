---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5bc4c78a4996c6690f40de863d20ba6f2d55949a
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030870"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="d40c8-103">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="d40c8-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="d40c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d40c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d40c8-105">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="d40c8-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="d40c8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d40c8-106">Properties</span></span>
| <span data-ttu-id="d40c8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d40c8-107">Property</span></span>     | <span data-ttu-id="d40c8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d40c8-108">Type</span></span>   |<span data-ttu-id="d40c8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d40c8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d40c8-110">pattern</span><span class="sxs-lookup"><span data-stu-id="d40c8-110">pattern</span></span>|[<span data-ttu-id="d40c8-111">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="d40c8-111">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="d40c8-112">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="d40c8-112">The frequency of an event.</span></span> <span data-ttu-id="d40c8-113">Não especifique para uma revisão de acesso único.</span><span class="sxs-lookup"><span data-stu-id="d40c8-113">Do not specify for a one-time access review.</span></span>|
|<span data-ttu-id="d40c8-114">range</span><span class="sxs-lookup"><span data-stu-id="d40c8-114">range</span></span>|[<span data-ttu-id="d40c8-115">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="d40c8-115">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="d40c8-116">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="d40c8-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d40c8-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d40c8-117">JSON representation</span></span>

<span data-ttu-id="d40c8-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d40c8-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

