---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5927c10a99b91e0130b8ceb30c33ae1fa19af3dd
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805050"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="877b0-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="877b0-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="877b0-104">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="877b0-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="877b0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="877b0-105">Properties</span></span>
| <span data-ttu-id="877b0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="877b0-106">Property</span></span>     | <span data-ttu-id="877b0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="877b0-107">Type</span></span>   |<span data-ttu-id="877b0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="877b0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="877b0-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="877b0-109">dateTime</span></span>|<span data-ttu-id="877b0-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="877b0-110">String</span></span>|<span data-ttu-id="877b0-111">Um único ponto de tempo em uma representação combinada de data e hora (`{date}T{time}`; por exemplo, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="877b0-111">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="877b0-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="877b0-112">timeZone</span></span>|<span data-ttu-id="877b0-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="877b0-113">String</span></span>|<span data-ttu-id="877b0-114">Representa um fuso horário, por exemplo, "Hora Padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="877b0-114">A string representing a specific time zone for the response, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="877b0-115">Veja a seguir os valores mais possíveis.</span><span class="sxs-lookup"><span data-stu-id="877b0-115">See below for information about the possible values.</span></span>|

<span data-ttu-id="877b0-116">Em geral, a propriedade**timeZone** _pode_ ser definida como qualquer um dos [fusos horários com suporte no Windows](https://docs.microsoft.com/pt-BR/windows-hardware/manufacture/desktop/default-time-zones), bem como [os fusos horários adicionais com suporte da API do calendário](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="877b0-116">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span> 

<span data-ttu-id="877b0-117">Ao usar **dateTimeTimeZone** em conjunto com um método (como por exemplo, [criar](../api/user-post-events.md) ou [atualizar](../api/event-update.md) um evento), anote os fusos horários que têm suporte, o que podem ser um subconjunto menor.</span><span class="sxs-lookup"><span data-stu-id="877b0-117">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="877b0-118">Fusos horários adicionais</span><span class="sxs-lookup"><span data-stu-id="877b0-118">Additional time zones</span></span>

<span data-ttu-id="877b0-119">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="877b0-119">Etc/GMT+12</span></span>

<span data-ttu-id="877b0-120">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="877b0-120">Etc/GMT+11</span></span>

<span data-ttu-id="877b0-121">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="877b0-121">Pacific/Honolulu</span></span>

<span data-ttu-id="877b0-122">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="877b0-122">America/Anchorage</span></span>

<span data-ttu-id="877b0-123">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="877b0-123">America/Santa_Isabel</span></span>

<span data-ttu-id="877b0-124">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="877b0-124">America/Los_Angeles</span></span>

<span data-ttu-id="877b0-125">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="877b0-125">America/Phoenix</span></span>

<span data-ttu-id="877b0-126">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="877b0-126">America/Chihuahua</span></span>

<span data-ttu-id="877b0-127">América/Denver</span><span class="sxs-lookup"><span data-stu-id="877b0-127">America/Denver</span></span>

<span data-ttu-id="877b0-128">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="877b0-128">America/Guatemala</span></span>

<span data-ttu-id="877b0-129">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="877b0-129">America/Chicago</span></span>

<span data-ttu-id="877b0-130">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="877b0-130">America/Mexico_City</span></span>

<span data-ttu-id="877b0-131">América/Regina</span><span class="sxs-lookup"><span data-stu-id="877b0-131">America/Regina</span></span>

<span data-ttu-id="877b0-132">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="877b0-132">America/Bogota</span></span>

<span data-ttu-id="877b0-133">América/New_York</span><span class="sxs-lookup"><span data-stu-id="877b0-133">America/New_York</span></span>

<span data-ttu-id="877b0-134">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="877b0-134">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="877b0-135">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="877b0-135">America/Caracas</span></span>

<span data-ttu-id="877b0-136">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="877b0-136">America/Asuncion</span></span>

<span data-ttu-id="877b0-137">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="877b0-137">America/Halifax</span></span>

<span data-ttu-id="877b0-138">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="877b0-138">America/Cuiaba</span></span>

<span data-ttu-id="877b0-139">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="877b0-139">America/La_Paz</span></span>

<span data-ttu-id="877b0-140">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="877b0-140">America/Santiago</span></span>

<span data-ttu-id="877b0-141">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="877b0-141">America/St_Johns</span></span>

<span data-ttu-id="877b0-142">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="877b0-142">America/Sao_Paulo</span></span>

<span data-ttu-id="877b0-143">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="877b0-143">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="877b0-144">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="877b0-144">America/Cayenne</span></span>

<span data-ttu-id="877b0-145">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="877b0-145">America/Godthab</span></span>

<span data-ttu-id="877b0-146">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="877b0-146">America/Montevideo</span></span>

<span data-ttu-id="877b0-147">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="877b0-147">America/Bahia</span></span>

<span data-ttu-id="877b0-148">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="877b0-148">Etc/GMT+2</span></span>

<span data-ttu-id="877b0-149">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="877b0-149">Atlantic/Azores</span></span>

<span data-ttu-id="877b0-150">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="877b0-150">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="877b0-151">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="877b0-151">Africa/Casablanca</span></span>

<span data-ttu-id="877b0-152">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="877b0-152">Etc/GMT</span></span>

<span data-ttu-id="877b0-153">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="877b0-153">Europe/London</span></span>

<span data-ttu-id="877b0-154">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="877b0-154">Atlantic/Reykjavik</span></span>

<span data-ttu-id="877b0-155">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="877b0-155">Europe/Berlin</span></span>

<span data-ttu-id="877b0-156">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="877b0-156">Europe/Budapest</span></span>

<span data-ttu-id="877b0-157">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="877b0-157">Europe/Paris</span></span>

<span data-ttu-id="877b0-158">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="877b0-158">Europe/Warsaw</span></span>

<span data-ttu-id="877b0-159">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="877b0-159">Africa/Lagos</span></span>

<span data-ttu-id="877b0-160">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="877b0-160">Africa/Windhoek</span></span>

<span data-ttu-id="877b0-161">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="877b0-161">Europe/Bucharest</span></span>

<span data-ttu-id="877b0-162">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="877b0-162">Asia/Beirut</span></span>

<span data-ttu-id="877b0-163">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="877b0-163">Africa/Cairo</span></span>

<span data-ttu-id="877b0-164">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="877b0-164">Asia/Damascus</span></span>

<span data-ttu-id="877b0-165">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="877b0-165">Africa/Johannesburg</span></span>

<span data-ttu-id="877b0-166">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="877b0-166">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="877b0-167">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="877b0-167">Europe/Istanbul</span></span>

<span data-ttu-id="877b0-168">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="877b0-168">Asia/Jerusalem</span></span>

<span data-ttu-id="877b0-169">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="877b0-169">Asia/Amman</span></span>

<span data-ttu-id="877b0-170">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="877b0-170">Asia/Baghdad</span></span>

<span data-ttu-id="877b0-171">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="877b0-171">Europe/Kaliningrad</span></span>

<span data-ttu-id="877b0-172">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="877b0-172">Asia/Riyadh</span></span>

<span data-ttu-id="877b0-173">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="877b0-173">Africa/Nairobi</span></span>

<span data-ttu-id="877b0-174">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="877b0-174">Asia/Tehran</span></span>

<span data-ttu-id="877b0-175">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="877b0-175">Asia/Dubai</span></span>

<span data-ttu-id="877b0-176">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="877b0-176">Asia/Baku</span></span>

<span data-ttu-id="877b0-177">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="877b0-177">Europe/Moscow</span></span>

<span data-ttu-id="877b0-178">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="877b0-178">Indian/Mauritius</span></span>

<span data-ttu-id="877b0-179">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="877b0-179">Asia/Tbilisi</span></span>

<span data-ttu-id="877b0-180">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="877b0-180">Asia/Yerevan</span></span>

<span data-ttu-id="877b0-181">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="877b0-181">Asia/Kabul</span></span>

<span data-ttu-id="877b0-182">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="877b0-182">Asia/Karachi</span></span>

<span data-ttu-id="877b0-183">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="877b0-183">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="877b0-184">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="877b0-184">Asia/Kolkata</span></span>

<span data-ttu-id="877b0-185">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="877b0-185">Asia/Colombo</span></span>

<span data-ttu-id="877b0-186">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="877b0-186">Asia/Kathmandu</span></span>

<span data-ttu-id="877b0-187">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="877b0-187">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="877b0-188">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="877b0-188">Asia/Dhaka</span></span>

<span data-ttu-id="877b0-189">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="877b0-189">Asia/Yekaterinburg</span></span>

<span data-ttu-id="877b0-190">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="877b0-190">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="877b0-191">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="877b0-191">Asia/Bangkok</span></span>

<span data-ttu-id="877b0-192">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="877b0-192">Asia/Novosibirsk</span></span>

<span data-ttu-id="877b0-193">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="877b0-193">Asia/Shanghai</span></span>

<span data-ttu-id="877b0-194">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="877b0-194">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="877b0-195">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="877b0-195">Asia/Singapore</span></span>

<span data-ttu-id="877b0-196">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="877b0-196">Australia/Perth</span></span>

<span data-ttu-id="877b0-197">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="877b0-197">Asia/Taipei</span></span>

<span data-ttu-id="877b0-198">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="877b0-198">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="877b0-199">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="877b0-199">Asia/Irkutsk</span></span>

<span data-ttu-id="877b0-200">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="877b0-200">Asia/Tokyo</span></span>

<span data-ttu-id="877b0-201">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="877b0-201">Asia/Seoul</span></span>

<span data-ttu-id="877b0-202">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="877b0-202">Australia/Adelaide</span></span>

<span data-ttu-id="877b0-203">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="877b0-203">Australia/Darwin</span></span>

<span data-ttu-id="877b0-204">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="877b0-204">Australia/Brisbane</span></span>

<span data-ttu-id="877b0-205">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="877b0-205">Australia/Sydney</span></span>

<span data-ttu-id="877b0-206">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="877b0-206">Pacific/Port_Moresby</span></span>

<span data-ttu-id="877b0-207">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="877b0-207">Australia/Hobart</span></span>

<span data-ttu-id="877b0-208">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="877b0-208">Asia/Yakutsk</span></span>

<span data-ttu-id="877b0-209">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="877b0-209">Pacific/Guadalcanal</span></span>

<span data-ttu-id="877b0-210">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="877b0-210">Asia/Vladivostok</span></span>

<span data-ttu-id="877b0-211">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="877b0-211">Pacific/Auckland</span></span>

<span data-ttu-id="877b0-212">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="877b0-212">Etc/GMT-12</span></span>

<span data-ttu-id="877b0-213">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="877b0-213">Pacific/Fiji</span></span>

<span data-ttu-id="877b0-214">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="877b0-214">Asia/Magadan</span></span>

<span data-ttu-id="877b0-215">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="877b0-215">Pacific/Tongatapu</span></span>

<span data-ttu-id="877b0-216">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="877b0-216">Pacific/Apia</span></span>

<span data-ttu-id="877b0-217">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="877b0-217">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="877b0-218">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="877b0-218">JSON representation</span></span>

<span data-ttu-id="877b0-219">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="877b0-219">Here is a JSON representation of the resource</span></span>

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
