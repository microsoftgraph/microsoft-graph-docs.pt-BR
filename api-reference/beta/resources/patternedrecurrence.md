---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
ms.openlocfilehash: 063df70dfeeb1d37cfc5e23710108dd4cfc9ae57
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344912"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="5a261-103">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="5a261-103">patternedRecurrence resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a261-104">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="5a261-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="5a261-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a261-105">Properties</span></span>
| <span data-ttu-id="5a261-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a261-106">Property</span></span>     | <span data-ttu-id="5a261-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a261-107">Type</span></span>   |<span data-ttu-id="5a261-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a261-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a261-109">pattern</span><span class="sxs-lookup"><span data-stu-id="5a261-109">pattern</span></span>|[<span data-ttu-id="5a261-110">GetRecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="5a261-110">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="5a261-111">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="5a261-111">The frequency of an event.</span></span>|
|<span data-ttu-id="5a261-112">range</span><span class="sxs-lookup"><span data-stu-id="5a261-112">range</span></span>|[<span data-ttu-id="5a261-113">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="5a261-113">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="5a261-114">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="5a261-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a261-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a261-115">JSON representation</span></span>

<span data-ttu-id="5a261-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5a261-116">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
