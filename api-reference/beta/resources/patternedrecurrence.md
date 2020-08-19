---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 7ca993e0639e532338ade3c3e1dc57d1baf284fc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807154"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="5aecb-103">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="5aecb-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="5aecb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aecb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aecb-105">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="5aecb-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="5aecb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5aecb-106">Properties</span></span>
| <span data-ttu-id="5aecb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5aecb-107">Property</span></span>     | <span data-ttu-id="5aecb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5aecb-108">Type</span></span>   |<span data-ttu-id="5aecb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aecb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5aecb-110">pattern</span><span class="sxs-lookup"><span data-stu-id="5aecb-110">pattern</span></span>|[<span data-ttu-id="5aecb-111">GetRecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="5aecb-111">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="5aecb-112">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="5aecb-112">The frequency of an event.</span></span>|
|<span data-ttu-id="5aecb-113">range</span><span class="sxs-lookup"><span data-stu-id="5aecb-113">range</span></span>|[<span data-ttu-id="5aecb-114">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="5aecb-114">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="5aecb-115">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="5aecb-115">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5aecb-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5aecb-116">JSON representation</span></span>

<span data-ttu-id="5aecb-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5aecb-117">Here is a JSON representation of the resource</span></span>

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
