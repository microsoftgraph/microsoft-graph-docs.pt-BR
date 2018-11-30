---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
ms.openlocfilehash: 10a90db032cd7461e28bc096fd6213df44f3ea45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004438"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="f7983-103">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="f7983-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="f7983-104">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="f7983-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="f7983-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7983-105">Properties</span></span>
| <span data-ttu-id="f7983-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7983-106">Property</span></span>     | <span data-ttu-id="f7983-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7983-107">Type</span></span>   |<span data-ttu-id="f7983-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7983-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7983-109">pattern</span><span class="sxs-lookup"><span data-stu-id="f7983-109">pattern</span></span>|[<span data-ttu-id="f7983-110">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="f7983-110">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="f7983-111">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="f7983-111">The frequency of an event.</span></span>|
|<span data-ttu-id="f7983-112">range</span><span class="sxs-lookup"><span data-stu-id="f7983-112">range</span></span>|[<span data-ttu-id="f7983-113">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="f7983-113">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="f7983-114">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="f7983-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7983-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7983-115">JSON representation</span></span>

<span data-ttu-id="f7983-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f7983-116">Here is a JSON representation of the resource</span></span>

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
