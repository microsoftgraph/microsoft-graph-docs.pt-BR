---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a5ad30474b23c6ef96bbc1a66142098e7f696138
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035564"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="8aacf-103">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="8aacf-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="8aacf-104">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="8aacf-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="8aacf-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8aacf-105">Properties</span></span>
| <span data-ttu-id="8aacf-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8aacf-106">Property</span></span>     | <span data-ttu-id="8aacf-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aacf-107">Type</span></span>   |<span data-ttu-id="8aacf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aacf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8aacf-109">pattern</span><span class="sxs-lookup"><span data-stu-id="8aacf-109">pattern</span></span>|[<span data-ttu-id="8aacf-110">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="8aacf-110">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="8aacf-111">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="8aacf-111">The frequency of an event.</span></span>|
|<span data-ttu-id="8aacf-112">range</span><span class="sxs-lookup"><span data-stu-id="8aacf-112">range</span></span>|[<span data-ttu-id="8aacf-113">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="8aacf-113">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="8aacf-114">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="8aacf-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8aacf-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8aacf-115">JSON representation</span></span>

<span data-ttu-id="8aacf-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8aacf-116">Here is a JSON representation of the resource</span></span>

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
