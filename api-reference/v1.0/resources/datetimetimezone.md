---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Priority
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 429f9b7d273b83b78580650ee323ea35343cdfaf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869833"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="bf730-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bf730-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="bf730-104">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="bf730-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="bf730-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf730-105">Properties</span></span>
| <span data-ttu-id="bf730-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf730-106">Property</span></span>     | <span data-ttu-id="bf730-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf730-107">Type</span></span>   |<span data-ttu-id="bf730-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf730-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf730-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="bf730-109">dateTime</span></span>|<span data-ttu-id="bf730-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf730-110">String</span></span>|<span data-ttu-id="bf730-111">Um único ponto de tempo em uma representação combinada de data e hora (`{date}T{time}`; por exemplo, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="bf730-111">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="bf730-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="bf730-112">timeZone</span></span>|<span data-ttu-id="bf730-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf730-113">String</span></span>|<span data-ttu-id="bf730-114">Representa um fuso horário, por exemplo, "Hora Padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="bf730-114">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="bf730-115">Veja a seguir os valores mais possíveis.</span><span class="sxs-lookup"><span data-stu-id="bf730-115">See below for more possible values.</span></span>|

<span data-ttu-id="bf730-116">Em geral, a propriedade**timeZone** _pode_ ser definida como qualquer um dos [fusos horários com suporte no Windows](/windows-hardware/manufacture/desktop/default-time-zones), bem como [os fusos horários adicionais com suporte da API do calendário](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="bf730-116">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="bf730-117">Ao usar **dateTimeTimeZone** em conjunto com um método (como por exemplo, [criar](../api/user-post-events.md) ou [atualizar](../api/event-update.md) um evento), anote os fusos horários que têm suporte, o que podem ser um subconjunto menor.</span><span class="sxs-lookup"><span data-stu-id="bf730-117">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="bf730-118">Fusos horários adicionais</span><span class="sxs-lookup"><span data-stu-id="bf730-118">Additional time zones</span></span>

<span data-ttu-id="bf730-119">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="bf730-119">Etc/GMT+12</span></span>

<span data-ttu-id="bf730-120">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="bf730-120">Etc/GMT+11</span></span>

<span data-ttu-id="bf730-121">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="bf730-121">Pacific/Honolulu</span></span>

<span data-ttu-id="bf730-122">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="bf730-122">America/Anchorage</span></span>

<span data-ttu-id="bf730-123">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="bf730-123">America/Santa_Isabel</span></span>

<span data-ttu-id="bf730-124">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="bf730-124">America/Los_Angeles</span></span>

<span data-ttu-id="bf730-125">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="bf730-125">America/Phoenix</span></span>

<span data-ttu-id="bf730-126">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="bf730-126">America/Chihuahua</span></span>

<span data-ttu-id="bf730-127">América/Denver</span><span class="sxs-lookup"><span data-stu-id="bf730-127">America/Denver</span></span>

<span data-ttu-id="bf730-128">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="bf730-128">America/Guatemala</span></span>

<span data-ttu-id="bf730-129">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="bf730-129">America/Chicago</span></span>

<span data-ttu-id="bf730-130">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="bf730-130">America/Mexico_City</span></span>

<span data-ttu-id="bf730-131">América/Regina</span><span class="sxs-lookup"><span data-stu-id="bf730-131">America/Regina</span></span>

<span data-ttu-id="bf730-132">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="bf730-132">America/Bogota</span></span>

<span data-ttu-id="bf730-133">América/New_York</span><span class="sxs-lookup"><span data-stu-id="bf730-133">America/New_York</span></span>

<span data-ttu-id="bf730-134">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="bf730-134">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="bf730-135">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="bf730-135">America/Caracas</span></span>

<span data-ttu-id="bf730-136">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="bf730-136">America/Asuncion</span></span>

<span data-ttu-id="bf730-137">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="bf730-137">America/Halifax</span></span>

<span data-ttu-id="bf730-138">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="bf730-138">America/Cuiaba</span></span>

<span data-ttu-id="bf730-139">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="bf730-139">America/La_Paz</span></span>

<span data-ttu-id="bf730-140">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="bf730-140">America/Santiago</span></span>

<span data-ttu-id="bf730-141">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="bf730-141">America/St_Johns</span></span>

<span data-ttu-id="bf730-142">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="bf730-142">America/Sao_Paulo</span></span>

<span data-ttu-id="bf730-143">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="bf730-143">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="bf730-144">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="bf730-144">America/Cayenne</span></span>

<span data-ttu-id="bf730-145">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="bf730-145">America/Godthab</span></span>

<span data-ttu-id="bf730-146">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="bf730-146">America/Montevideo</span></span>

<span data-ttu-id="bf730-147">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="bf730-147">America/Bahia</span></span>

<span data-ttu-id="bf730-148">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="bf730-148">Etc/GMT+2</span></span>

<span data-ttu-id="bf730-149">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="bf730-149">Atlantic/Azores</span></span>

<span data-ttu-id="bf730-150">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="bf730-150">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="bf730-151">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="bf730-151">Africa/Casablanca</span></span>

<span data-ttu-id="bf730-152">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="bf730-152">Etc/GMT</span></span>

<span data-ttu-id="bf730-153">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="bf730-153">Europe/London</span></span>

<span data-ttu-id="bf730-154">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="bf730-154">Atlantic/Reykjavik</span></span>

<span data-ttu-id="bf730-155">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="bf730-155">Europe/Berlin</span></span>

<span data-ttu-id="bf730-156">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="bf730-156">Europe/Budapest</span></span>

<span data-ttu-id="bf730-157">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="bf730-157">Europe/Paris</span></span>

<span data-ttu-id="bf730-158">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="bf730-158">Europe/Warsaw</span></span>

<span data-ttu-id="bf730-159">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="bf730-159">Africa/Lagos</span></span>

<span data-ttu-id="bf730-160">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="bf730-160">Africa/Windhoek</span></span>

<span data-ttu-id="bf730-161">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="bf730-161">Europe/Bucharest</span></span>

<span data-ttu-id="bf730-162">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="bf730-162">Asia/Beirut</span></span>

<span data-ttu-id="bf730-163">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="bf730-163">Africa/Cairo</span></span>

<span data-ttu-id="bf730-164">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="bf730-164">Asia/Damascus</span></span>

<span data-ttu-id="bf730-165">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="bf730-165">Africa/Johannesburg</span></span>

<span data-ttu-id="bf730-166">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="bf730-166">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="bf730-167">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="bf730-167">Europe/Istanbul</span></span>

<span data-ttu-id="bf730-168">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="bf730-168">Asia/Jerusalem</span></span>

<span data-ttu-id="bf730-169">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="bf730-169">Asia/Amman</span></span>

<span data-ttu-id="bf730-170">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="bf730-170">Asia/Baghdad</span></span>

<span data-ttu-id="bf730-171">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="bf730-171">Europe/Kaliningrad</span></span>

<span data-ttu-id="bf730-172">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="bf730-172">Asia/Riyadh</span></span>

<span data-ttu-id="bf730-173">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="bf730-173">Africa/Nairobi</span></span>

<span data-ttu-id="bf730-174">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="bf730-174">Asia/Tehran</span></span>

<span data-ttu-id="bf730-175">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="bf730-175">Asia/Dubai</span></span>

<span data-ttu-id="bf730-176">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="bf730-176">Asia/Baku</span></span>

<span data-ttu-id="bf730-177">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="bf730-177">Europe/Moscow</span></span>

<span data-ttu-id="bf730-178">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="bf730-178">Indian/Mauritius</span></span>

<span data-ttu-id="bf730-179">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="bf730-179">Asia/Tbilisi</span></span>

<span data-ttu-id="bf730-180">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="bf730-180">Asia/Yerevan</span></span>

<span data-ttu-id="bf730-181">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="bf730-181">Asia/Kabul</span></span>

<span data-ttu-id="bf730-182">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="bf730-182">Asia/Karachi</span></span>

<span data-ttu-id="bf730-183">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="bf730-183">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="bf730-184">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="bf730-184">Asia/Kolkata</span></span>

<span data-ttu-id="bf730-185">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="bf730-185">Asia/Colombo</span></span>

<span data-ttu-id="bf730-186">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="bf730-186">Asia/Kathmandu</span></span>

<span data-ttu-id="bf730-187">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="bf730-187">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="bf730-188">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="bf730-188">Asia/Dhaka</span></span>

<span data-ttu-id="bf730-189">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="bf730-189">Asia/Yekaterinburg</span></span>

<span data-ttu-id="bf730-190">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="bf730-190">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="bf730-191">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="bf730-191">Asia/Bangkok</span></span>

<span data-ttu-id="bf730-192">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="bf730-192">Asia/Novosibirsk</span></span>

<span data-ttu-id="bf730-193">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="bf730-193">Asia/Shanghai</span></span>

<span data-ttu-id="bf730-194">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="bf730-194">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="bf730-195">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="bf730-195">Asia/Singapore</span></span>

<span data-ttu-id="bf730-196">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="bf730-196">Australia/Perth</span></span>

<span data-ttu-id="bf730-197">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="bf730-197">Asia/Taipei</span></span>

<span data-ttu-id="bf730-198">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="bf730-198">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="bf730-199">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="bf730-199">Asia/Irkutsk</span></span>

<span data-ttu-id="bf730-200">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="bf730-200">Asia/Tokyo</span></span>

<span data-ttu-id="bf730-201">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="bf730-201">Asia/Seoul</span></span>

<span data-ttu-id="bf730-202">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="bf730-202">Australia/Adelaide</span></span>

<span data-ttu-id="bf730-203">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="bf730-203">Australia/Darwin</span></span>

<span data-ttu-id="bf730-204">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="bf730-204">Australia/Brisbane</span></span>

<span data-ttu-id="bf730-205">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="bf730-205">Australia/Sydney</span></span>

<span data-ttu-id="bf730-206">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="bf730-206">Pacific/Port_Moresby</span></span>

<span data-ttu-id="bf730-207">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="bf730-207">Australia/Hobart</span></span>

<span data-ttu-id="bf730-208">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="bf730-208">Asia/Yakutsk</span></span>

<span data-ttu-id="bf730-209">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="bf730-209">Pacific/Guadalcanal</span></span>

<span data-ttu-id="bf730-210">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="bf730-210">Asia/Vladivostok</span></span>

<span data-ttu-id="bf730-211">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="bf730-211">Pacific/Auckland</span></span>

<span data-ttu-id="bf730-212">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="bf730-212">Etc/GMT-12</span></span>

<span data-ttu-id="bf730-213">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="bf730-213">Pacific/Fiji</span></span>

<span data-ttu-id="bf730-214">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="bf730-214">Asia/Magadan</span></span>

<span data-ttu-id="bf730-215">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="bf730-215">Pacific/Tongatapu</span></span>

<span data-ttu-id="bf730-216">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="bf730-216">Pacific/Apia</span></span>

<span data-ttu-id="bf730-217">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="bf730-217">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf730-218">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf730-218">JSON representation</span></span>

<span data-ttu-id="bf730-219">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bf730-219">Here is a JSON representation of the resource</span></span>

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
