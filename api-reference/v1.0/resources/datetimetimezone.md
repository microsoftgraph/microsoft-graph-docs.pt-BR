---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Priority
ms.openlocfilehash: 9e031b053ebc185ee02fa11571019529a870cf04
ms.sourcegitcommit: 7412dd2f2d5ed66afa2b0759c861ad23b4c6ecdf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/23/2019
ms.locfileid: "30212358"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="853ba-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="853ba-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="853ba-104">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="853ba-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="853ba-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="853ba-105">Properties</span></span>
| <span data-ttu-id="853ba-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="853ba-106">Property</span></span>     | <span data-ttu-id="853ba-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="853ba-107">Type</span></span>   |<span data-ttu-id="853ba-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="853ba-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="853ba-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="853ba-109">DateTime</span></span>|<span data-ttu-id="853ba-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="853ba-110">String</span></span>|<span data-ttu-id="853ba-111">Um único ponto de tempo em uma representação combinada de data e hora (`{date}T{time}`; por exemplo, `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="853ba-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span>|
|<span data-ttu-id="853ba-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="853ba-112">timeZone</span></span>|<span data-ttu-id="853ba-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="853ba-113">String</span></span>|<span data-ttu-id="853ba-114">Um dos seguintes nomes de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="853ba-114">One of the following time zone names.</span></span>|

<span data-ttu-id="853ba-115">A propriedade _TimeZone_ pode ser definida para qualquer um dos fusos horários com suporte no Windows, bem como os nomes de fusos horários a seguir.</span><span class="sxs-lookup"><span data-stu-id="853ba-115">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="853ba-116">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="853ba-116">Etc/GMT+12</span></span>

<span data-ttu-id="853ba-117">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="853ba-117">Etc/GMT+11</span></span>

<span data-ttu-id="853ba-118">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="853ba-118">Pacific/Honolulu</span></span>

<span data-ttu-id="853ba-119">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="853ba-119">America/Anchorage</span></span>

<span data-ttu-id="853ba-120">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="853ba-120">America/Santa_Isabel</span></span>

<span data-ttu-id="853ba-121">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="853ba-121">America/Los_Angeles</span></span>

<span data-ttu-id="853ba-122">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="853ba-122">America/Phoenix</span></span>

<span data-ttu-id="853ba-123">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="853ba-123">America/Chihuahua</span></span>

<span data-ttu-id="853ba-124">América/Denver</span><span class="sxs-lookup"><span data-stu-id="853ba-124">America/Denver</span></span>

<span data-ttu-id="853ba-125">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="853ba-125">America/Guatemala</span></span>

<span data-ttu-id="853ba-126">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="853ba-126">America/Chicago</span></span>

<span data-ttu-id="853ba-127">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="853ba-127">America/Mexico_City</span></span>

<span data-ttu-id="853ba-128">América/Regina</span><span class="sxs-lookup"><span data-stu-id="853ba-128">America/Regina</span></span>

<span data-ttu-id="853ba-129">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="853ba-129">America/Bogota</span></span>

<span data-ttu-id="853ba-130">América/New_York</span><span class="sxs-lookup"><span data-stu-id="853ba-130">America/New_York</span></span>

<span data-ttu-id="853ba-131">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="853ba-131">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="853ba-132">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="853ba-132">America/Caracas</span></span>

<span data-ttu-id="853ba-133">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="853ba-133">America/Asuncion</span></span>

<span data-ttu-id="853ba-134">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="853ba-134">America/Halifax</span></span>

<span data-ttu-id="853ba-135">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="853ba-135">America/Cuiaba</span></span>

<span data-ttu-id="853ba-136">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="853ba-136">America/La_Paz</span></span>

<span data-ttu-id="853ba-137">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="853ba-137">America/Santiago</span></span>

<span data-ttu-id="853ba-138">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="853ba-138">America/St_Johns</span></span>

<span data-ttu-id="853ba-139">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="853ba-139">America/Sao_Paulo</span></span>

<span data-ttu-id="853ba-140">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="853ba-140">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="853ba-141">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="853ba-141">America/Cayenne</span></span>

<span data-ttu-id="853ba-142">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="853ba-142">America/Godthab</span></span>

<span data-ttu-id="853ba-143">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="853ba-143">America/Montevideo</span></span>

<span data-ttu-id="853ba-144">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="853ba-144">America/Bahia</span></span>

<span data-ttu-id="853ba-145">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="853ba-145">Etc/GMT+2</span></span>

<span data-ttu-id="853ba-146">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="853ba-146">Atlantic/Azores</span></span>

<span data-ttu-id="853ba-147">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="853ba-147">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="853ba-148">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="853ba-148">Africa/Casablanca</span></span>

<span data-ttu-id="853ba-149">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="853ba-149">Etc/GMT</span></span>

<span data-ttu-id="853ba-150">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="853ba-150">Europe/London</span></span>

<span data-ttu-id="853ba-151">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="853ba-151">Atlantic/Reykjavik</span></span>

<span data-ttu-id="853ba-152">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="853ba-152">Europe/Berlin</span></span>

<span data-ttu-id="853ba-153">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="853ba-153">Europe/Budapest</span></span>

<span data-ttu-id="853ba-154">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="853ba-154">Europe/Paris</span></span>

<span data-ttu-id="853ba-155">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="853ba-155">Europe/Warsaw</span></span>

<span data-ttu-id="853ba-156">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="853ba-156">Africa/Lagos</span></span>

<span data-ttu-id="853ba-157">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="853ba-157">Africa/Windhoek</span></span>

<span data-ttu-id="853ba-158">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="853ba-158">Europe/Bucharest</span></span>

<span data-ttu-id="853ba-159">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="853ba-159">Asia/Beirut</span></span>

<span data-ttu-id="853ba-160">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="853ba-160">Africa/Cairo</span></span>

<span data-ttu-id="853ba-161">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="853ba-161">Asia/Damascus</span></span>

<span data-ttu-id="853ba-162">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="853ba-162">Africa/Johannesburg</span></span>

<span data-ttu-id="853ba-163">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="853ba-163">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="853ba-164">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="853ba-164">Europe/Istanbul</span></span>

<span data-ttu-id="853ba-165">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="853ba-165">Asia/Jerusalem</span></span>

<span data-ttu-id="853ba-166">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="853ba-166">Asia/Amman</span></span>

<span data-ttu-id="853ba-167">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="853ba-167">Asia/Baghdad</span></span>

<span data-ttu-id="853ba-168">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="853ba-168">Europe/Kaliningrad</span></span>

<span data-ttu-id="853ba-169">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="853ba-169">Asia/Riyadh</span></span>

<span data-ttu-id="853ba-170">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="853ba-170">Africa/Nairobi</span></span>

<span data-ttu-id="853ba-171">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="853ba-171">Asia/Tehran</span></span>

<span data-ttu-id="853ba-172">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="853ba-172">Asia/Dubai</span></span>

<span data-ttu-id="853ba-173">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="853ba-173">Asia/Baku</span></span>

<span data-ttu-id="853ba-174">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="853ba-174">Europe/Moscow</span></span>

<span data-ttu-id="853ba-175">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="853ba-175">Indian/Mauritius</span></span>

<span data-ttu-id="853ba-176">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="853ba-176">Asia/Tbilisi</span></span>

<span data-ttu-id="853ba-177">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="853ba-177">Asia/Yerevan</span></span>

<span data-ttu-id="853ba-178">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="853ba-178">Asia/Kabul</span></span>

<span data-ttu-id="853ba-179">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="853ba-179">Asia/Karachi</span></span>

<span data-ttu-id="853ba-180">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="853ba-180">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="853ba-181">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="853ba-181">Asia/Kolkata</span></span>

<span data-ttu-id="853ba-182">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="853ba-182">Asia/Colombo</span></span>

<span data-ttu-id="853ba-183">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="853ba-183">Asia/Kathmandu</span></span>

<span data-ttu-id="853ba-184">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="853ba-184">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="853ba-185">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="853ba-185">Asia/Dhaka</span></span>

<span data-ttu-id="853ba-186">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="853ba-186">Asia/Yekaterinburg</span></span>

<span data-ttu-id="853ba-187">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="853ba-187">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="853ba-188">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="853ba-188">Asia/Bangkok</span></span>

<span data-ttu-id="853ba-189">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="853ba-189">Asia/Novosibirsk</span></span>

<span data-ttu-id="853ba-190">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="853ba-190">Asia/Shanghai</span></span>

<span data-ttu-id="853ba-191">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="853ba-191">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="853ba-192">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="853ba-192">Asia/Singapore</span></span>

<span data-ttu-id="853ba-193">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="853ba-193">Australia/Perth</span></span>

<span data-ttu-id="853ba-194">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="853ba-194">Asia/Taipei</span></span>

<span data-ttu-id="853ba-195">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="853ba-195">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="853ba-196">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="853ba-196">Asia/Irkutsk</span></span>

<span data-ttu-id="853ba-197">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="853ba-197">Asia/Tokyo</span></span>

<span data-ttu-id="853ba-198">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="853ba-198">Asia/Seoul</span></span>

<span data-ttu-id="853ba-199">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="853ba-199">Australia/Adelaide</span></span>

<span data-ttu-id="853ba-200">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="853ba-200">Australia/Darwin</span></span>

<span data-ttu-id="853ba-201">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="853ba-201">Australia/Brisbane</span></span>

<span data-ttu-id="853ba-202">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="853ba-202">Australia/Sydney</span></span>

<span data-ttu-id="853ba-203">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="853ba-203">Pacific/Port_Moresby</span></span>

<span data-ttu-id="853ba-204">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="853ba-204">Australia/Hobart</span></span>

<span data-ttu-id="853ba-205">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="853ba-205">Asia/Yakutsk</span></span>

<span data-ttu-id="853ba-206">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="853ba-206">Pacific/Guadalcanal</span></span>

<span data-ttu-id="853ba-207">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="853ba-207">Asia/Vladivostok</span></span>

<span data-ttu-id="853ba-208">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="853ba-208">Pacific/Auckland</span></span>

<span data-ttu-id="853ba-209">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="853ba-209">Etc/GMT-12</span></span>

<span data-ttu-id="853ba-210">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="853ba-210">Pacific/Fiji</span></span>

<span data-ttu-id="853ba-211">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="853ba-211">Asia/Magadan</span></span>

<span data-ttu-id="853ba-212">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="853ba-212">Pacific/Tongatapu</span></span>

<span data-ttu-id="853ba-213">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="853ba-213">Pacific/Apia</span></span>

<span data-ttu-id="853ba-214">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="853ba-214">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="853ba-215">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="853ba-215">JSON representation</span></span>

<span data-ttu-id="853ba-216">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="853ba-216">Here is a JSON representation of the resource</span></span>

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
