---
title: tipo de recurso dateTimeTimeZone
description: Descreve a data, a hora e o fuso horário de um ponto no tempo.
localization_priority: Normal
ms.openlocfilehash: ee5359c0ababad2a4f785d17a02ac5bb618d2681
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057040"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="68dec-103">tipo de recurso dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="68dec-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68dec-104">Descreve a data, a hora e o fuso horário de um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="68dec-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="68dec-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68dec-105">Properties</span></span>
| <span data-ttu-id="68dec-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68dec-106">Property</span></span>     | <span data-ttu-id="68dec-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="68dec-107">Type</span></span>   |<span data-ttu-id="68dec-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="68dec-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68dec-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="68dec-109">dateTime</span></span>|<span data-ttu-id="68dec-110">String</span><span class="sxs-lookup"><span data-stu-id="68dec-110">String</span></span>|<span data-ttu-id="68dec-111">Um único ponto de tempo em uma representação combinada de data e hora (`{date}T{time}`).</span><span class="sxs-lookup"><span data-stu-id="68dec-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="68dec-112">Por exemplo, "2019-04-16T09:00:00".</span><span class="sxs-lookup"><span data-stu-id="68dec-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="68dec-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="68dec-113">timeZone</span></span>|<span data-ttu-id="68dec-114">String</span><span class="sxs-lookup"><span data-stu-id="68dec-114">String</span></span>|<span data-ttu-id="68dec-115">Um nome de fuso horário, conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="68dec-115">A time zone name as described below.</span></span>|

<span data-ttu-id="68dec-116">A propriedade **timeZone** pode ser definida para qualquer um dos fusos horários com suporte no Windows, bem como os nomes de fusos horários a seguir.</span><span class="sxs-lookup"><span data-stu-id="68dec-116">The **timeZone** property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="68dec-117">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="68dec-117">Etc/GMT+12</span></span>

<span data-ttu-id="68dec-118">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="68dec-118">Etc/GMT+11</span></span>

<span data-ttu-id="68dec-119">Pacífico/Honolulu</span><span class="sxs-lookup"><span data-stu-id="68dec-119">Pacific/Honolulu</span></span>

<span data-ttu-id="68dec-120">América/Anchorage</span><span class="sxs-lookup"><span data-stu-id="68dec-120">America/Anchorage</span></span>

<span data-ttu-id="68dec-121">América/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="68dec-121">America/Santa_Isabel</span></span>

<span data-ttu-id="68dec-122">América/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="68dec-122">America/Los_Angeles</span></span>

<span data-ttu-id="68dec-123">América/Phoenix</span><span class="sxs-lookup"><span data-stu-id="68dec-123">America/Phoenix</span></span>

<span data-ttu-id="68dec-124">América/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="68dec-124">America/Chihuahua</span></span>

<span data-ttu-id="68dec-125">América/Denver</span><span class="sxs-lookup"><span data-stu-id="68dec-125">America/Denver</span></span>

<span data-ttu-id="68dec-126">América/Guatemala</span><span class="sxs-lookup"><span data-stu-id="68dec-126">America/Guatemala</span></span>

<span data-ttu-id="68dec-127">América/Chicago</span><span class="sxs-lookup"><span data-stu-id="68dec-127">America/Chicago</span></span>

<span data-ttu-id="68dec-128">América/Mexico_City</span><span class="sxs-lookup"><span data-stu-id="68dec-128">America/Mexico_City</span></span>

<span data-ttu-id="68dec-129">América/Regina</span><span class="sxs-lookup"><span data-stu-id="68dec-129">America/Regina</span></span>

<span data-ttu-id="68dec-130">América/Bogotá</span><span class="sxs-lookup"><span data-stu-id="68dec-130">America/Bogota</span></span>

<span data-ttu-id="68dec-131">América/New_York</span><span class="sxs-lookup"><span data-stu-id="68dec-131">America/New_York</span></span>

<span data-ttu-id="68dec-132">América/Indiana/Indianápolis</span><span class="sxs-lookup"><span data-stu-id="68dec-132">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="68dec-133">América/Caracas</span><span class="sxs-lookup"><span data-stu-id="68dec-133">America/Caracas</span></span>

<span data-ttu-id="68dec-134">América/Asunción</span><span class="sxs-lookup"><span data-stu-id="68dec-134">America/Asuncion</span></span>

<span data-ttu-id="68dec-135">América/Halifax</span><span class="sxs-lookup"><span data-stu-id="68dec-135">America/Halifax</span></span>

<span data-ttu-id="68dec-136">América/Cuiabá</span><span class="sxs-lookup"><span data-stu-id="68dec-136">America/Cuiaba</span></span>

<span data-ttu-id="68dec-137">América/La_Paz</span><span class="sxs-lookup"><span data-stu-id="68dec-137">America/La_Paz</span></span>

<span data-ttu-id="68dec-138">América/Santiago</span><span class="sxs-lookup"><span data-stu-id="68dec-138">America/Santiago</span></span>

<span data-ttu-id="68dec-139">América/St_Johns</span><span class="sxs-lookup"><span data-stu-id="68dec-139">America/St_Johns</span></span>

<span data-ttu-id="68dec-140">América/São_Paulo</span><span class="sxs-lookup"><span data-stu-id="68dec-140">America/Sao_Paulo</span></span>

<span data-ttu-id="68dec-141">América/Argentina/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="68dec-141">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="68dec-142">América/Cayenne</span><span class="sxs-lookup"><span data-stu-id="68dec-142">America/Cayenne</span></span>

<span data-ttu-id="68dec-143">América/Godthab</span><span class="sxs-lookup"><span data-stu-id="68dec-143">America/Godthab</span></span>

<span data-ttu-id="68dec-144">América/Montevidéu</span><span class="sxs-lookup"><span data-stu-id="68dec-144">America/Montevideo</span></span>

<span data-ttu-id="68dec-145">América/Bahia</span><span class="sxs-lookup"><span data-stu-id="68dec-145">America/Bahia</span></span>

<span data-ttu-id="68dec-146">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="68dec-146">Etc/GMT+2</span></span>

<span data-ttu-id="68dec-147">Atlântico/Açores</span><span class="sxs-lookup"><span data-stu-id="68dec-147">Atlantic/Azores</span></span>

<span data-ttu-id="68dec-148">Atlântico/Cape_Verde</span><span class="sxs-lookup"><span data-stu-id="68dec-148">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="68dec-149">África/Casablanca</span><span class="sxs-lookup"><span data-stu-id="68dec-149">Africa/Casablanca</span></span>

<span data-ttu-id="68dec-150">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="68dec-150">Etc/GMT</span></span>

<span data-ttu-id="68dec-151">Europa/Londres</span><span class="sxs-lookup"><span data-stu-id="68dec-151">Europe/London</span></span>

<span data-ttu-id="68dec-152">Atlântico/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="68dec-152">Atlantic/Reykjavik</span></span>

<span data-ttu-id="68dec-153">Europa/Berlim</span><span class="sxs-lookup"><span data-stu-id="68dec-153">Europe/Berlin</span></span>

<span data-ttu-id="68dec-154">Europa/Budapeste</span><span class="sxs-lookup"><span data-stu-id="68dec-154">Europe/Budapest</span></span>

<span data-ttu-id="68dec-155">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="68dec-155">Europe/Paris</span></span>

<span data-ttu-id="68dec-156">Europa/Varsóvia</span><span class="sxs-lookup"><span data-stu-id="68dec-156">Europe/Warsaw</span></span>

<span data-ttu-id="68dec-157">África/Lagos</span><span class="sxs-lookup"><span data-stu-id="68dec-157">Africa/Lagos</span></span>

<span data-ttu-id="68dec-158">África/Windhoek</span><span class="sxs-lookup"><span data-stu-id="68dec-158">Africa/Windhoek</span></span>

<span data-ttu-id="68dec-159">Europa/Bucareste</span><span class="sxs-lookup"><span data-stu-id="68dec-159">Europe/Bucharest</span></span>

<span data-ttu-id="68dec-160">Ásia/Beirute</span><span class="sxs-lookup"><span data-stu-id="68dec-160">Asia/Beirut</span></span>

<span data-ttu-id="68dec-161">África/Cairo</span><span class="sxs-lookup"><span data-stu-id="68dec-161">Africa/Cairo</span></span>

<span data-ttu-id="68dec-162">Ásia/Damasco</span><span class="sxs-lookup"><span data-stu-id="68dec-162">Asia/Damascus</span></span>

<span data-ttu-id="68dec-163">África/Joanesburgo</span><span class="sxs-lookup"><span data-stu-id="68dec-163">Africa/Johannesburg</span></span>

<span data-ttu-id="68dec-164">Europa/Kiev (Kiev)</span><span class="sxs-lookup"><span data-stu-id="68dec-164">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="68dec-165">Europa/Istambul</span><span class="sxs-lookup"><span data-stu-id="68dec-165">Europe/Istanbul</span></span>

<span data-ttu-id="68dec-166">Ásia/Jerusalém</span><span class="sxs-lookup"><span data-stu-id="68dec-166">Asia/Jerusalem</span></span>

<span data-ttu-id="68dec-167">Ásia/Amman</span><span class="sxs-lookup"><span data-stu-id="68dec-167">Asia/Amman</span></span>

<span data-ttu-id="68dec-168">Ásia/Bagdá</span><span class="sxs-lookup"><span data-stu-id="68dec-168">Asia/Baghdad</span></span>

<span data-ttu-id="68dec-169">Europa/Caliningrado</span><span class="sxs-lookup"><span data-stu-id="68dec-169">Europe/Kaliningrad</span></span>

<span data-ttu-id="68dec-170">Ásia/Riad</span><span class="sxs-lookup"><span data-stu-id="68dec-170">Asia/Riyadh</span></span>

<span data-ttu-id="68dec-171">África/Nairóbi</span><span class="sxs-lookup"><span data-stu-id="68dec-171">Africa/Nairobi</span></span>

<span data-ttu-id="68dec-172">Ásia/Teerã</span><span class="sxs-lookup"><span data-stu-id="68dec-172">Asia/Tehran</span></span>

<span data-ttu-id="68dec-173">Ásia/Dubai</span><span class="sxs-lookup"><span data-stu-id="68dec-173">Asia/Dubai</span></span>

<span data-ttu-id="68dec-174">Ásia/Baku</span><span class="sxs-lookup"><span data-stu-id="68dec-174">Asia/Baku</span></span>

<span data-ttu-id="68dec-175">Europa/Moscou</span><span class="sxs-lookup"><span data-stu-id="68dec-175">Europe/Moscow</span></span>

<span data-ttu-id="68dec-176">Índia/Maurício</span><span class="sxs-lookup"><span data-stu-id="68dec-176">Indian/Mauritius</span></span>

<span data-ttu-id="68dec-177">Ásia/Tbilisi</span><span class="sxs-lookup"><span data-stu-id="68dec-177">Asia/Tbilisi</span></span>

<span data-ttu-id="68dec-178">Ásia/Ierevan</span><span class="sxs-lookup"><span data-stu-id="68dec-178">Asia/Yerevan</span></span>

<span data-ttu-id="68dec-179">Ásia/Cabul</span><span class="sxs-lookup"><span data-stu-id="68dec-179">Asia/Kabul</span></span>

<span data-ttu-id="68dec-180">Ásia/Karachi</span><span class="sxs-lookup"><span data-stu-id="68dec-180">Asia/Karachi</span></span>

<span data-ttu-id="68dec-181">Ásia/Toshkent (Tashkent)</span><span class="sxs-lookup"><span data-stu-id="68dec-181">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="68dec-182">Ásia/Kolkata (Calcutá)</span><span class="sxs-lookup"><span data-stu-id="68dec-182">Asia/Kolkata</span></span>

<span data-ttu-id="68dec-183">Ásia/Colombo</span><span class="sxs-lookup"><span data-stu-id="68dec-183">Asia/Colombo</span></span>

<span data-ttu-id="68dec-184">Ásia/Katmandu</span><span class="sxs-lookup"><span data-stu-id="68dec-184">Asia/Kathmandu</span></span>

<span data-ttu-id="68dec-185">Ásia/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="68dec-185">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="68dec-186">Ásia/Dacca</span><span class="sxs-lookup"><span data-stu-id="68dec-186">Asia/Dhaka</span></span>

<span data-ttu-id="68dec-187">Ásia/Ecaterimburgo</span><span class="sxs-lookup"><span data-stu-id="68dec-187">Asia/Yekaterinburg</span></span>

<span data-ttu-id="68dec-188">Ásia/Yakutsk (Yangon)</span><span class="sxs-lookup"><span data-stu-id="68dec-188">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="68dec-189">Ásia/Bangcoc</span><span class="sxs-lookup"><span data-stu-id="68dec-189">Asia/Bangkok</span></span>

<span data-ttu-id="68dec-190">Ásia/Novosibirsk</span><span class="sxs-lookup"><span data-stu-id="68dec-190">Asia/Novosibirsk</span></span>

<span data-ttu-id="68dec-191">Ásia/Shanghai</span><span class="sxs-lookup"><span data-stu-id="68dec-191">Asia/Shanghai</span></span>

<span data-ttu-id="68dec-192">Ásia/Krasnoyarsk</span><span class="sxs-lookup"><span data-stu-id="68dec-192">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="68dec-193">Ásia/Cingapura</span><span class="sxs-lookup"><span data-stu-id="68dec-193">Asia/Singapore</span></span>

<span data-ttu-id="68dec-194">Austrália/Perth</span><span class="sxs-lookup"><span data-stu-id="68dec-194">Australia/Perth</span></span>

<span data-ttu-id="68dec-195">Ásia/Taipé</span><span class="sxs-lookup"><span data-stu-id="68dec-195">Asia/Taipei</span></span>

<span data-ttu-id="68dec-196">Ásia/Ulan Bator</span><span class="sxs-lookup"><span data-stu-id="68dec-196">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="68dec-197">Ásia/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="68dec-197">Asia/Irkutsk</span></span>

<span data-ttu-id="68dec-198">Ásia/Tóquio</span><span class="sxs-lookup"><span data-stu-id="68dec-198">Asia/Tokyo</span></span>

<span data-ttu-id="68dec-199">Ásia/Seul</span><span class="sxs-lookup"><span data-stu-id="68dec-199">Asia/Seoul</span></span>

<span data-ttu-id="68dec-200">Austrália/Adelaide</span><span class="sxs-lookup"><span data-stu-id="68dec-200">Australia/Adelaide</span></span>

<span data-ttu-id="68dec-201">Austrália/Darwin</span><span class="sxs-lookup"><span data-stu-id="68dec-201">Australia/Darwin</span></span>

<span data-ttu-id="68dec-202">Austrália/Brisbane</span><span class="sxs-lookup"><span data-stu-id="68dec-202">Australia/Brisbane</span></span>

<span data-ttu-id="68dec-203">Austrália/Sidney</span><span class="sxs-lookup"><span data-stu-id="68dec-203">Australia/Sydney</span></span>

<span data-ttu-id="68dec-204">Pacífico/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="68dec-204">Pacific/Port_Moresby</span></span>

<span data-ttu-id="68dec-205">Austrália/Hobart</span><span class="sxs-lookup"><span data-stu-id="68dec-205">Australia/Hobart</span></span>

<span data-ttu-id="68dec-206">Ásia/Yakutsk</span><span class="sxs-lookup"><span data-stu-id="68dec-206">Asia/Yakutsk</span></span>

<span data-ttu-id="68dec-207">Pacífico/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="68dec-207">Pacific/Guadalcanal</span></span>

<span data-ttu-id="68dec-208">Ásia/Vladivostok</span><span class="sxs-lookup"><span data-stu-id="68dec-208">Asia/Vladivostok</span></span>

<span data-ttu-id="68dec-209">Pacífico/Auckland</span><span class="sxs-lookup"><span data-stu-id="68dec-209">Pacific/Auckland</span></span>

<span data-ttu-id="68dec-210">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="68dec-210">Etc/GMT-12</span></span>

<span data-ttu-id="68dec-211">Pacífico/Fiji</span><span class="sxs-lookup"><span data-stu-id="68dec-211">Pacific/Fiji</span></span>

<span data-ttu-id="68dec-212">Ásia/Magadã</span><span class="sxs-lookup"><span data-stu-id="68dec-212">Asia/Magadan</span></span>

<span data-ttu-id="68dec-213">Pacífico/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="68dec-213">Pacific/Tongatapu</span></span>

<span data-ttu-id="68dec-214">Pacífico/Apia</span><span class="sxs-lookup"><span data-stu-id="68dec-214">Pacific/Apia</span></span>

<span data-ttu-id="68dec-215">Pacífico/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="68dec-215">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="68dec-216">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68dec-216">JSON representation</span></span>

<span data-ttu-id="68dec-217">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="68dec-217">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimetimezone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
