---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Priority
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e265e6de20491e44ba7756ffd02f4dc4d09d0b31
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029537"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="43081-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="43081-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="43081-104">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="43081-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="43081-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43081-105">Properties</span></span>
| <span data-ttu-id="43081-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43081-106">Property</span></span>     | <span data-ttu-id="43081-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="43081-107">Type</span></span>   |<span data-ttu-id="43081-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="43081-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43081-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="43081-109">dateTime</span></span>|<span data-ttu-id="43081-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43081-110">String</span></span>|<span data-ttu-id="43081-111">Um único ponto de tempo em uma representação combinada de data e hora (`{date}T{time}`; por exemplo, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="43081-111">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="43081-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="43081-112">timeZone</span></span>|<span data-ttu-id="43081-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43081-113">String</span></span>|<span data-ttu-id="43081-114">Representa um fuso horário, por exemplo, "Hora Padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="43081-114">A string representing a specific time zone for the response, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="43081-115">Veja a seguir os valores mais possíveis.</span><span class="sxs-lookup"><span data-stu-id="43081-115">See below for information about the possible values.</span></span>|

<span data-ttu-id="43081-116">Em geral, a propriedade**timeZone** _pode_ ser definida como qualquer um dos [fusos horários com suporte no Windows](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/default-time-zones), bem como [os fusos horários adicionais com suporte da API do calendário](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="43081-116">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span> 

<span data-ttu-id="43081-117">Ao usar **dateTimeTimeZone** em conjunto com um método (como por exemplo, [criar](../api/user-post-events.md) ou [atualizar](../api/event-update.md) um evento), anote os fusos horários que têm suporte, o que podem ser um subconjunto menor.</span><span class="sxs-lookup"><span data-stu-id="43081-117">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="43081-118">Fusos horários adicionais</span><span class="sxs-lookup"><span data-stu-id="43081-118">Additional time zones</span></span>

<span data-ttu-id="43081-119">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="43081-119">Etc/GMT+12</span></span>

<span data-ttu-id="43081-120">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="43081-120">Etc/GMT+11</span></span>

<span data-ttu-id="43081-121">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="43081-121">Pacific/Honolulu</span></span>

<span data-ttu-id="43081-122">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="43081-122">America/Anchorage</span></span>

<span data-ttu-id="43081-123">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="43081-123">America/Santa_Isabel</span></span>

<span data-ttu-id="43081-124">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="43081-124">America/Los_Angeles</span></span>

<span data-ttu-id="43081-125">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="43081-125">America/Phoenix</span></span>

<span data-ttu-id="43081-126">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="43081-126">America/Chihuahua</span></span>

<span data-ttu-id="43081-127">América/Denver</span><span class="sxs-lookup"><span data-stu-id="43081-127">America/Denver</span></span>

<span data-ttu-id="43081-128">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="43081-128">America/Guatemala</span></span>

<span data-ttu-id="43081-129">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="43081-129">America/Chicago</span></span>

<span data-ttu-id="43081-130">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="43081-130">America/Mexico_City</span></span>

<span data-ttu-id="43081-131">América/Regina</span><span class="sxs-lookup"><span data-stu-id="43081-131">America/Regina</span></span>

<span data-ttu-id="43081-132">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="43081-132">America/Bogota</span></span>

<span data-ttu-id="43081-133">América/New_York</span><span class="sxs-lookup"><span data-stu-id="43081-133">America/New_York</span></span>

<span data-ttu-id="43081-134">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="43081-134">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="43081-135">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="43081-135">America/Caracas</span></span>

<span data-ttu-id="43081-136">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="43081-136">America/Asuncion</span></span>

<span data-ttu-id="43081-137">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="43081-137">America/Halifax</span></span>

<span data-ttu-id="43081-138">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="43081-138">America/Cuiaba</span></span>

<span data-ttu-id="43081-139">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="43081-139">America/La_Paz</span></span>

<span data-ttu-id="43081-140">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="43081-140">America/Santiago</span></span>

<span data-ttu-id="43081-141">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="43081-141">America/St_Johns</span></span>

<span data-ttu-id="43081-142">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="43081-142">America/Sao_Paulo</span></span>

<span data-ttu-id="43081-143">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="43081-143">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="43081-144">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="43081-144">America/Cayenne</span></span>

<span data-ttu-id="43081-145">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="43081-145">America/Godthab</span></span>

<span data-ttu-id="43081-146">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="43081-146">America/Montevideo</span></span>

<span data-ttu-id="43081-147">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="43081-147">America/Bahia</span></span>

<span data-ttu-id="43081-148">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="43081-148">Etc/GMT+2</span></span>

<span data-ttu-id="43081-149">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="43081-149">Atlantic/Azores</span></span>

<span data-ttu-id="43081-150">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="43081-150">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="43081-151">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="43081-151">Africa/Casablanca</span></span>

<span data-ttu-id="43081-152">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="43081-152">Etc/GMT</span></span>

<span data-ttu-id="43081-153">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="43081-153">Europe/London</span></span>

<span data-ttu-id="43081-154">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="43081-154">Atlantic/Reykjavik</span></span>

<span data-ttu-id="43081-155">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="43081-155">Europe/Berlin</span></span>

<span data-ttu-id="43081-156">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="43081-156">Europe/Budapest</span></span>

<span data-ttu-id="43081-157">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="43081-157">Europe/Paris</span></span>

<span data-ttu-id="43081-158">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="43081-158">Europe/Warsaw</span></span>

<span data-ttu-id="43081-159">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="43081-159">Africa/Lagos</span></span>

<span data-ttu-id="43081-160">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="43081-160">Africa/Windhoek</span></span>

<span data-ttu-id="43081-161">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="43081-161">Europe/Bucharest</span></span>

<span data-ttu-id="43081-162">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="43081-162">Asia/Beirut</span></span>

<span data-ttu-id="43081-163">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="43081-163">Africa/Cairo</span></span>

<span data-ttu-id="43081-164">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="43081-164">Asia/Damascus</span></span>

<span data-ttu-id="43081-165">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="43081-165">Africa/Johannesburg</span></span>

<span data-ttu-id="43081-166">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="43081-166">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="43081-167">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="43081-167">Europe/Istanbul</span></span>

<span data-ttu-id="43081-168">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="43081-168">Asia/Jerusalem</span></span>

<span data-ttu-id="43081-169">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="43081-169">Asia/Amman</span></span>

<span data-ttu-id="43081-170">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="43081-170">Asia/Baghdad</span></span>

<span data-ttu-id="43081-171">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="43081-171">Europe/Kaliningrad</span></span>

<span data-ttu-id="43081-172">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="43081-172">Asia/Riyadh</span></span>

<span data-ttu-id="43081-173">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="43081-173">Africa/Nairobi</span></span>

<span data-ttu-id="43081-174">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="43081-174">Asia/Tehran</span></span>

<span data-ttu-id="43081-175">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="43081-175">Asia/Dubai</span></span>

<span data-ttu-id="43081-176">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="43081-176">Asia/Baku</span></span>

<span data-ttu-id="43081-177">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="43081-177">Europe/Moscow</span></span>

<span data-ttu-id="43081-178">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="43081-178">Indian/Mauritius</span></span>

<span data-ttu-id="43081-179">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="43081-179">Asia/Tbilisi</span></span>

<span data-ttu-id="43081-180">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="43081-180">Asia/Yerevan</span></span>

<span data-ttu-id="43081-181">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="43081-181">Asia/Kabul</span></span>

<span data-ttu-id="43081-182">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="43081-182">Asia/Karachi</span></span>

<span data-ttu-id="43081-183">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="43081-183">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="43081-184">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="43081-184">Asia/Kolkata</span></span>

<span data-ttu-id="43081-185">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="43081-185">Asia/Colombo</span></span>

<span data-ttu-id="43081-186">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="43081-186">Asia/Kathmandu</span></span>

<span data-ttu-id="43081-187">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="43081-187">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="43081-188">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="43081-188">Asia/Dhaka</span></span>

<span data-ttu-id="43081-189">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="43081-189">Asia/Yekaterinburg</span></span>

<span data-ttu-id="43081-190">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="43081-190">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="43081-191">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="43081-191">Asia/Bangkok</span></span>

<span data-ttu-id="43081-192">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="43081-192">Asia/Novosibirsk</span></span>

<span data-ttu-id="43081-193">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="43081-193">Asia/Shanghai</span></span>

<span data-ttu-id="43081-194">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="43081-194">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="43081-195">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="43081-195">Asia/Singapore</span></span>

<span data-ttu-id="43081-196">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="43081-196">Australia/Perth</span></span>

<span data-ttu-id="43081-197">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="43081-197">Asia/Taipei</span></span>

<span data-ttu-id="43081-198">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="43081-198">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="43081-199">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="43081-199">Asia/Irkutsk</span></span>

<span data-ttu-id="43081-200">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="43081-200">Asia/Tokyo</span></span>

<span data-ttu-id="43081-201">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="43081-201">Asia/Seoul</span></span>

<span data-ttu-id="43081-202">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="43081-202">Australia/Adelaide</span></span>

<span data-ttu-id="43081-203">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="43081-203">Australia/Darwin</span></span>

<span data-ttu-id="43081-204">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="43081-204">Australia/Brisbane</span></span>

<span data-ttu-id="43081-205">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="43081-205">Australia/Sydney</span></span>

<span data-ttu-id="43081-206">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="43081-206">Pacific/Port_Moresby</span></span>

<span data-ttu-id="43081-207">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="43081-207">Australia/Hobart</span></span>

<span data-ttu-id="43081-208">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="43081-208">Asia/Yakutsk</span></span>

<span data-ttu-id="43081-209">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="43081-209">Pacific/Guadalcanal</span></span>

<span data-ttu-id="43081-210">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="43081-210">Asia/Vladivostok</span></span>

<span data-ttu-id="43081-211">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="43081-211">Pacific/Auckland</span></span>

<span data-ttu-id="43081-212">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="43081-212">Etc/GMT-12</span></span>

<span data-ttu-id="43081-213">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="43081-213">Pacific/Fiji</span></span>

<span data-ttu-id="43081-214">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="43081-214">Asia/Magadan</span></span>

<span data-ttu-id="43081-215">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="43081-215">Pacific/Tongatapu</span></span>

<span data-ttu-id="43081-216">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="43081-216">Pacific/Apia</span></span>

<span data-ttu-id="43081-217">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="43081-217">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="43081-218">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43081-218">JSON representation</span></span>

<span data-ttu-id="43081-219">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="43081-219">Here is a JSON representation of the resource</span></span>

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
