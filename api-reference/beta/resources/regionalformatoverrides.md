---
title: Tipo de recurso regionalFormatOverrides
description: Um recurso que representa substituições de formatação regional para calendários, datas e horários.
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 2b4046ad8ec6b2d646d1dc2d93cbe7bed205cbad
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516063"
---
# <a name="regionalformatoverrides-resource-type"></a><span data-ttu-id="66e2e-103">Tipo de recurso regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="66e2e-103">regionalFormatOverrides resource type</span></span>

<span data-ttu-id="66e2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66e2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66e2e-105">Uma coleção de cadeias de caracteres que representa substituições de formatação para calendários, datas e horários.</span><span class="sxs-lookup"><span data-stu-id="66e2e-105">A collection of strings representing formatting overrides for calendars, dates, and times.</span></span> 

## <a name="properties"></a><span data-ttu-id="66e2e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66e2e-106">Properties</span></span>

|<span data-ttu-id="66e2e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66e2e-107">Property</span></span>             |<span data-ttu-id="66e2e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="66e2e-108">Type</span></span>                     |<span data-ttu-id="66e2e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="66e2e-109">Description</span></span>                                                    |
|---------------------|-------------------------|---------------------------------------------------------------|
|<span data-ttu-id="66e2e-110">calendar</span><span class="sxs-lookup"><span data-stu-id="66e2e-110">calendar</span></span>             |<span data-ttu-id="66e2e-111">String</span><span class="sxs-lookup"><span data-stu-id="66e2e-111">String</span></span>                   |<span data-ttu-id="66e2e-112">O calendário a ser usado, por exemplo, Calendário Gregoriano.</span><span class="sxs-lookup"><span data-stu-id="66e2e-112">The calendar to use, e.g., Gregorian Calendar.</span></span><br><br><span data-ttu-id="66e2e-113">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="66e2e-113">Returned by default.</span></span>|                   
|<span data-ttu-id="66e2e-114">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="66e2e-114">firstDayOfWeek</span></span>       |<span data-ttu-id="66e2e-115">microsoft.graph.dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="66e2e-115">microsoft.graph.dayOfWeek</span></span>|<span data-ttu-id="66e2e-116">O primeiro dia da semana a ser usado, por exemplo, domingo.</span><span class="sxs-lookup"><span data-stu-id="66e2e-116">The first day of the week to use, e.g., Sunday.</span></span><br><br><span data-ttu-id="66e2e-117">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="66e2e-117">Returned by default.</span></span>|
|<span data-ttu-id="66e2e-118">shortDateFormat</span><span class="sxs-lookup"><span data-stu-id="66e2e-118">shortDateFormat</span></span>      |<span data-ttu-id="66e2e-119">String</span><span class="sxs-lookup"><span data-stu-id="66e2e-119">String</span></span>                   |<span data-ttu-id="66e2e-120">O formato de tempo curto a ser usado para exibição de datas.</span><span class="sxs-lookup"><span data-stu-id="66e2e-120">The short date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="66e2e-121">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="66e2e-121">Returned by default.</span></span>|
|<span data-ttu-id="66e2e-122">longDateFormat</span><span class="sxs-lookup"><span data-stu-id="66e2e-122">longDateFormat</span></span>       |<span data-ttu-id="66e2e-123">String</span><span class="sxs-lookup"><span data-stu-id="66e2e-123">String</span></span>                   |<span data-ttu-id="66e2e-124">O formato de data longa a ser usado para exibição de datas.</span><span class="sxs-lookup"><span data-stu-id="66e2e-124">The long date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="66e2e-125">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="66e2e-125">Returned by default.</span></span>|
|<span data-ttu-id="66e2e-126">shortTimeFormat</span><span class="sxs-lookup"><span data-stu-id="66e2e-126">shortTimeFormat</span></span>      |<span data-ttu-id="66e2e-127">String</span><span class="sxs-lookup"><span data-stu-id="66e2e-127">String</span></span>                   |<span data-ttu-id="66e2e-128">O formato de tempo curto a ser usado para exibição de tempo.</span><span class="sxs-lookup"><span data-stu-id="66e2e-128">The short time format to be used for displaying time.</span></span><br><br><span data-ttu-id="66e2e-129">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="66e2e-129">Returned by default.</span></span>|
|<span data-ttu-id="66e2e-130">longTimeFormat</span><span class="sxs-lookup"><span data-stu-id="66e2e-130">longTimeFormat</span></span>       |<span data-ttu-id="66e2e-131">String</span><span class="sxs-lookup"><span data-stu-id="66e2e-131">String</span></span>                   |<span data-ttu-id="66e2e-132">O formato de longo tempo a ser usado para exibição de tempo.</span><span class="sxs-lookup"><span data-stu-id="66e2e-132">The long time format to be used for displaying time.</span></span><br><br><span data-ttu-id="66e2e-133">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="66e2e-133">Returned by default.</span></span>|
|<span data-ttu-id="66e2e-134">timeZone</span><span class="sxs-lookup"><span data-stu-id="66e2e-134">timeZone</span></span>             |<span data-ttu-id="66e2e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66e2e-135">String</span></span>                   |<span data-ttu-id="66e2e-136">O timezone a ser usado para exibição de tempo.</span><span class="sxs-lookup"><span data-stu-id="66e2e-136">The timezone to be used for displaying time.</span></span><br><br><span data-ttu-id="66e2e-137">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="66e2e-137">Returned by default.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66e2e-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66e2e-138">JSON representation</span></span>

<span data-ttu-id="66e2e-139">A seguir está uma definição JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66e2e-139">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.regionalFormatOverrides"
}-->

```json
{
    "calendar": "string",
    "firstDayOfWeek": "string",
    "shortDateFormat": "string",
    "longDateFormat": "string",
    "shortTimeFormat": "string",
    "longTimeFormat": "string",
    "timeZone": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalFormatOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


