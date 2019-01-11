---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
ms.openlocfilehash: 2c2d68046c69ed702738318121a0289eb6a347a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825241"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="3167b-103">Tipo de recurso patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="3167b-103">patternedRecurrence resource type</span></span>

> <span data-ttu-id="3167b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3167b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3167b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3167b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3167b-106">O padrão e o intervalo da recorrência.</span><span class="sxs-lookup"><span data-stu-id="3167b-106">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="3167b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3167b-107">Properties</span></span>
| <span data-ttu-id="3167b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3167b-108">Property</span></span>     | <span data-ttu-id="3167b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3167b-109">Type</span></span>   |<span data-ttu-id="3167b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3167b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3167b-111">pattern</span><span class="sxs-lookup"><span data-stu-id="3167b-111">pattern</span></span>|[<span data-ttu-id="3167b-112">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="3167b-112">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="3167b-113">A frequência de um evento.</span><span class="sxs-lookup"><span data-stu-id="3167b-113">The frequency of an event.</span></span>|
|<span data-ttu-id="3167b-114">range</span><span class="sxs-lookup"><span data-stu-id="3167b-114">range</span></span>|[<span data-ttu-id="3167b-115">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="3167b-115">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="3167b-116">A duração de um evento.</span><span class="sxs-lookup"><span data-stu-id="3167b-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3167b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3167b-117">JSON representation</span></span>

<span data-ttu-id="3167b-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3167b-118">Here is a JSON representation of the resource</span></span>

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
