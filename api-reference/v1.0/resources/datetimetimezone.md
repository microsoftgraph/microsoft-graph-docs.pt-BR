---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Priority
doc_type: resourcePageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: 3af4a12dad40cd6f18790ddedf99ef7e3a1770f6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449422"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="c086f-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c086f-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="c086f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c086f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c086f-105">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="c086f-105">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="c086f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c086f-106">Properties</span></span>
| <span data-ttu-id="c086f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c086f-107">Property</span></span>     | <span data-ttu-id="c086f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c086f-108">Type</span></span>   |<span data-ttu-id="c086f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c086f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c086f-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="c086f-110">dateTime</span></span>|<span data-ttu-id="c086f-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c086f-111">String</span></span>|<span data-ttu-id="c086f-112">Um único ponto de tempo em uma representação combinada de data e hora (`{date}T{time}`; por exemplo, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="c086f-112">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="c086f-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="c086f-113">timeZone</span></span>|<span data-ttu-id="c086f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c086f-114">String</span></span>|<span data-ttu-id="c086f-115">Representa um fuso horário, por exemplo, "Hora Padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="c086f-115">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="c086f-116">Veja a seguir os valores mais possíveis.</span><span class="sxs-lookup"><span data-stu-id="c086f-116">See below for more possible values.</span></span>|

<span data-ttu-id="c086f-117">Em geral, a propriedade**timeZone** _pode_ ser definida como qualquer um dos [fusos horários com suporte no Windows](/windows-hardware/manufacture/desktop/default-time-zones), bem como [os fusos horários adicionais com suporte da API do calendário](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="c086f-117">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="c086f-118">Ao usar **dateTimeTimeZone** em conjunto com um método (como por exemplo, [criar](../api/user-post-events.md) ou [atualizar](../api/event-update.md) um evento), anote os fusos horários que têm suporte, o que podem ser um subconjunto menor.</span><span class="sxs-lookup"><span data-stu-id="c086f-118">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="c086f-119">Fusos horários adicionais</span><span class="sxs-lookup"><span data-stu-id="c086f-119">Additional time zones</span></span>

<span data-ttu-id="c086f-120">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="c086f-120">Etc/GMT+12</span></span>

<span data-ttu-id="c086f-121">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="c086f-121">Etc/GMT+11</span></span>

<span data-ttu-id="c086f-122">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="c086f-122">Pacific/Honolulu</span></span>

<span data-ttu-id="c086f-123">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="c086f-123">America/Anchorage</span></span>

<span data-ttu-id="c086f-124">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="c086f-124">America/Santa_Isabel</span></span>

<span data-ttu-id="c086f-125">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="c086f-125">America/Los_Angeles</span></span>

<span data-ttu-id="c086f-126">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="c086f-126">America/Phoenix</span></span>

<span data-ttu-id="c086f-127">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="c086f-127">America/Chihuahua</span></span>

<span data-ttu-id="c086f-128">América/Denver</span><span class="sxs-lookup"><span data-stu-id="c086f-128">America/Denver</span></span>

<span data-ttu-id="c086f-129">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="c086f-129">America/Guatemala</span></span>

<span data-ttu-id="c086f-130">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="c086f-130">America/Chicago</span></span>

<span data-ttu-id="c086f-131">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="c086f-131">America/Mexico_City</span></span>

<span data-ttu-id="c086f-132">América/Regina</span><span class="sxs-lookup"><span data-stu-id="c086f-132">America/Regina</span></span>

<span data-ttu-id="c086f-133">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="c086f-133">America/Bogota</span></span>

<span data-ttu-id="c086f-134">América/New_York</span><span class="sxs-lookup"><span data-stu-id="c086f-134">America/New_York</span></span>

<span data-ttu-id="c086f-135">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="c086f-135">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="c086f-136">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="c086f-136">America/Caracas</span></span>

<span data-ttu-id="c086f-137">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="c086f-137">America/Asuncion</span></span>

<span data-ttu-id="c086f-138">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="c086f-138">America/Halifax</span></span>

<span data-ttu-id="c086f-139">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="c086f-139">America/Cuiaba</span></span>

<span data-ttu-id="c086f-140">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="c086f-140">America/La_Paz</span></span>

<span data-ttu-id="c086f-141">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="c086f-141">America/Santiago</span></span>

<span data-ttu-id="c086f-142">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="c086f-142">America/St_Johns</span></span>

<span data-ttu-id="c086f-143">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="c086f-143">America/Sao_Paulo</span></span>

<span data-ttu-id="c086f-144">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="c086f-144">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="c086f-145">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="c086f-145">America/Cayenne</span></span>

<span data-ttu-id="c086f-146">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="c086f-146">America/Godthab</span></span>

<span data-ttu-id="c086f-147">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="c086f-147">America/Montevideo</span></span>

<span data-ttu-id="c086f-148">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="c086f-148">America/Bahia</span></span>

<span data-ttu-id="c086f-149">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="c086f-149">Etc/GMT+2</span></span>

<span data-ttu-id="c086f-150">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="c086f-150">Atlantic/Azores</span></span>

<span data-ttu-id="c086f-151">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="c086f-151">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="c086f-152">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="c086f-152">Africa/Casablanca</span></span>

<span data-ttu-id="c086f-153">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="c086f-153">Etc/GMT</span></span>

<span data-ttu-id="c086f-154">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="c086f-154">Europe/London</span></span>

<span data-ttu-id="c086f-155">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="c086f-155">Atlantic/Reykjavik</span></span>

<span data-ttu-id="c086f-156">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="c086f-156">Europe/Berlin</span></span>

<span data-ttu-id="c086f-157">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="c086f-157">Europe/Budapest</span></span>

<span data-ttu-id="c086f-158">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="c086f-158">Europe/Paris</span></span>

<span data-ttu-id="c086f-159">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="c086f-159">Europe/Warsaw</span></span>

<span data-ttu-id="c086f-160">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="c086f-160">Africa/Lagos</span></span>

<span data-ttu-id="c086f-161">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="c086f-161">Africa/Windhoek</span></span>

<span data-ttu-id="c086f-162">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="c086f-162">Europe/Bucharest</span></span>

<span data-ttu-id="c086f-163">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="c086f-163">Asia/Beirut</span></span>

<span data-ttu-id="c086f-164">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="c086f-164">Africa/Cairo</span></span>

<span data-ttu-id="c086f-165">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="c086f-165">Asia/Damascus</span></span>

<span data-ttu-id="c086f-166">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="c086f-166">Africa/Johannesburg</span></span>

<span data-ttu-id="c086f-167">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="c086f-167">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="c086f-168">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="c086f-168">Europe/Istanbul</span></span>

<span data-ttu-id="c086f-169">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="c086f-169">Asia/Jerusalem</span></span>

<span data-ttu-id="c086f-170">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="c086f-170">Asia/Amman</span></span>

<span data-ttu-id="c086f-171">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="c086f-171">Asia/Baghdad</span></span>

<span data-ttu-id="c086f-172">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="c086f-172">Europe/Kaliningrad</span></span>

<span data-ttu-id="c086f-173">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="c086f-173">Asia/Riyadh</span></span>

<span data-ttu-id="c086f-174">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="c086f-174">Africa/Nairobi</span></span>

<span data-ttu-id="c086f-175">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="c086f-175">Asia/Tehran</span></span>

<span data-ttu-id="c086f-176">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="c086f-176">Asia/Dubai</span></span>

<span data-ttu-id="c086f-177">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="c086f-177">Asia/Baku</span></span>

<span data-ttu-id="c086f-178">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="c086f-178">Europe/Moscow</span></span>

<span data-ttu-id="c086f-179">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="c086f-179">Indian/Mauritius</span></span>

<span data-ttu-id="c086f-180">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="c086f-180">Asia/Tbilisi</span></span>

<span data-ttu-id="c086f-181">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="c086f-181">Asia/Yerevan</span></span>

<span data-ttu-id="c086f-182">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="c086f-182">Asia/Kabul</span></span>

<span data-ttu-id="c086f-183">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="c086f-183">Asia/Karachi</span></span>

<span data-ttu-id="c086f-184">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="c086f-184">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="c086f-185">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="c086f-185">Asia/Kolkata</span></span>

<span data-ttu-id="c086f-186">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="c086f-186">Asia/Colombo</span></span>

<span data-ttu-id="c086f-187">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="c086f-187">Asia/Kathmandu</span></span>

<span data-ttu-id="c086f-188">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="c086f-188">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="c086f-189">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="c086f-189">Asia/Dhaka</span></span>

<span data-ttu-id="c086f-190">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="c086f-190">Asia/Yekaterinburg</span></span>

<span data-ttu-id="c086f-191">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="c086f-191">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="c086f-192">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="c086f-192">Asia/Bangkok</span></span>

<span data-ttu-id="c086f-193">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="c086f-193">Asia/Novosibirsk</span></span>

<span data-ttu-id="c086f-194">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="c086f-194">Asia/Shanghai</span></span>

<span data-ttu-id="c086f-195">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="c086f-195">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="c086f-196">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="c086f-196">Asia/Singapore</span></span>

<span data-ttu-id="c086f-197">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="c086f-197">Australia/Perth</span></span>

<span data-ttu-id="c086f-198">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="c086f-198">Asia/Taipei</span></span>

<span data-ttu-id="c086f-199">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="c086f-199">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="c086f-200">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="c086f-200">Asia/Irkutsk</span></span>

<span data-ttu-id="c086f-201">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="c086f-201">Asia/Tokyo</span></span>

<span data-ttu-id="c086f-202">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="c086f-202">Asia/Seoul</span></span>

<span data-ttu-id="c086f-203">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="c086f-203">Australia/Adelaide</span></span>

<span data-ttu-id="c086f-204">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="c086f-204">Australia/Darwin</span></span>

<span data-ttu-id="c086f-205">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="c086f-205">Australia/Brisbane</span></span>

<span data-ttu-id="c086f-206">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="c086f-206">Australia/Sydney</span></span>

<span data-ttu-id="c086f-207">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="c086f-207">Pacific/Port_Moresby</span></span>

<span data-ttu-id="c086f-208">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="c086f-208">Australia/Hobart</span></span>

<span data-ttu-id="c086f-209">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="c086f-209">Asia/Yakutsk</span></span>

<span data-ttu-id="c086f-210">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="c086f-210">Pacific/Guadalcanal</span></span>

<span data-ttu-id="c086f-211">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="c086f-211">Asia/Vladivostok</span></span>

<span data-ttu-id="c086f-212">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="c086f-212">Pacific/Auckland</span></span>

<span data-ttu-id="c086f-213">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="c086f-213">Etc/GMT-12</span></span>

<span data-ttu-id="c086f-214">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="c086f-214">Pacific/Fiji</span></span>

<span data-ttu-id="c086f-215">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="c086f-215">Asia/Magadan</span></span>

<span data-ttu-id="c086f-216">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="c086f-216">Pacific/Tongatapu</span></span>

<span data-ttu-id="c086f-217">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="c086f-217">Pacific/Apia</span></span>

<span data-ttu-id="c086f-218">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="c086f-218">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="c086f-219">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c086f-219">JSON representation</span></span>

<span data-ttu-id="c086f-220">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c086f-220">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
