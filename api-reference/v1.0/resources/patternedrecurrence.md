---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 57e42faaaa30be31c45be7bfec6ad9ee17ffc869
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546200"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="d9baa-103">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="d9baa-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="d9baa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9baa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9baa-105">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="d9baa-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="d9baa-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9baa-106">Properties</span></span>
| <span data-ttu-id="d9baa-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9baa-107">Property</span></span>     | <span data-ttu-id="d9baa-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9baa-108">Type</span></span>   |<span data-ttu-id="d9baa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9baa-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9baa-110">pattern</span><span class="sxs-lookup"><span data-stu-id="d9baa-110">pattern</span></span>|[<span data-ttu-id="d9baa-111">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="d9baa-111">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="d9baa-112">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="d9baa-112">The frequency of an event.</span></span>|
|<span data-ttu-id="d9baa-113">range</span><span class="sxs-lookup"><span data-stu-id="d9baa-113">range</span></span>|[<span data-ttu-id="d9baa-114">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="d9baa-114">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="d9baa-115">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="d9baa-115">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9baa-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9baa-116">JSON representation</span></span>

<span data-ttu-id="d9baa-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d9baa-117">Here is a JSON representation of the resource</span></span>

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

