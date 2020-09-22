---
title: tipo de recurso shiftAvailability
description: Disponibilidade do usuário a ser agendada para trabalho e seu padrão de recorrência.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 86ad11ae32977ac07a7755ebe0a169686f6f605e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058050"
---
# <a name="shiftavailability-resource-type"></a><span data-ttu-id="239c3-103">tipo de recurso shiftAvailability</span><span class="sxs-lookup"><span data-stu-id="239c3-103">shiftAvailability resource type</span></span>

<span data-ttu-id="239c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="239c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="239c3-105">Disponibilidade do usuário a ser agendada para um [turno](shift.md) e seu padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="239c3-105">Availability of the user to be scheduled for a [shift](shift.md) and its recurrence pattern.</span></span>

## <a name="properties"></a><span data-ttu-id="239c3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="239c3-106">Properties</span></span>

| <span data-ttu-id="239c3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="239c3-107">Property</span></span>     | <span data-ttu-id="239c3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="239c3-108">Type</span></span>        | <span data-ttu-id="239c3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="239c3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="239c3-110">recurrence</span><span class="sxs-lookup"><span data-stu-id="239c3-110">recurrence</span></span>|[<span data-ttu-id="239c3-111">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="239c3-111">patternedRecurrence</span></span>](patternedrecurrence.md)| <span data-ttu-id="239c3-112">Especifica o padrão de recorrência</span><span class="sxs-lookup"><span data-stu-id="239c3-112">Specifies the pattern for recurrence</span></span> |
|<span data-ttu-id="239c3-113">Intervalos</span><span class="sxs-lookup"><span data-stu-id="239c3-113">timeSlots</span></span>|<span data-ttu-id="239c3-114">coleção [timerange](timerange.md)</span><span class="sxs-lookup"><span data-stu-id="239c3-114">[timeRange](timerange.md) collection</span></span>|<span data-ttu-id="239c3-115">O (s) intervalo (s) de tempo preferido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="239c3-115">The time slot(s) preferred by the user.</span></span>|
|<span data-ttu-id="239c3-116">timeZone</span><span class="sxs-lookup"><span data-stu-id="239c3-116">timeZone</span></span>|<span data-ttu-id="239c3-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="239c3-117">String</span></span>|<span data-ttu-id="239c3-118">Especifica o fuso horário do horário indicado.</span><span class="sxs-lookup"><span data-stu-id="239c3-118">Specifies the time zone for the indicated time.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="239c3-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="239c3-119">JSON representation</span></span>

<span data-ttu-id="239c3-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="239c3-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftAvailability",
  "baseType": null
}-->

```json
{
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "timeSlots": [{"@odata.type": "microsoft.graph.timeRange"}],
  "timeZone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


