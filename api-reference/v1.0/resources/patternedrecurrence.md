---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 77c413f98e4c329e7dc7ebcb2412ac12bedfad8d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447224"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="7fe4b-103">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="7fe4b-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="7fe4b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7fe4b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7fe4b-105">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="7fe4b-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="7fe4b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7fe4b-106">Properties</span></span>
| <span data-ttu-id="7fe4b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fe4b-107">Property</span></span>     | <span data-ttu-id="7fe4b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fe4b-108">Type</span></span>   |<span data-ttu-id="7fe4b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fe4b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7fe4b-110">pattern</span><span class="sxs-lookup"><span data-stu-id="7fe4b-110">pattern</span></span>|[<span data-ttu-id="7fe4b-111">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="7fe4b-111">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="7fe4b-112">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="7fe4b-112">The frequency of an event.</span></span>|
|<span data-ttu-id="7fe4b-113">range</span><span class="sxs-lookup"><span data-stu-id="7fe4b-113">range</span></span>|[<span data-ttu-id="7fe4b-114">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="7fe4b-114">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="7fe4b-115">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="7fe4b-115">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7fe4b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7fe4b-116">JSON representation</span></span>

<span data-ttu-id="7fe4b-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7fe4b-117">Here is a JSON representation of the resource</span></span>

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
