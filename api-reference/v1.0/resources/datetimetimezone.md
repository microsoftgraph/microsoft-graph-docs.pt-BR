---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Priority
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: cd60bf4416ae02b74d9c49fdb69c93ffa19c7c66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531716"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="2429d-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2429d-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="2429d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2429d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2429d-105">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="2429d-105">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="2429d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2429d-106">Properties</span></span>
| <span data-ttu-id="2429d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2429d-107">Property</span></span>     | <span data-ttu-id="2429d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2429d-108">Type</span></span>   |<span data-ttu-id="2429d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2429d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2429d-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="2429d-110">dateTime</span></span>|<span data-ttu-id="2429d-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2429d-111">String</span></span>|<span data-ttu-id="2429d-112">Um único ponto de tempo em uma representação combinada de data e hora (`{date}T{time}`; por exemplo, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="2429d-112">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="2429d-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="2429d-113">timeZone</span></span>|<span data-ttu-id="2429d-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2429d-114">String</span></span>|<span data-ttu-id="2429d-115">Representa um fuso horário, por exemplo, "Hora Padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="2429d-115">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="2429d-116">Veja a seguir os valores mais possíveis.</span><span class="sxs-lookup"><span data-stu-id="2429d-116">See below for more possible values.</span></span>|

<span data-ttu-id="2429d-117">Em geral, a propriedade**timeZone** _pode_ ser definida como qualquer um dos [fusos horários com suporte no Windows](/windows-hardware/manufacture/desktop/default-time-zones), bem como [os fusos horários adicionais com suporte da API do calendário](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="2429d-117">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="2429d-118">Ao usar **dateTimeTimeZone** em conjunto com um método (como por exemplo, [criar](../api/user-post-events.md) ou [atualizar](../api/event-update.md) um evento), anote os fusos horários que têm suporte, o que podem ser um subconjunto menor.</span><span class="sxs-lookup"><span data-stu-id="2429d-118">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="2429d-119">Fusos horários adicionais</span><span class="sxs-lookup"><span data-stu-id="2429d-119">Additional time zones</span></span>

<span data-ttu-id="2429d-120">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="2429d-120">Etc/GMT+12</span></span>

<span data-ttu-id="2429d-121">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="2429d-121">Etc/GMT+11</span></span>

<span data-ttu-id="2429d-122">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="2429d-122">Pacific/Honolulu</span></span>

<span data-ttu-id="2429d-123">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="2429d-123">America/Anchorage</span></span>

<span data-ttu-id="2429d-124">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="2429d-124">America/Santa_Isabel</span></span>

<span data-ttu-id="2429d-125">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="2429d-125">America/Los_Angeles</span></span>

<span data-ttu-id="2429d-126">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="2429d-126">America/Phoenix</span></span>

<span data-ttu-id="2429d-127">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="2429d-127">America/Chihuahua</span></span>

<span data-ttu-id="2429d-128">América/Denver</span><span class="sxs-lookup"><span data-stu-id="2429d-128">America/Denver</span></span>

<span data-ttu-id="2429d-129">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="2429d-129">America/Guatemala</span></span>

<span data-ttu-id="2429d-130">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="2429d-130">America/Chicago</span></span>

<span data-ttu-id="2429d-131">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="2429d-131">America/Mexico_City</span></span>

<span data-ttu-id="2429d-132">América/Regina</span><span class="sxs-lookup"><span data-stu-id="2429d-132">America/Regina</span></span>

<span data-ttu-id="2429d-133">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="2429d-133">America/Bogota</span></span>

<span data-ttu-id="2429d-134">América/New_York</span><span class="sxs-lookup"><span data-stu-id="2429d-134">America/New_York</span></span>

<span data-ttu-id="2429d-135">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="2429d-135">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="2429d-136">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="2429d-136">America/Caracas</span></span>

<span data-ttu-id="2429d-137">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="2429d-137">America/Asuncion</span></span>

<span data-ttu-id="2429d-138">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="2429d-138">America/Halifax</span></span>

<span data-ttu-id="2429d-139">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="2429d-139">America/Cuiaba</span></span>

<span data-ttu-id="2429d-140">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="2429d-140">America/La_Paz</span></span>

<span data-ttu-id="2429d-141">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="2429d-141">America/Santiago</span></span>

<span data-ttu-id="2429d-142">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="2429d-142">America/St_Johns</span></span>

<span data-ttu-id="2429d-143">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="2429d-143">America/Sao_Paulo</span></span>

<span data-ttu-id="2429d-144">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="2429d-144">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="2429d-145">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="2429d-145">America/Cayenne</span></span>

<span data-ttu-id="2429d-146">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="2429d-146">America/Godthab</span></span>

<span data-ttu-id="2429d-147">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="2429d-147">America/Montevideo</span></span>

<span data-ttu-id="2429d-148">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="2429d-148">America/Bahia</span></span>

<span data-ttu-id="2429d-149">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="2429d-149">Etc/GMT+2</span></span>

<span data-ttu-id="2429d-150">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="2429d-150">Atlantic/Azores</span></span>

<span data-ttu-id="2429d-151">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="2429d-151">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="2429d-152">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="2429d-152">Africa/Casablanca</span></span>

<span data-ttu-id="2429d-153">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="2429d-153">Etc/GMT</span></span>

<span data-ttu-id="2429d-154">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="2429d-154">Europe/London</span></span>

<span data-ttu-id="2429d-155">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="2429d-155">Atlantic/Reykjavik</span></span>

<span data-ttu-id="2429d-156">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="2429d-156">Europe/Berlin</span></span>

<span data-ttu-id="2429d-157">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="2429d-157">Europe/Budapest</span></span>

<span data-ttu-id="2429d-158">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="2429d-158">Europe/Paris</span></span>

<span data-ttu-id="2429d-159">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="2429d-159">Europe/Warsaw</span></span>

<span data-ttu-id="2429d-160">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="2429d-160">Africa/Lagos</span></span>

<span data-ttu-id="2429d-161">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="2429d-161">Africa/Windhoek</span></span>

<span data-ttu-id="2429d-162">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="2429d-162">Europe/Bucharest</span></span>

<span data-ttu-id="2429d-163">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="2429d-163">Asia/Beirut</span></span>

<span data-ttu-id="2429d-164">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="2429d-164">Africa/Cairo</span></span>

<span data-ttu-id="2429d-165">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="2429d-165">Asia/Damascus</span></span>

<span data-ttu-id="2429d-166">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="2429d-166">Africa/Johannesburg</span></span>

<span data-ttu-id="2429d-167">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="2429d-167">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="2429d-168">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="2429d-168">Europe/Istanbul</span></span>

<span data-ttu-id="2429d-169">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="2429d-169">Asia/Jerusalem</span></span>

<span data-ttu-id="2429d-170">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="2429d-170">Asia/Amman</span></span>

<span data-ttu-id="2429d-171">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="2429d-171">Asia/Baghdad</span></span>

<span data-ttu-id="2429d-172">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="2429d-172">Europe/Kaliningrad</span></span>

<span data-ttu-id="2429d-173">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="2429d-173">Asia/Riyadh</span></span>

<span data-ttu-id="2429d-174">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="2429d-174">Africa/Nairobi</span></span>

<span data-ttu-id="2429d-175">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="2429d-175">Asia/Tehran</span></span>

<span data-ttu-id="2429d-176">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="2429d-176">Asia/Dubai</span></span>

<span data-ttu-id="2429d-177">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="2429d-177">Asia/Baku</span></span>

<span data-ttu-id="2429d-178">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="2429d-178">Europe/Moscow</span></span>

<span data-ttu-id="2429d-179">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="2429d-179">Indian/Mauritius</span></span>

<span data-ttu-id="2429d-180">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="2429d-180">Asia/Tbilisi</span></span>

<span data-ttu-id="2429d-181">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="2429d-181">Asia/Yerevan</span></span>

<span data-ttu-id="2429d-182">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="2429d-182">Asia/Kabul</span></span>

<span data-ttu-id="2429d-183">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="2429d-183">Asia/Karachi</span></span>

<span data-ttu-id="2429d-184">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="2429d-184">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="2429d-185">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="2429d-185">Asia/Kolkata</span></span>

<span data-ttu-id="2429d-186">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="2429d-186">Asia/Colombo</span></span>

<span data-ttu-id="2429d-187">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="2429d-187">Asia/Kathmandu</span></span>

<span data-ttu-id="2429d-188">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="2429d-188">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="2429d-189">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="2429d-189">Asia/Dhaka</span></span>

<span data-ttu-id="2429d-190">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="2429d-190">Asia/Yekaterinburg</span></span>

<span data-ttu-id="2429d-191">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="2429d-191">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="2429d-192">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="2429d-192">Asia/Bangkok</span></span>

<span data-ttu-id="2429d-193">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="2429d-193">Asia/Novosibirsk</span></span>

<span data-ttu-id="2429d-194">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="2429d-194">Asia/Shanghai</span></span>

<span data-ttu-id="2429d-195">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="2429d-195">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="2429d-196">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="2429d-196">Asia/Singapore</span></span>

<span data-ttu-id="2429d-197">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="2429d-197">Australia/Perth</span></span>

<span data-ttu-id="2429d-198">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="2429d-198">Asia/Taipei</span></span>

<span data-ttu-id="2429d-199">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="2429d-199">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="2429d-200">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="2429d-200">Asia/Irkutsk</span></span>

<span data-ttu-id="2429d-201">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="2429d-201">Asia/Tokyo</span></span>

<span data-ttu-id="2429d-202">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="2429d-202">Asia/Seoul</span></span>

<span data-ttu-id="2429d-203">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="2429d-203">Australia/Adelaide</span></span>

<span data-ttu-id="2429d-204">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="2429d-204">Australia/Darwin</span></span>

<span data-ttu-id="2429d-205">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="2429d-205">Australia/Brisbane</span></span>

<span data-ttu-id="2429d-206">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="2429d-206">Australia/Sydney</span></span>

<span data-ttu-id="2429d-207">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="2429d-207">Pacific/Port_Moresby</span></span>

<span data-ttu-id="2429d-208">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="2429d-208">Australia/Hobart</span></span>

<span data-ttu-id="2429d-209">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="2429d-209">Asia/Yakutsk</span></span>

<span data-ttu-id="2429d-210">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="2429d-210">Pacific/Guadalcanal</span></span>

<span data-ttu-id="2429d-211">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="2429d-211">Asia/Vladivostok</span></span>

<span data-ttu-id="2429d-212">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="2429d-212">Pacific/Auckland</span></span>

<span data-ttu-id="2429d-213">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="2429d-213">Etc/GMT-12</span></span>

<span data-ttu-id="2429d-214">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="2429d-214">Pacific/Fiji</span></span>

<span data-ttu-id="2429d-215">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="2429d-215">Asia/Magadan</span></span>

<span data-ttu-id="2429d-216">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="2429d-216">Pacific/Tongatapu</span></span>

<span data-ttu-id="2429d-217">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="2429d-217">Pacific/Apia</span></span>

<span data-ttu-id="2429d-218">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="2429d-218">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="2429d-219">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2429d-219">JSON representation</span></span>

<span data-ttu-id="2429d-220">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2429d-220">Here is a JSON representation of the resource</span></span>

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
