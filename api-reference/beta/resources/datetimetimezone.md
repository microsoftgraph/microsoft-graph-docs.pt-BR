---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Normal
doc_type: resourcePageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: 592e8cecccdf8d1514515c4b67a9517352f5a643
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463057"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="5a31a-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5a31a-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="5a31a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a31a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a31a-105">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="5a31a-105">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="5a31a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a31a-106">Properties</span></span>
| <span data-ttu-id="5a31a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a31a-107">Property</span></span>     | <span data-ttu-id="5a31a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a31a-108">Type</span></span>   |<span data-ttu-id="5a31a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a31a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a31a-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="5a31a-110">dateTime</span></span>|<span data-ttu-id="5a31a-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a31a-111">String</span></span>|<span data-ttu-id="5a31a-112">Um único ponto de tempo em uma representação combinada de data e hora (`{date}T{time}`).</span><span class="sxs-lookup"><span data-stu-id="5a31a-112">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="5a31a-113">Por exemplo, "2019-04-16T09:00:00".</span><span class="sxs-lookup"><span data-stu-id="5a31a-113">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="5a31a-114">timeZone</span><span class="sxs-lookup"><span data-stu-id="5a31a-114">timeZone</span></span>|<span data-ttu-id="5a31a-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a31a-115">String</span></span>|<span data-ttu-id="5a31a-116">Representa um fuso horário, por exemplo, "Hora Padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="5a31a-116">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="5a31a-117">Confira abaixo os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="5a31a-117">See below for possible values.</span></span>|

<span data-ttu-id="5a31a-118">Em geral, a propriedade**timeZone** _pode_ ser definida como qualquer um dos [fusos horários com suporte no Windows](/windows-hardware/manufacture/desktop/default-time-zones), bem como [os fusos horários adicionais com suporte da API do calendário](#additional-time-zones).</span><span class="sxs-lookup"><span data-stu-id="5a31a-118">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="5a31a-119">Ao usar **dateTimeTimeZone** em conjunto com um método (como por exemplo, [criar](../api/user-post-events.md) ou [atualizar](../api/event-update.md) um evento), anote os fusos horários que têm suporte, o que podem ser um subconjunto menor.</span><span class="sxs-lookup"><span data-stu-id="5a31a-119">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="5a31a-120">Fusos horários adicionais</span><span class="sxs-lookup"><span data-stu-id="5a31a-120">Additional time zones</span></span>

<span data-ttu-id="5a31a-121">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="5a31a-121">Etc/GMT+12</span></span>

<span data-ttu-id="5a31a-122">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="5a31a-122">Etc/GMT+11</span></span>

<span data-ttu-id="5a31a-123">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="5a31a-123">Pacific/Honolulu</span></span>

<span data-ttu-id="5a31a-124">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="5a31a-124">America/Anchorage</span></span>

<span data-ttu-id="5a31a-125">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="5a31a-125">America/Santa_Isabel</span></span>

<span data-ttu-id="5a31a-126">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="5a31a-126">America/Los_Angeles</span></span>

<span data-ttu-id="5a31a-127">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="5a31a-127">America/Phoenix</span></span>

<span data-ttu-id="5a31a-128">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="5a31a-128">America/Chihuahua</span></span>

<span data-ttu-id="5a31a-129">América/Denver</span><span class="sxs-lookup"><span data-stu-id="5a31a-129">America/Denver</span></span>

<span data-ttu-id="5a31a-130">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="5a31a-130">America/Guatemala</span></span>

<span data-ttu-id="5a31a-131">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="5a31a-131">America/Chicago</span></span>

<span data-ttu-id="5a31a-132">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="5a31a-132">America/Mexico_City</span></span>

<span data-ttu-id="5a31a-133">América/Regina</span><span class="sxs-lookup"><span data-stu-id="5a31a-133">America/Regina</span></span>

<span data-ttu-id="5a31a-134">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="5a31a-134">America/Bogota</span></span>

<span data-ttu-id="5a31a-135">América/New_York</span><span class="sxs-lookup"><span data-stu-id="5a31a-135">America/New_York</span></span>

<span data-ttu-id="5a31a-136">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="5a31a-136">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="5a31a-137">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="5a31a-137">America/Caracas</span></span>

<span data-ttu-id="5a31a-138">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="5a31a-138">America/Asuncion</span></span>

<span data-ttu-id="5a31a-139">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="5a31a-139">America/Halifax</span></span>

<span data-ttu-id="5a31a-140">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="5a31a-140">America/Cuiaba</span></span>

<span data-ttu-id="5a31a-141">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="5a31a-141">America/La_Paz</span></span>

<span data-ttu-id="5a31a-142">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="5a31a-142">America/Santiago</span></span>

<span data-ttu-id="5a31a-143">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="5a31a-143">America/St_Johns</span></span>

<span data-ttu-id="5a31a-144">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="5a31a-144">America/Sao_Paulo</span></span>

<span data-ttu-id="5a31a-145">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="5a31a-145">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="5a31a-146">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="5a31a-146">America/Cayenne</span></span>

<span data-ttu-id="5a31a-147">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="5a31a-147">America/Godthab</span></span>

<span data-ttu-id="5a31a-148">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="5a31a-148">America/Montevideo</span></span>

<span data-ttu-id="5a31a-149">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="5a31a-149">America/Bahia</span></span>

<span data-ttu-id="5a31a-150">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="5a31a-150">Etc/GMT+2</span></span>

<span data-ttu-id="5a31a-151">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="5a31a-151">Atlantic/Azores</span></span>

<span data-ttu-id="5a31a-152">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="5a31a-152">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="5a31a-153">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="5a31a-153">Africa/Casablanca</span></span>

<span data-ttu-id="5a31a-154">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="5a31a-154">Etc/GMT</span></span>

<span data-ttu-id="5a31a-155">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="5a31a-155">Europe/London</span></span>

<span data-ttu-id="5a31a-156">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="5a31a-156">Atlantic/Reykjavik</span></span>

<span data-ttu-id="5a31a-157">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="5a31a-157">Europe/Berlin</span></span>

<span data-ttu-id="5a31a-158">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="5a31a-158">Europe/Budapest</span></span>

<span data-ttu-id="5a31a-159">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="5a31a-159">Europe/Paris</span></span>

<span data-ttu-id="5a31a-160">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="5a31a-160">Europe/Warsaw</span></span>

<span data-ttu-id="5a31a-161">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="5a31a-161">Africa/Lagos</span></span>

<span data-ttu-id="5a31a-162">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="5a31a-162">Africa/Windhoek</span></span>

<span data-ttu-id="5a31a-163">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="5a31a-163">Europe/Bucharest</span></span>

<span data-ttu-id="5a31a-164">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="5a31a-164">Asia/Beirut</span></span>

<span data-ttu-id="5a31a-165">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="5a31a-165">Africa/Cairo</span></span>

<span data-ttu-id="5a31a-166">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="5a31a-166">Asia/Damascus</span></span>

<span data-ttu-id="5a31a-167">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="5a31a-167">Africa/Johannesburg</span></span>

<span data-ttu-id="5a31a-168">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="5a31a-168">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="5a31a-169">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="5a31a-169">Europe/Istanbul</span></span>

<span data-ttu-id="5a31a-170">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="5a31a-170">Asia/Jerusalem</span></span>

<span data-ttu-id="5a31a-171">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="5a31a-171">Asia/Amman</span></span>

<span data-ttu-id="5a31a-172">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="5a31a-172">Asia/Baghdad</span></span>

<span data-ttu-id="5a31a-173">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="5a31a-173">Europe/Kaliningrad</span></span>

<span data-ttu-id="5a31a-174">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="5a31a-174">Asia/Riyadh</span></span>

<span data-ttu-id="5a31a-175">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="5a31a-175">Africa/Nairobi</span></span>

<span data-ttu-id="5a31a-176">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="5a31a-176">Asia/Tehran</span></span>

<span data-ttu-id="5a31a-177">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="5a31a-177">Asia/Dubai</span></span>

<span data-ttu-id="5a31a-178">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="5a31a-178">Asia/Baku</span></span>

<span data-ttu-id="5a31a-179">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="5a31a-179">Europe/Moscow</span></span>

<span data-ttu-id="5a31a-180">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="5a31a-180">Indian/Mauritius</span></span>

<span data-ttu-id="5a31a-181">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="5a31a-181">Asia/Tbilisi</span></span>

<span data-ttu-id="5a31a-182">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="5a31a-182">Asia/Yerevan</span></span>

<span data-ttu-id="5a31a-183">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="5a31a-183">Asia/Kabul</span></span>

<span data-ttu-id="5a31a-184">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="5a31a-184">Asia/Karachi</span></span>

<span data-ttu-id="5a31a-185">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="5a31a-185">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="5a31a-186">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="5a31a-186">Asia/Kolkata</span></span>

<span data-ttu-id="5a31a-187">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="5a31a-187">Asia/Colombo</span></span>

<span data-ttu-id="5a31a-188">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="5a31a-188">Asia/Kathmandu</span></span>

<span data-ttu-id="5a31a-189">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="5a31a-189">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="5a31a-190">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="5a31a-190">Asia/Dhaka</span></span>

<span data-ttu-id="5a31a-191">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="5a31a-191">Asia/Yekaterinburg</span></span>

<span data-ttu-id="5a31a-192">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="5a31a-192">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="5a31a-193">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="5a31a-193">Asia/Bangkok</span></span>

<span data-ttu-id="5a31a-194">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="5a31a-194">Asia/Novosibirsk</span></span>

<span data-ttu-id="5a31a-195">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="5a31a-195">Asia/Shanghai</span></span>

<span data-ttu-id="5a31a-196">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="5a31a-196">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="5a31a-197">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="5a31a-197">Asia/Singapore</span></span>

<span data-ttu-id="5a31a-198">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="5a31a-198">Australia/Perth</span></span>

<span data-ttu-id="5a31a-199">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="5a31a-199">Asia/Taipei</span></span>

<span data-ttu-id="5a31a-200">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="5a31a-200">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="5a31a-201">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="5a31a-201">Asia/Irkutsk</span></span>

<span data-ttu-id="5a31a-202">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="5a31a-202">Asia/Tokyo</span></span>

<span data-ttu-id="5a31a-203">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="5a31a-203">Asia/Seoul</span></span>

<span data-ttu-id="5a31a-204">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="5a31a-204">Australia/Adelaide</span></span>

<span data-ttu-id="5a31a-205">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="5a31a-205">Australia/Darwin</span></span>

<span data-ttu-id="5a31a-206">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="5a31a-206">Australia/Brisbane</span></span>

<span data-ttu-id="5a31a-207">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="5a31a-207">Australia/Sydney</span></span>

<span data-ttu-id="5a31a-208">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="5a31a-208">Pacific/Port_Moresby</span></span>

<span data-ttu-id="5a31a-209">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="5a31a-209">Australia/Hobart</span></span>

<span data-ttu-id="5a31a-210">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="5a31a-210">Asia/Yakutsk</span></span>

<span data-ttu-id="5a31a-211">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="5a31a-211">Pacific/Guadalcanal</span></span>

<span data-ttu-id="5a31a-212">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="5a31a-212">Asia/Vladivostok</span></span>

<span data-ttu-id="5a31a-213">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="5a31a-213">Pacific/Auckland</span></span>

<span data-ttu-id="5a31a-214">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="5a31a-214">Etc/GMT-12</span></span>

<span data-ttu-id="5a31a-215">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="5a31a-215">Pacific/Fiji</span></span>

<span data-ttu-id="5a31a-216">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="5a31a-216">Asia/Magadan</span></span>

<span data-ttu-id="5a31a-217">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="5a31a-217">Pacific/Tongatapu</span></span>

<span data-ttu-id="5a31a-218">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="5a31a-218">Pacific/Apia</span></span>

<span data-ttu-id="5a31a-219">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="5a31a-219">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a31a-220">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a31a-220">JSON representation</span></span>

<span data-ttu-id="5a31a-221">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5a31a-221">Here is a JSON representation of the resource</span></span>

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
