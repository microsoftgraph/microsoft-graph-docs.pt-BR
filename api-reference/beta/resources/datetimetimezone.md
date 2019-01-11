---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Normal
ms.openlocfilehash: 5090edce8d86ff12470cc1bb39f92ef13b42ba15
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876066"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="93698-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="93698-103">dateTimeTimeZone resource type</span></span>

> <span data-ttu-id="93698-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="93698-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93698-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="93698-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93698-106">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="93698-106">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="93698-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93698-107">Properties</span></span>
| <span data-ttu-id="93698-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93698-108">Property</span></span>     | <span data-ttu-id="93698-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="93698-109">Type</span></span>   |<span data-ttu-id="93698-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="93698-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93698-111">DateTime</span><span class="sxs-lookup"><span data-stu-id="93698-111">DateTime</span></span>|<span data-ttu-id="93698-112">String</span><span class="sxs-lookup"><span data-stu-id="93698-112">String</span></span>|<span data-ttu-id="93698-113">Um único ponto de tempo em uma representação combinada de data e hora (`<date>T<time>`).</span><span class="sxs-lookup"><span data-stu-id="93698-113">A single point of time in a combined date and time representation (`<date>T<time>`).</span></span>|
|<span data-ttu-id="93698-114">TimeZone</span><span class="sxs-lookup"><span data-stu-id="93698-114">TimeZone</span></span>|<span data-ttu-id="93698-115">String</span><span class="sxs-lookup"><span data-stu-id="93698-115">String</span></span>|<span data-ttu-id="93698-116">Um dos seguintes nomes de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="93698-116">One of the following time zone names.</span></span>|

<span data-ttu-id="93698-117">A propriedade _TimeZone_ pode ser definida para qualquer um dos fusos horários com suporte no Windows, bem como os nomes de fusos horários a seguir.</span><span class="sxs-lookup"><span data-stu-id="93698-117">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="93698-118">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="93698-118">Etc/GMT+12</span></span>

<span data-ttu-id="93698-119">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="93698-119">Etc/GMT+11</span></span>

<span data-ttu-id="93698-120">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="93698-120">Pacific/Honolulu</span></span>

<span data-ttu-id="93698-121">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="93698-121">America/Anchorage</span></span>

<span data-ttu-id="93698-122">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="93698-122">America/Santa_Isabel</span></span>

<span data-ttu-id="93698-123">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="93698-123">America/Los_Angeles</span></span>

<span data-ttu-id="93698-124">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="93698-124">America/Phoenix</span></span>

<span data-ttu-id="93698-125">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="93698-125">America/Chihuahua</span></span>

<span data-ttu-id="93698-126">América/Denver</span><span class="sxs-lookup"><span data-stu-id="93698-126">America/Denver</span></span>

<span data-ttu-id="93698-127">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="93698-127">America/Guatemala</span></span>

<span data-ttu-id="93698-128">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="93698-128">America/Chicago</span></span>

<span data-ttu-id="93698-129">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="93698-129">America/Mexico_City</span></span>

<span data-ttu-id="93698-130">América/Regina</span><span class="sxs-lookup"><span data-stu-id="93698-130">America/Regina</span></span>

<span data-ttu-id="93698-131">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="93698-131">America/Bogota</span></span>

<span data-ttu-id="93698-132">América/New_York</span><span class="sxs-lookup"><span data-stu-id="93698-132">America/New_York</span></span>

<span data-ttu-id="93698-133">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="93698-133">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="93698-134">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="93698-134">America/Caracas</span></span>

<span data-ttu-id="93698-135">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="93698-135">America/Asuncion</span></span>

<span data-ttu-id="93698-136">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="93698-136">America/Halifax</span></span>

<span data-ttu-id="93698-137">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="93698-137">America/Cuiaba</span></span>

<span data-ttu-id="93698-138">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="93698-138">America/La_Paz</span></span>

<span data-ttu-id="93698-139">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="93698-139">America/Santiago</span></span>

<span data-ttu-id="93698-140">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="93698-140">America/St_Johns</span></span>

<span data-ttu-id="93698-141">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="93698-141">America/Sao_Paulo</span></span>

<span data-ttu-id="93698-142">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="93698-142">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="93698-143">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="93698-143">America/Cayenne</span></span>

<span data-ttu-id="93698-144">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="93698-144">America/Godthab</span></span>

<span data-ttu-id="93698-145">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="93698-145">America/Montevideo</span></span>

<span data-ttu-id="93698-146">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="93698-146">America/Bahia</span></span>

<span data-ttu-id="93698-147">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="93698-147">Etc/GMT+2</span></span>

<span data-ttu-id="93698-148">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="93698-148">Atlantic/Azores</span></span>

<span data-ttu-id="93698-149">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="93698-149">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="93698-150">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="93698-150">Africa/Casablanca</span></span>

<span data-ttu-id="93698-151">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="93698-151">Etc/GMT</span></span>

<span data-ttu-id="93698-152">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="93698-152">Europe/London</span></span>

<span data-ttu-id="93698-153">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="93698-153">Atlantic/Reykjavik</span></span>

<span data-ttu-id="93698-154">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="93698-154">Europe/Berlin</span></span>

<span data-ttu-id="93698-155">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="93698-155">Europe/Budapest</span></span>

<span data-ttu-id="93698-156">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="93698-156">Europe/Paris</span></span>

<span data-ttu-id="93698-157">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="93698-157">Europe/Warsaw</span></span>

<span data-ttu-id="93698-158">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="93698-158">Africa/Lagos</span></span>

<span data-ttu-id="93698-159">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="93698-159">Africa/Windhoek</span></span>

<span data-ttu-id="93698-160">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="93698-160">Europe/Bucharest</span></span>

<span data-ttu-id="93698-161">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="93698-161">Asia/Beirut</span></span>

<span data-ttu-id="93698-162">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="93698-162">Africa/Cairo</span></span>

<span data-ttu-id="93698-163">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="93698-163">Asia/Damascus</span></span>

<span data-ttu-id="93698-164">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="93698-164">Africa/Johannesburg</span></span>

<span data-ttu-id="93698-165">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="93698-165">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="93698-166">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="93698-166">Europe/Istanbul</span></span>

<span data-ttu-id="93698-167">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="93698-167">Asia/Jerusalem</span></span>

<span data-ttu-id="93698-168">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="93698-168">Asia/Amman</span></span>

<span data-ttu-id="93698-169">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="93698-169">Asia/Baghdad</span></span>

<span data-ttu-id="93698-170">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="93698-170">Europe/Kaliningrad</span></span>

<span data-ttu-id="93698-171">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="93698-171">Asia/Riyadh</span></span>

<span data-ttu-id="93698-172">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="93698-172">Africa/Nairobi</span></span>

<span data-ttu-id="93698-173">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="93698-173">Asia/Tehran</span></span>

<span data-ttu-id="93698-174">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="93698-174">Asia/Dubai</span></span>

<span data-ttu-id="93698-175">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="93698-175">Asia/Baku</span></span>

<span data-ttu-id="93698-176">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="93698-176">Europe/Moscow</span></span>

<span data-ttu-id="93698-177">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="93698-177">Indian/Mauritius</span></span>

<span data-ttu-id="93698-178">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="93698-178">Asia/Tbilisi</span></span>

<span data-ttu-id="93698-179">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="93698-179">Asia/Yerevan</span></span>

<span data-ttu-id="93698-180">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="93698-180">Asia/Kabul</span></span>

<span data-ttu-id="93698-181">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="93698-181">Asia/Karachi</span></span>

<span data-ttu-id="93698-182">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="93698-182">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="93698-183">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="93698-183">Asia/Kolkata</span></span>

<span data-ttu-id="93698-184">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="93698-184">Asia/Colombo</span></span>

<span data-ttu-id="93698-185">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="93698-185">Asia/Kathmandu</span></span>

<span data-ttu-id="93698-186">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="93698-186">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="93698-187">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="93698-187">Asia/Dhaka</span></span>

<span data-ttu-id="93698-188">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="93698-188">Asia/Yekaterinburg</span></span>

<span data-ttu-id="93698-189">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="93698-189">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="93698-190">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="93698-190">Asia/Bangkok</span></span>

<span data-ttu-id="93698-191">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="93698-191">Asia/Novosibirsk</span></span>

<span data-ttu-id="93698-192">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="93698-192">Asia/Shanghai</span></span>

<span data-ttu-id="93698-193">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="93698-193">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="93698-194">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="93698-194">Asia/Singapore</span></span>

<span data-ttu-id="93698-195">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="93698-195">Australia/Perth</span></span>

<span data-ttu-id="93698-196">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="93698-196">Asia/Taipei</span></span>

<span data-ttu-id="93698-197">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="93698-197">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="93698-198">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="93698-198">Asia/Irkutsk</span></span>

<span data-ttu-id="93698-199">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="93698-199">Asia/Tokyo</span></span>

<span data-ttu-id="93698-200">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="93698-200">Asia/Seoul</span></span>

<span data-ttu-id="93698-201">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="93698-201">Australia/Adelaide</span></span>

<span data-ttu-id="93698-202">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="93698-202">Australia/Darwin</span></span>

<span data-ttu-id="93698-203">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="93698-203">Australia/Brisbane</span></span>

<span data-ttu-id="93698-204">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="93698-204">Australia/Sydney</span></span>

<span data-ttu-id="93698-205">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="93698-205">Pacific/Port_Moresby</span></span>

<span data-ttu-id="93698-206">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="93698-206">Australia/Hobart</span></span>

<span data-ttu-id="93698-207">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="93698-207">Asia/Yakutsk</span></span>

<span data-ttu-id="93698-208">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="93698-208">Pacific/Guadalcanal</span></span>

<span data-ttu-id="93698-209">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="93698-209">Asia/Vladivostok</span></span>

<span data-ttu-id="93698-210">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="93698-210">Pacific/Auckland</span></span>

<span data-ttu-id="93698-211">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="93698-211">Etc/GMT-12</span></span>

<span data-ttu-id="93698-212">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="93698-212">Pacific/Fiji</span></span>

<span data-ttu-id="93698-213">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="93698-213">Asia/Magadan</span></span>

<span data-ttu-id="93698-214">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="93698-214">Pacific/Tongatapu</span></span>

<span data-ttu-id="93698-215">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="93698-215">Pacific/Apia</span></span>

<span data-ttu-id="93698-216">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="93698-216">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="93698-217">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93698-217">JSON representation</span></span>

<span data-ttu-id="93698-218">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="93698-218">Here is a JSON representation of the resource</span></span>

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
