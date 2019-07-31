---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 463e3324d3a32d0679584a3aa2dddbe6613d2925
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966192"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="d2928-103">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="d2928-103">patternedRecurrence resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2928-104">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="d2928-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="d2928-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2928-105">Properties</span></span>
| <span data-ttu-id="d2928-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2928-106">Property</span></span>     | <span data-ttu-id="d2928-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2928-107">Type</span></span>   |<span data-ttu-id="d2928-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2928-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2928-109">pattern</span><span class="sxs-lookup"><span data-stu-id="d2928-109">pattern</span></span>|[<span data-ttu-id="d2928-110">GetRecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="d2928-110">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="d2928-111">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="d2928-111">The frequency of an event.</span></span>|
|<span data-ttu-id="d2928-112">range</span><span class="sxs-lookup"><span data-stu-id="d2928-112">range</span></span>|[<span data-ttu-id="d2928-113">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="d2928-113">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="d2928-114">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="d2928-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2928-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2928-115">JSON representation</span></span>

<span data-ttu-id="d2928-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d2928-116">Here is a JSON representation of the resource</span></span>

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
