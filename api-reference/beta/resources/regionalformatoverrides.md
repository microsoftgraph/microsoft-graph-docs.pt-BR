---
title: tipo de recurso regionalFormatOverrides
description: Um recurso representando substituições regionais de formatação para calendários, datas e horas.
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 2ed130135571faeced90a638e9334a7e2a185a5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073503"
---
# <a name="regionalformatoverrides-resource-type"></a><span data-ttu-id="76b25-103">tipo de recurso regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="76b25-103">regionalFormatOverrides resource type</span></span>

<span data-ttu-id="76b25-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76b25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76b25-105">Uma coleção de cadeias de caracteres que representam substituições de formatação para calendários, datas e horas.</span><span class="sxs-lookup"><span data-stu-id="76b25-105">A collection of strings representing formatting overrides for calendars, dates, and times.</span></span> 

## <a name="properties"></a><span data-ttu-id="76b25-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76b25-106">Properties</span></span>

|<span data-ttu-id="76b25-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76b25-107">Property</span></span>             |<span data-ttu-id="76b25-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="76b25-108">Type</span></span>                 |<span data-ttu-id="76b25-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="76b25-109">Description</span></span>                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|<span data-ttu-id="76b25-110">calendar</span><span class="sxs-lookup"><span data-stu-id="76b25-110">calendar</span></span>             |<span data-ttu-id="76b25-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76b25-111">String</span></span>               |<span data-ttu-id="76b25-112">O calendário a ser usado, por exemplo, calendário gregoriano.</span><span class="sxs-lookup"><span data-stu-id="76b25-112">The calendar to use, e.g., Gregorian Calendar.</span></span><br><br><span data-ttu-id="76b25-113">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="76b25-113">Returned by default.</span></span>|                   
|<span data-ttu-id="76b25-114">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="76b25-114">firstDayOfWeek</span></span>       |<span data-ttu-id="76b25-115">String</span><span class="sxs-lookup"><span data-stu-id="76b25-115">String</span></span>               |<span data-ttu-id="76b25-116">O primeiro dia da semana a ser usado, por exemplo, domingo.</span><span class="sxs-lookup"><span data-stu-id="76b25-116">The first day of the week to use, e.g., Sunday.</span></span><br><br><span data-ttu-id="76b25-117">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="76b25-117">Returned by default.</span></span>|
|<span data-ttu-id="76b25-118">shortDateFormat</span><span class="sxs-lookup"><span data-stu-id="76b25-118">shortDateFormat</span></span>      |<span data-ttu-id="76b25-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76b25-119">String</span></span>               |<span data-ttu-id="76b25-120">O formato de data de curto prazo a ser usado para exibir datas.</span><span class="sxs-lookup"><span data-stu-id="76b25-120">The short date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="76b25-121">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="76b25-121">Returned by default.</span></span>|
|<span data-ttu-id="76b25-122">longDateFormat</span><span class="sxs-lookup"><span data-stu-id="76b25-122">longDateFormat</span></span>       |<span data-ttu-id="76b25-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76b25-123">String</span></span>               |<span data-ttu-id="76b25-124">O formato de data e hora por extenso a ser usado para exibir datas.</span><span class="sxs-lookup"><span data-stu-id="76b25-124">The long date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="76b25-125">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="76b25-125">Returned by default.</span></span>|
|<span data-ttu-id="76b25-126">shortTimeFormat</span><span class="sxs-lookup"><span data-stu-id="76b25-126">shortTimeFormat</span></span>      |<span data-ttu-id="76b25-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76b25-127">String</span></span>               |<span data-ttu-id="76b25-128">O formato de tempo curto a ser usado para exibir o tempo.</span><span class="sxs-lookup"><span data-stu-id="76b25-128">The short time format to be used for displaying time.</span></span><br><br><span data-ttu-id="76b25-129">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="76b25-129">Returned by default.</span></span>|
|<span data-ttu-id="76b25-130">longTimeFormat</span><span class="sxs-lookup"><span data-stu-id="76b25-130">longTimeFormat</span></span>       |<span data-ttu-id="76b25-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76b25-131">String</span></span>               |<span data-ttu-id="76b25-132">O formato de hora longa a ser usado para exibir o tempo.</span><span class="sxs-lookup"><span data-stu-id="76b25-132">The long time format to be used for displaying time.</span></span><br><br><span data-ttu-id="76b25-133">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="76b25-133">Returned by default.</span></span>|
|<span data-ttu-id="76b25-134">timeZone</span><span class="sxs-lookup"><span data-stu-id="76b25-134">timeZone</span></span>             |<span data-ttu-id="76b25-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76b25-135">String</span></span>               |<span data-ttu-id="76b25-136">O fuso horário a ser usado para exibir o tempo.</span><span class="sxs-lookup"><span data-stu-id="76b25-136">The timezone to be used for displaying time.</span></span><br><br><span data-ttu-id="76b25-137">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="76b25-137">Returned by default.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76b25-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76b25-138">JSON representation</span></span>

<span data-ttu-id="76b25-139">A seguir está uma definição de JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76b25-139">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "",
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


