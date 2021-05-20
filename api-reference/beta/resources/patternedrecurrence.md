---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: harini84
ms.openlocfilehash: baff2147ee0a9e03e4e55a143341171707dee2d7
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579299"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="bbe3b-103">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="bbe3b-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="bbe3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbe3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbe3b-105">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="bbe3b-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="bbe3b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbe3b-106">Properties</span></span>
| <span data-ttu-id="bbe3b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbe3b-107">Property</span></span>     | <span data-ttu-id="bbe3b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbe3b-108">Type</span></span>   |<span data-ttu-id="bbe3b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbe3b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbe3b-110">pattern</span><span class="sxs-lookup"><span data-stu-id="bbe3b-110">pattern</span></span>|[<span data-ttu-id="bbe3b-111">recurrencePattern</span><span class="sxs-lookup"><span data-stu-id="bbe3b-111">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="bbe3b-112">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="bbe3b-112">The frequency of an event.</span></span> <span data-ttu-id="bbe3b-113">Não especifique para uma revisão de acesso único.</span><span class="sxs-lookup"><span data-stu-id="bbe3b-113">Do not specify for a one-time access review.</span></span>|
|<span data-ttu-id="bbe3b-114">intervalo</span><span class="sxs-lookup"><span data-stu-id="bbe3b-114">range</span></span>|[<span data-ttu-id="bbe3b-115">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="bbe3b-115">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="bbe3b-116">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="bbe3b-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbe3b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbe3b-117">JSON representation</span></span>

<span data-ttu-id="bbe3b-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bbe3b-118">Here is a JSON representation of the resource</span></span>

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


