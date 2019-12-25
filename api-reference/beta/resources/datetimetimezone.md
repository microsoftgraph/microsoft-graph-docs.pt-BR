---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Normal
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6c1bae369b71744e69753b9e7b38e5b193db00a7
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870334"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="fc834-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fc834-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc834-104">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="fc834-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="fc834-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc834-105">Properties</span></span>
| <span data-ttu-id="fc834-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc834-106">Property</span></span>     | <span data-ttu-id="fc834-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc834-107">Type</span></span>   |<span data-ttu-id="fc834-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc834-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc834-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="fc834-109">dateTime</span></span>|<span data-ttu-id="fc834-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc834-110">String</span></span>|<span data-ttu-id="fc834-111">Um único ponto de tempo em uma representação combinada de data e hora (`{date}T{time}`).</span><span class="sxs-lookup"><span data-stu-id="fc834-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="fc834-112">Por exemplo, "2019-04-16T09:00:00".</span><span class="sxs-lookup"><span data-stu-id="fc834-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="fc834-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="fc834-113">timeZone</span></span>|<span data-ttu-id="fc834-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc834-114">String</span></span>|<span data-ttu-id="fc834-115">Representa um fuso horário, por exemplo, "Hora Padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="fc834-115">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="fc834-116">Confira abaixo os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="fc834-116">See below for possible values.</span></span>|

<span data-ttu-id="fc834-117">Em geral, a propriedade**timeZone** _pode_ ser definida como qualquer um dos [fusos horários com suporte no Windows](/windows-hardware/manufacture/desktop/default-time-zones), bem como [os fusos horários adicionais com suporte da API do calendário](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="fc834-117">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="fc834-118">Ao usar **dateTimeTimeZone** em conjunto com um método (como por exemplo, [criar](../api/user-post-events.md) ou [atualizar](../api/event-update.md) um evento), anote os fusos horários que têm suporte, o que podem ser um subconjunto menor.</span><span class="sxs-lookup"><span data-stu-id="fc834-118">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="fc834-119">Fusos horários adicionais</span><span class="sxs-lookup"><span data-stu-id="fc834-119">Additional time zones</span></span>

<span data-ttu-id="fc834-120">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="fc834-120">Etc/GMT+12</span></span>

<span data-ttu-id="fc834-121">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="fc834-121">Etc/GMT+11</span></span>

<span data-ttu-id="fc834-122">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="fc834-122">Pacific/Honolulu</span></span>

<span data-ttu-id="fc834-123">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="fc834-123">America/Anchorage</span></span>

<span data-ttu-id="fc834-124">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="fc834-124">America/Santa_Isabel</span></span>

<span data-ttu-id="fc834-125">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="fc834-125">America/Los_Angeles</span></span>

<span data-ttu-id="fc834-126">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="fc834-126">America/Phoenix</span></span>

<span data-ttu-id="fc834-127">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="fc834-127">America/Chihuahua</span></span>

<span data-ttu-id="fc834-128">América/Denver</span><span class="sxs-lookup"><span data-stu-id="fc834-128">America/Denver</span></span>

<span data-ttu-id="fc834-129">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="fc834-129">America/Guatemala</span></span>

<span data-ttu-id="fc834-130">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="fc834-130">America/Chicago</span></span>

<span data-ttu-id="fc834-131">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="fc834-131">America/Mexico_City</span></span>

<span data-ttu-id="fc834-132">América/Regina</span><span class="sxs-lookup"><span data-stu-id="fc834-132">America/Regina</span></span>

<span data-ttu-id="fc834-133">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="fc834-133">America/Bogota</span></span>

<span data-ttu-id="fc834-134">América/New_York</span><span class="sxs-lookup"><span data-stu-id="fc834-134">America/New_York</span></span>

<span data-ttu-id="fc834-135">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="fc834-135">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="fc834-136">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="fc834-136">America/Caracas</span></span>

<span data-ttu-id="fc834-137">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="fc834-137">America/Asuncion</span></span>

<span data-ttu-id="fc834-138">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="fc834-138">America/Halifax</span></span>

<span data-ttu-id="fc834-139">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="fc834-139">America/Cuiaba</span></span>

<span data-ttu-id="fc834-140">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="fc834-140">America/La_Paz</span></span>

<span data-ttu-id="fc834-141">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="fc834-141">America/Santiago</span></span>

<span data-ttu-id="fc834-142">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="fc834-142">America/St_Johns</span></span>

<span data-ttu-id="fc834-143">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="fc834-143">America/Sao_Paulo</span></span>

<span data-ttu-id="fc834-144">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="fc834-144">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="fc834-145">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="fc834-145">America/Cayenne</span></span>

<span data-ttu-id="fc834-146">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="fc834-146">America/Godthab</span></span>

<span data-ttu-id="fc834-147">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="fc834-147">America/Montevideo</span></span>

<span data-ttu-id="fc834-148">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="fc834-148">America/Bahia</span></span>

<span data-ttu-id="fc834-149">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="fc834-149">Etc/GMT+2</span></span>

<span data-ttu-id="fc834-150">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="fc834-150">Atlantic/Azores</span></span>

<span data-ttu-id="fc834-151">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="fc834-151">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="fc834-152">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="fc834-152">Africa/Casablanca</span></span>

<span data-ttu-id="fc834-153">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="fc834-153">Etc/GMT</span></span>

<span data-ttu-id="fc834-154">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="fc834-154">Europe/London</span></span>

<span data-ttu-id="fc834-155">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="fc834-155">Atlantic/Reykjavik</span></span>

<span data-ttu-id="fc834-156">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="fc834-156">Europe/Berlin</span></span>

<span data-ttu-id="fc834-157">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="fc834-157">Europe/Budapest</span></span>

<span data-ttu-id="fc834-158">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="fc834-158">Europe/Paris</span></span>

<span data-ttu-id="fc834-159">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="fc834-159">Europe/Warsaw</span></span>

<span data-ttu-id="fc834-160">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="fc834-160">Africa/Lagos</span></span>

<span data-ttu-id="fc834-161">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="fc834-161">Africa/Windhoek</span></span>

<span data-ttu-id="fc834-162">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="fc834-162">Europe/Bucharest</span></span>

<span data-ttu-id="fc834-163">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="fc834-163">Asia/Beirut</span></span>

<span data-ttu-id="fc834-164">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="fc834-164">Africa/Cairo</span></span>

<span data-ttu-id="fc834-165">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="fc834-165">Asia/Damascus</span></span>

<span data-ttu-id="fc834-166">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="fc834-166">Africa/Johannesburg</span></span>

<span data-ttu-id="fc834-167">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="fc834-167">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="fc834-168">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="fc834-168">Europe/Istanbul</span></span>

<span data-ttu-id="fc834-169">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="fc834-169">Asia/Jerusalem</span></span>

<span data-ttu-id="fc834-170">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="fc834-170">Asia/Amman</span></span>

<span data-ttu-id="fc834-171">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="fc834-171">Asia/Baghdad</span></span>

<span data-ttu-id="fc834-172">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="fc834-172">Europe/Kaliningrad</span></span>

<span data-ttu-id="fc834-173">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="fc834-173">Asia/Riyadh</span></span>

<span data-ttu-id="fc834-174">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="fc834-174">Africa/Nairobi</span></span>

<span data-ttu-id="fc834-175">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="fc834-175">Asia/Tehran</span></span>

<span data-ttu-id="fc834-176">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="fc834-176">Asia/Dubai</span></span>

<span data-ttu-id="fc834-177">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="fc834-177">Asia/Baku</span></span>

<span data-ttu-id="fc834-178">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="fc834-178">Europe/Moscow</span></span>

<span data-ttu-id="fc834-179">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="fc834-179">Indian/Mauritius</span></span>

<span data-ttu-id="fc834-180">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="fc834-180">Asia/Tbilisi</span></span>

<span data-ttu-id="fc834-181">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="fc834-181">Asia/Yerevan</span></span>

<span data-ttu-id="fc834-182">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="fc834-182">Asia/Kabul</span></span>

<span data-ttu-id="fc834-183">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="fc834-183">Asia/Karachi</span></span>

<span data-ttu-id="fc834-184">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="fc834-184">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="fc834-185">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="fc834-185">Asia/Kolkata</span></span>

<span data-ttu-id="fc834-186">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="fc834-186">Asia/Colombo</span></span>

<span data-ttu-id="fc834-187">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="fc834-187">Asia/Kathmandu</span></span>

<span data-ttu-id="fc834-188">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="fc834-188">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="fc834-189">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="fc834-189">Asia/Dhaka</span></span>

<span data-ttu-id="fc834-190">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="fc834-190">Asia/Yekaterinburg</span></span>

<span data-ttu-id="fc834-191">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="fc834-191">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="fc834-192">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="fc834-192">Asia/Bangkok</span></span>

<span data-ttu-id="fc834-193">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="fc834-193">Asia/Novosibirsk</span></span>

<span data-ttu-id="fc834-194">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="fc834-194">Asia/Shanghai</span></span>

<span data-ttu-id="fc834-195">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="fc834-195">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="fc834-196">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="fc834-196">Asia/Singapore</span></span>

<span data-ttu-id="fc834-197">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="fc834-197">Australia/Perth</span></span>

<span data-ttu-id="fc834-198">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="fc834-198">Asia/Taipei</span></span>

<span data-ttu-id="fc834-199">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="fc834-199">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="fc834-200">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="fc834-200">Asia/Irkutsk</span></span>

<span data-ttu-id="fc834-201">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="fc834-201">Asia/Tokyo</span></span>

<span data-ttu-id="fc834-202">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="fc834-202">Asia/Seoul</span></span>

<span data-ttu-id="fc834-203">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="fc834-203">Australia/Adelaide</span></span>

<span data-ttu-id="fc834-204">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="fc834-204">Australia/Darwin</span></span>

<span data-ttu-id="fc834-205">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="fc834-205">Australia/Brisbane</span></span>

<span data-ttu-id="fc834-206">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="fc834-206">Australia/Sydney</span></span>

<span data-ttu-id="fc834-207">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="fc834-207">Pacific/Port_Moresby</span></span>

<span data-ttu-id="fc834-208">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="fc834-208">Australia/Hobart</span></span>

<span data-ttu-id="fc834-209">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="fc834-209">Asia/Yakutsk</span></span>

<span data-ttu-id="fc834-210">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="fc834-210">Pacific/Guadalcanal</span></span>

<span data-ttu-id="fc834-211">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="fc834-211">Asia/Vladivostok</span></span>

<span data-ttu-id="fc834-212">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="fc834-212">Pacific/Auckland</span></span>

<span data-ttu-id="fc834-213">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="fc834-213">Etc/GMT-12</span></span>

<span data-ttu-id="fc834-214">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="fc834-214">Pacific/Fiji</span></span>

<span data-ttu-id="fc834-215">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="fc834-215">Asia/Magadan</span></span>

<span data-ttu-id="fc834-216">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="fc834-216">Pacific/Tongatapu</span></span>

<span data-ttu-id="fc834-217">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="fc834-217">Pacific/Apia</span></span>

<span data-ttu-id="fc834-218">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="fc834-218">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc834-219">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc834-219">JSON representation</span></span>

<span data-ttu-id="fc834-220">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fc834-220">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dateTimeTimeZone"
}-->

```json
{
  "dateTime": "string",
  "timeZone": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
