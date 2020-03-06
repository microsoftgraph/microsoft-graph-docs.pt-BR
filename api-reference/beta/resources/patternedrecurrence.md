---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b26a5272611e27ffe29afc0254c1d1384f6a9c69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521987"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="7692e-103">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="7692e-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="7692e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7692e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7692e-105">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="7692e-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="7692e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7692e-106">Properties</span></span>
| <span data-ttu-id="7692e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7692e-107">Property</span></span>     | <span data-ttu-id="7692e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7692e-108">Type</span></span>   |<span data-ttu-id="7692e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7692e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7692e-110">pattern</span><span class="sxs-lookup"><span data-stu-id="7692e-110">pattern</span></span>|[<span data-ttu-id="7692e-111">GetRecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="7692e-111">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="7692e-112">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="7692e-112">The frequency of an event.</span></span>|
|<span data-ttu-id="7692e-113">range</span><span class="sxs-lookup"><span data-stu-id="7692e-113">range</span></span>|[<span data-ttu-id="7692e-114">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="7692e-114">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="7692e-115">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="7692e-115">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7692e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7692e-116">JSON representation</span></span>

<span data-ttu-id="7692e-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7692e-117">Here is a JSON representation of the resource</span></span>

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
