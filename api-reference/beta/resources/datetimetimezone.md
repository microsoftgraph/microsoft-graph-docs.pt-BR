---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Normal
doc_type: resourcePageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: e7f283cc98406564a7c58a525a689b54e043a333
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049965"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="fe536-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="fe536-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="fe536-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe536-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe536-105">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="fe536-105">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="fe536-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe536-106">Properties</span></span>
| <span data-ttu-id="fe536-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe536-107">Property</span></span>     | <span data-ttu-id="fe536-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe536-108">Type</span></span>   |<span data-ttu-id="fe536-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe536-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe536-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="fe536-110">dateTime</span></span>|<span data-ttu-id="fe536-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe536-111">String</span></span>|<span data-ttu-id="fe536-112">Um único ponto de tempo em uma representação combinada de data e hora (`{date}T{time}`).</span><span class="sxs-lookup"><span data-stu-id="fe536-112">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="fe536-113">Por exemplo, "2019-04-16T09:00:00".</span><span class="sxs-lookup"><span data-stu-id="fe536-113">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="fe536-114">timeZone</span><span class="sxs-lookup"><span data-stu-id="fe536-114">timeZone</span></span>|<span data-ttu-id="fe536-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe536-115">String</span></span>|<span data-ttu-id="fe536-116">Representa um fuso horário, por exemplo, "Hora Padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="fe536-116">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="fe536-117">Confira abaixo os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="fe536-117">See below for possible values.</span></span>|

<span data-ttu-id="fe536-118">Em geral, a propriedade**timeZone** _pode_ ser definida como qualquer um dos [fusos horários com suporte no Windows](/windows-hardware/manufacture/desktop/default-time-zones), bem como [os fusos horários adicionais com suporte da API do calendário](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="fe536-118">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="fe536-119">Ao usar **dateTimeTimeZone** em conjunto com um método (como por exemplo, [criar](../api/user-post-events.md) ou [atualizar](../api/event-update.md) um evento), anote os fusos horários que têm suporte, o que podem ser um subconjunto menor.</span><span class="sxs-lookup"><span data-stu-id="fe536-119">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="fe536-120">Fusos horários adicionais</span><span class="sxs-lookup"><span data-stu-id="fe536-120">Additional time zones</span></span>

<span data-ttu-id="fe536-121">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="fe536-121">Etc/GMT+12</span></span>

<span data-ttu-id="fe536-122">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="fe536-122">Etc/GMT+11</span></span>

<span data-ttu-id="fe536-123">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="fe536-123">Pacific/Honolulu</span></span>

<span data-ttu-id="fe536-124">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="fe536-124">America/Anchorage</span></span>

<span data-ttu-id="fe536-125">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="fe536-125">America/Santa_Isabel</span></span>

<span data-ttu-id="fe536-126">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="fe536-126">America/Los_Angeles</span></span>

<span data-ttu-id="fe536-127">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="fe536-127">America/Phoenix</span></span>

<span data-ttu-id="fe536-128">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="fe536-128">America/Chihuahua</span></span>

<span data-ttu-id="fe536-129">América/Denver</span><span class="sxs-lookup"><span data-stu-id="fe536-129">America/Denver</span></span>

<span data-ttu-id="fe536-130">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="fe536-130">America/Guatemala</span></span>

<span data-ttu-id="fe536-131">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="fe536-131">America/Chicago</span></span>

<span data-ttu-id="fe536-132">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="fe536-132">America/Mexico_City</span></span>

<span data-ttu-id="fe536-133">América/Regina</span><span class="sxs-lookup"><span data-stu-id="fe536-133">America/Regina</span></span>

<span data-ttu-id="fe536-134">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="fe536-134">America/Bogota</span></span>

<span data-ttu-id="fe536-135">América/New_York</span><span class="sxs-lookup"><span data-stu-id="fe536-135">America/New_York</span></span>

<span data-ttu-id="fe536-136">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="fe536-136">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="fe536-137">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="fe536-137">America/Caracas</span></span>

<span data-ttu-id="fe536-138">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="fe536-138">America/Asuncion</span></span>

<span data-ttu-id="fe536-139">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="fe536-139">America/Halifax</span></span>

<span data-ttu-id="fe536-140">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="fe536-140">America/Cuiaba</span></span>

<span data-ttu-id="fe536-141">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="fe536-141">America/La_Paz</span></span>

<span data-ttu-id="fe536-142">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="fe536-142">America/Santiago</span></span>

<span data-ttu-id="fe536-143">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="fe536-143">America/St_Johns</span></span>

<span data-ttu-id="fe536-144">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="fe536-144">America/Sao_Paulo</span></span>

<span data-ttu-id="fe536-145">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="fe536-145">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="fe536-146">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="fe536-146">America/Cayenne</span></span>

<span data-ttu-id="fe536-147">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="fe536-147">America/Godthab</span></span>

<span data-ttu-id="fe536-148">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="fe536-148">America/Montevideo</span></span>

<span data-ttu-id="fe536-149">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="fe536-149">America/Bahia</span></span>

<span data-ttu-id="fe536-150">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="fe536-150">Etc/GMT+2</span></span>

<span data-ttu-id="fe536-151">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="fe536-151">Atlantic/Azores</span></span>

<span data-ttu-id="fe536-152">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="fe536-152">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="fe536-153">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="fe536-153">Africa/Casablanca</span></span>

<span data-ttu-id="fe536-154">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="fe536-154">Etc/GMT</span></span>

<span data-ttu-id="fe536-155">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="fe536-155">Europe/London</span></span>

<span data-ttu-id="fe536-156">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="fe536-156">Atlantic/Reykjavik</span></span>

<span data-ttu-id="fe536-157">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="fe536-157">Europe/Berlin</span></span>

<span data-ttu-id="fe536-158">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="fe536-158">Europe/Budapest</span></span>

<span data-ttu-id="fe536-159">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="fe536-159">Europe/Paris</span></span>

<span data-ttu-id="fe536-160">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="fe536-160">Europe/Warsaw</span></span>

<span data-ttu-id="fe536-161">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="fe536-161">Africa/Lagos</span></span>

<span data-ttu-id="fe536-162">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="fe536-162">Africa/Windhoek</span></span>

<span data-ttu-id="fe536-163">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="fe536-163">Europe/Bucharest</span></span>

<span data-ttu-id="fe536-164">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="fe536-164">Asia/Beirut</span></span>

<span data-ttu-id="fe536-165">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="fe536-165">Africa/Cairo</span></span>

<span data-ttu-id="fe536-166">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="fe536-166">Asia/Damascus</span></span>

<span data-ttu-id="fe536-167">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="fe536-167">Africa/Johannesburg</span></span>

<span data-ttu-id="fe536-168">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="fe536-168">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="fe536-169">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="fe536-169">Europe/Istanbul</span></span>

<span data-ttu-id="fe536-170">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="fe536-170">Asia/Jerusalem</span></span>

<span data-ttu-id="fe536-171">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="fe536-171">Asia/Amman</span></span>

<span data-ttu-id="fe536-172">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="fe536-172">Asia/Baghdad</span></span>

<span data-ttu-id="fe536-173">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="fe536-173">Europe/Kaliningrad</span></span>

<span data-ttu-id="fe536-174">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="fe536-174">Asia/Riyadh</span></span>

<span data-ttu-id="fe536-175">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="fe536-175">Africa/Nairobi</span></span>

<span data-ttu-id="fe536-176">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="fe536-176">Asia/Tehran</span></span>

<span data-ttu-id="fe536-177">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="fe536-177">Asia/Dubai</span></span>

<span data-ttu-id="fe536-178">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="fe536-178">Asia/Baku</span></span>

<span data-ttu-id="fe536-179">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="fe536-179">Europe/Moscow</span></span>

<span data-ttu-id="fe536-180">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="fe536-180">Indian/Mauritius</span></span>

<span data-ttu-id="fe536-181">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="fe536-181">Asia/Tbilisi</span></span>

<span data-ttu-id="fe536-182">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="fe536-182">Asia/Yerevan</span></span>

<span data-ttu-id="fe536-183">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="fe536-183">Asia/Kabul</span></span>

<span data-ttu-id="fe536-184">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="fe536-184">Asia/Karachi</span></span>

<span data-ttu-id="fe536-185">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="fe536-185">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="fe536-186">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="fe536-186">Asia/Kolkata</span></span>

<span data-ttu-id="fe536-187">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="fe536-187">Asia/Colombo</span></span>

<span data-ttu-id="fe536-188">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="fe536-188">Asia/Kathmandu</span></span>

<span data-ttu-id="fe536-189">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="fe536-189">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="fe536-190">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="fe536-190">Asia/Dhaka</span></span>

<span data-ttu-id="fe536-191">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="fe536-191">Asia/Yekaterinburg</span></span>

<span data-ttu-id="fe536-192">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="fe536-192">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="fe536-193">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="fe536-193">Asia/Bangkok</span></span>

<span data-ttu-id="fe536-194">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="fe536-194">Asia/Novosibirsk</span></span>

<span data-ttu-id="fe536-195">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="fe536-195">Asia/Shanghai</span></span>

<span data-ttu-id="fe536-196">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="fe536-196">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="fe536-197">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="fe536-197">Asia/Singapore</span></span>

<span data-ttu-id="fe536-198">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="fe536-198">Australia/Perth</span></span>

<span data-ttu-id="fe536-199">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="fe536-199">Asia/Taipei</span></span>

<span data-ttu-id="fe536-200">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="fe536-200">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="fe536-201">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="fe536-201">Asia/Irkutsk</span></span>

<span data-ttu-id="fe536-202">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="fe536-202">Asia/Tokyo</span></span>

<span data-ttu-id="fe536-203">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="fe536-203">Asia/Seoul</span></span>

<span data-ttu-id="fe536-204">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="fe536-204">Australia/Adelaide</span></span>

<span data-ttu-id="fe536-205">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="fe536-205">Australia/Darwin</span></span>

<span data-ttu-id="fe536-206">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="fe536-206">Australia/Brisbane</span></span>

<span data-ttu-id="fe536-207">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="fe536-207">Australia/Sydney</span></span>

<span data-ttu-id="fe536-208">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="fe536-208">Pacific/Port_Moresby</span></span>

<span data-ttu-id="fe536-209">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="fe536-209">Australia/Hobart</span></span>

<span data-ttu-id="fe536-210">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="fe536-210">Asia/Yakutsk</span></span>

<span data-ttu-id="fe536-211">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="fe536-211">Pacific/Guadalcanal</span></span>

<span data-ttu-id="fe536-212">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="fe536-212">Asia/Vladivostok</span></span>

<span data-ttu-id="fe536-213">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="fe536-213">Pacific/Auckland</span></span>

<span data-ttu-id="fe536-214">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="fe536-214">Etc/GMT-12</span></span>

<span data-ttu-id="fe536-215">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="fe536-215">Pacific/Fiji</span></span>

<span data-ttu-id="fe536-216">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="fe536-216">Asia/Magadan</span></span>

<span data-ttu-id="fe536-217">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="fe536-217">Pacific/Tongatapu</span></span>

<span data-ttu-id="fe536-218">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="fe536-218">Pacific/Apia</span></span>

<span data-ttu-id="fe536-219">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="fe536-219">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe536-220">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe536-220">JSON representation</span></span>

<span data-ttu-id="fe536-221">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fe536-221">Here is a JSON representation of the resource</span></span>

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


