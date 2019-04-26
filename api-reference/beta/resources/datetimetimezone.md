---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Normal
ms.openlocfilehash: 4bf62081d190e3af031d305c7db7f64d606926b6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340955"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="5d3a8-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5d3a8-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d3a8-104">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="5d3a8-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="5d3a8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d3a8-105">Properties</span></span>
| <span data-ttu-id="5d3a8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d3a8-106">Property</span></span>     | <span data-ttu-id="5d3a8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d3a8-107">Type</span></span>   |<span data-ttu-id="5d3a8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d3a8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d3a8-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="5d3a8-109">dateTime</span></span>|<span data-ttu-id="5d3a8-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d3a8-110">String</span></span>|<span data-ttu-id="5d3a8-111">Um único ponto de tempo em uma representação combinada de data e hora (`{date}T{time}`).</span><span class="sxs-lookup"><span data-stu-id="5d3a8-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="5d3a8-112">Por exemplo, "2019-04-16T09:00:00".</span><span class="sxs-lookup"><span data-stu-id="5d3a8-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="5d3a8-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="5d3a8-113">timeZone</span></span>|<span data-ttu-id="5d3a8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d3a8-114">String</span></span>|<span data-ttu-id="5d3a8-115">Um nome de fuso horário, conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="5d3a8-115">A time zone name as described below.</span></span>|

<span data-ttu-id="5d3a8-116">A propriedade **timeZone** pode ser definida para qualquer um dos fusos horários com suporte no Windows, bem como os nomes de fusos horários a seguir.</span><span class="sxs-lookup"><span data-stu-id="5d3a8-116">The **timeZone** property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="5d3a8-117">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="5d3a8-117">Etc/GMT+12</span></span>

<span data-ttu-id="5d3a8-118">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="5d3a8-118">Etc/GMT+11</span></span>

<span data-ttu-id="5d3a8-119">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="5d3a8-119">Pacific/Honolulu</span></span>

<span data-ttu-id="5d3a8-120">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="5d3a8-120">America/Anchorage</span></span>

<span data-ttu-id="5d3a8-121">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="5d3a8-121">America/Santa_Isabel</span></span>

<span data-ttu-id="5d3a8-122">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="5d3a8-122">America/Los_Angeles</span></span>

<span data-ttu-id="5d3a8-123">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="5d3a8-123">America/Phoenix</span></span>

<span data-ttu-id="5d3a8-124">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="5d3a8-124">America/Chihuahua</span></span>

<span data-ttu-id="5d3a8-125">América/Denver</span><span class="sxs-lookup"><span data-stu-id="5d3a8-125">America/Denver</span></span>

<span data-ttu-id="5d3a8-126">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="5d3a8-126">America/Guatemala</span></span>

<span data-ttu-id="5d3a8-127">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="5d3a8-127">America/Chicago</span></span>

<span data-ttu-id="5d3a8-128">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="5d3a8-128">America/Mexico_City</span></span>

<span data-ttu-id="5d3a8-129">América/Regina</span><span class="sxs-lookup"><span data-stu-id="5d3a8-129">America/Regina</span></span>

<span data-ttu-id="5d3a8-130">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="5d3a8-130">America/Bogota</span></span>

<span data-ttu-id="5d3a8-131">América/New_York</span><span class="sxs-lookup"><span data-stu-id="5d3a8-131">America/New_York</span></span>

<span data-ttu-id="5d3a8-132">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="5d3a8-132">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="5d3a8-133">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="5d3a8-133">America/Caracas</span></span>

<span data-ttu-id="5d3a8-134">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="5d3a8-134">America/Asuncion</span></span>

<span data-ttu-id="5d3a8-135">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="5d3a8-135">America/Halifax</span></span>

<span data-ttu-id="5d3a8-136">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="5d3a8-136">America/Cuiaba</span></span>

<span data-ttu-id="5d3a8-137">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="5d3a8-137">America/La_Paz</span></span>

<span data-ttu-id="5d3a8-138">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="5d3a8-138">America/Santiago</span></span>

<span data-ttu-id="5d3a8-139">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="5d3a8-139">America/St_Johns</span></span>

<span data-ttu-id="5d3a8-140">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="5d3a8-140">America/Sao_Paulo</span></span>

<span data-ttu-id="5d3a8-141">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="5d3a8-141">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="5d3a8-142">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="5d3a8-142">America/Cayenne</span></span>

<span data-ttu-id="5d3a8-143">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="5d3a8-143">America/Godthab</span></span>

<span data-ttu-id="5d3a8-144">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="5d3a8-144">America/Montevideo</span></span>

<span data-ttu-id="5d3a8-145">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="5d3a8-145">America/Bahia</span></span>

<span data-ttu-id="5d3a8-146">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="5d3a8-146">Etc/GMT+2</span></span>

<span data-ttu-id="5d3a8-147">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="5d3a8-147">Atlantic/Azores</span></span>

<span data-ttu-id="5d3a8-148">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="5d3a8-148">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="5d3a8-149">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="5d3a8-149">Africa/Casablanca</span></span>

<span data-ttu-id="5d3a8-150">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="5d3a8-150">Etc/GMT</span></span>

<span data-ttu-id="5d3a8-151">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="5d3a8-151">Europe/London</span></span>

<span data-ttu-id="5d3a8-152">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="5d3a8-152">Atlantic/Reykjavik</span></span>

<span data-ttu-id="5d3a8-153">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="5d3a8-153">Europe/Berlin</span></span>

<span data-ttu-id="5d3a8-154">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="5d3a8-154">Europe/Budapest</span></span>

<span data-ttu-id="5d3a8-155">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="5d3a8-155">Europe/Paris</span></span>

<span data-ttu-id="5d3a8-156">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="5d3a8-156">Europe/Warsaw</span></span>

<span data-ttu-id="5d3a8-157">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="5d3a8-157">Africa/Lagos</span></span>

<span data-ttu-id="5d3a8-158">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="5d3a8-158">Africa/Windhoek</span></span>

<span data-ttu-id="5d3a8-159">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="5d3a8-159">Europe/Bucharest</span></span>

<span data-ttu-id="5d3a8-160">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="5d3a8-160">Asia/Beirut</span></span>

<span data-ttu-id="5d3a8-161">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="5d3a8-161">Africa/Cairo</span></span>

<span data-ttu-id="5d3a8-162">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="5d3a8-162">Asia/Damascus</span></span>

<span data-ttu-id="5d3a8-163">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="5d3a8-163">Africa/Johannesburg</span></span>

<span data-ttu-id="5d3a8-164">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="5d3a8-164">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="5d3a8-165">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="5d3a8-165">Europe/Istanbul</span></span>

<span data-ttu-id="5d3a8-166">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="5d3a8-166">Asia/Jerusalem</span></span>

<span data-ttu-id="5d3a8-167">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="5d3a8-167">Asia/Amman</span></span>

<span data-ttu-id="5d3a8-168">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="5d3a8-168">Asia/Baghdad</span></span>

<span data-ttu-id="5d3a8-169">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="5d3a8-169">Europe/Kaliningrad</span></span>

<span data-ttu-id="5d3a8-170">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="5d3a8-170">Asia/Riyadh</span></span>

<span data-ttu-id="5d3a8-171">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="5d3a8-171">Africa/Nairobi</span></span>

<span data-ttu-id="5d3a8-172">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="5d3a8-172">Asia/Tehran</span></span>

<span data-ttu-id="5d3a8-173">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="5d3a8-173">Asia/Dubai</span></span>

<span data-ttu-id="5d3a8-174">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="5d3a8-174">Asia/Baku</span></span>

<span data-ttu-id="5d3a8-175">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="5d3a8-175">Europe/Moscow</span></span>

<span data-ttu-id="5d3a8-176">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="5d3a8-176">Indian/Mauritius</span></span>

<span data-ttu-id="5d3a8-177">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="5d3a8-177">Asia/Tbilisi</span></span>

<span data-ttu-id="5d3a8-178">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="5d3a8-178">Asia/Yerevan</span></span>

<span data-ttu-id="5d3a8-179">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="5d3a8-179">Asia/Kabul</span></span>

<span data-ttu-id="5d3a8-180">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="5d3a8-180">Asia/Karachi</span></span>

<span data-ttu-id="5d3a8-181">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="5d3a8-181">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="5d3a8-182">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="5d3a8-182">Asia/Kolkata</span></span>

<span data-ttu-id="5d3a8-183">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="5d3a8-183">Asia/Colombo</span></span>

<span data-ttu-id="5d3a8-184">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="5d3a8-184">Asia/Kathmandu</span></span>

<span data-ttu-id="5d3a8-185">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="5d3a8-185">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="5d3a8-186">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="5d3a8-186">Asia/Dhaka</span></span>

<span data-ttu-id="5d3a8-187">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="5d3a8-187">Asia/Yekaterinburg</span></span>

<span data-ttu-id="5d3a8-188">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="5d3a8-188">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="5d3a8-189">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="5d3a8-189">Asia/Bangkok</span></span>

<span data-ttu-id="5d3a8-190">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="5d3a8-190">Asia/Novosibirsk</span></span>

<span data-ttu-id="5d3a8-191">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="5d3a8-191">Asia/Shanghai</span></span>

<span data-ttu-id="5d3a8-192">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="5d3a8-192">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="5d3a8-193">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="5d3a8-193">Asia/Singapore</span></span>

<span data-ttu-id="5d3a8-194">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="5d3a8-194">Australia/Perth</span></span>

<span data-ttu-id="5d3a8-195">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="5d3a8-195">Asia/Taipei</span></span>

<span data-ttu-id="5d3a8-196">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="5d3a8-196">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="5d3a8-197">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="5d3a8-197">Asia/Irkutsk</span></span>

<span data-ttu-id="5d3a8-198">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="5d3a8-198">Asia/Tokyo</span></span>

<span data-ttu-id="5d3a8-199">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="5d3a8-199">Asia/Seoul</span></span>

<span data-ttu-id="5d3a8-200">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="5d3a8-200">Australia/Adelaide</span></span>

<span data-ttu-id="5d3a8-201">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="5d3a8-201">Australia/Darwin</span></span>

<span data-ttu-id="5d3a8-202">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="5d3a8-202">Australia/Brisbane</span></span>

<span data-ttu-id="5d3a8-203">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="5d3a8-203">Australia/Sydney</span></span>

<span data-ttu-id="5d3a8-204">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="5d3a8-204">Pacific/Port_Moresby</span></span>

<span data-ttu-id="5d3a8-205">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="5d3a8-205">Australia/Hobart</span></span>

<span data-ttu-id="5d3a8-206">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="5d3a8-206">Asia/Yakutsk</span></span>

<span data-ttu-id="5d3a8-207">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="5d3a8-207">Pacific/Guadalcanal</span></span>

<span data-ttu-id="5d3a8-208">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="5d3a8-208">Asia/Vladivostok</span></span>

<span data-ttu-id="5d3a8-209">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="5d3a8-209">Pacific/Auckland</span></span>

<span data-ttu-id="5d3a8-210">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="5d3a8-210">Etc/GMT-12</span></span>

<span data-ttu-id="5d3a8-211">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="5d3a8-211">Pacific/Fiji</span></span>

<span data-ttu-id="5d3a8-212">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="5d3a8-212">Asia/Magadan</span></span>

<span data-ttu-id="5d3a8-213">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="5d3a8-213">Pacific/Tongatapu</span></span>

<span data-ttu-id="5d3a8-214">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="5d3a8-214">Pacific/Apia</span></span>

<span data-ttu-id="5d3a8-215">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="5d3a8-215">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d3a8-216">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d3a8-216">JSON representation</span></span>

<span data-ttu-id="5d3a8-217">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5d3a8-217">Here is a JSON representation of the resource</span></span>

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
