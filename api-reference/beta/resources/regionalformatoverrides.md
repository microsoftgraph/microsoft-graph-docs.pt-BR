---
title: tipo de recurso regionalFormatOverrides
description: Um recurso representando substituições regionais de formatação para calendários, datas e horas.
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 437b67f6a99017bb20096dbd20451b7662145cbd
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777593"
---
# <a name="regionalformatoverrides-resource-type"></a><span data-ttu-id="a9588-103">tipo de recurso regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="a9588-103">regionalFormatOverrides resource type</span></span>

<span data-ttu-id="a9588-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9588-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9588-105">Uma coleção de cadeias de caracteres que representam substituições de formatação para calendários, datas e horas.</span><span class="sxs-lookup"><span data-stu-id="a9588-105">A collection of strings representing formatting overrides for calendars, dates, and times.</span></span> 

## <a name="properties"></a><span data-ttu-id="a9588-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9588-106">Properties</span></span>

|<span data-ttu-id="a9588-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9588-107">Property</span></span>             |<span data-ttu-id="a9588-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9588-108">Type</span></span>                 |<span data-ttu-id="a9588-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9588-109">Description</span></span>                                                    |
|---------------------|---------------------|---------------------------------------------------------------|
|<span data-ttu-id="a9588-110">calendar</span><span class="sxs-lookup"><span data-stu-id="a9588-110">calendar</span></span>             |<span data-ttu-id="a9588-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9588-111">String</span></span>               |<span data-ttu-id="a9588-112">O calendário a ser usado, por exemplo, calendário gregoriano.</span><span class="sxs-lookup"><span data-stu-id="a9588-112">The calendar to use, e.g., Gregorian Calendar.</span></span><br><br><span data-ttu-id="a9588-113">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="a9588-113">Returned by default.</span></span>|                   
|<span data-ttu-id="a9588-114">firstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="a9588-114">firstDayOfWeek</span></span>       |<span data-ttu-id="a9588-115">String</span><span class="sxs-lookup"><span data-stu-id="a9588-115">String</span></span>               |<span data-ttu-id="a9588-116">O primeiro dia da semana a ser usado, por exemplo, domingo.</span><span class="sxs-lookup"><span data-stu-id="a9588-116">The first day of the week to use, e.g., Sunday.</span></span><br><br><span data-ttu-id="a9588-117">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="a9588-117">Returned by default.</span></span>|
|<span data-ttu-id="a9588-118">shortDateFormat</span><span class="sxs-lookup"><span data-stu-id="a9588-118">shortDateFormat</span></span>      |<span data-ttu-id="a9588-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9588-119">String</span></span>               |<span data-ttu-id="a9588-120">O formato de data de curto prazo a ser usado para exibir datas.</span><span class="sxs-lookup"><span data-stu-id="a9588-120">The short date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="a9588-121">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="a9588-121">Returned by default.</span></span>|
|<span data-ttu-id="a9588-122">longDateFormat</span><span class="sxs-lookup"><span data-stu-id="a9588-122">longDateFormat</span></span>       |<span data-ttu-id="a9588-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9588-123">String</span></span>               |<span data-ttu-id="a9588-124">O formato de data e hora por extenso a ser usado para exibir datas.</span><span class="sxs-lookup"><span data-stu-id="a9588-124">The long date time format to be used for displaying dates.</span></span><br><br><span data-ttu-id="a9588-125">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="a9588-125">Returned by default.</span></span>|
|<span data-ttu-id="a9588-126">shortTimeFormat</span><span class="sxs-lookup"><span data-stu-id="a9588-126">shortTimeFormat</span></span>      |<span data-ttu-id="a9588-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9588-127">String</span></span>               |<span data-ttu-id="a9588-128">O formato de tempo curto a ser usado para exibir o tempo.</span><span class="sxs-lookup"><span data-stu-id="a9588-128">The short time format to be used for displaying time.</span></span><br><br><span data-ttu-id="a9588-129">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="a9588-129">Returned by default.</span></span>|
|<span data-ttu-id="a9588-130">longTimeFormat</span><span class="sxs-lookup"><span data-stu-id="a9588-130">longTimeFormat</span></span>       |<span data-ttu-id="a9588-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9588-131">String</span></span>               |<span data-ttu-id="a9588-132">O formato de hora longa a ser usado para exibir o tempo.</span><span class="sxs-lookup"><span data-stu-id="a9588-132">The long time format to be used for displaying time.</span></span><br><br><span data-ttu-id="a9588-133">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="a9588-133">Returned by default.</span></span>|
|<span data-ttu-id="a9588-134">timeZone</span><span class="sxs-lookup"><span data-stu-id="a9588-134">timeZone</span></span>             |<span data-ttu-id="a9588-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9588-135">String</span></span>               |<span data-ttu-id="a9588-136">O fuso horário a ser usado para exibir o tempo.</span><span class="sxs-lookup"><span data-stu-id="a9588-136">The timezone to be used for displaying time.</span></span><br><br><span data-ttu-id="a9588-137">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="a9588-137">Returned by default.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9588-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9588-138">JSON representation</span></span>

<span data-ttu-id="a9588-139">A seguir está uma definição de JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9588-139">The following is a JSON definition of the resource.</span></span>

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


