---
title: Tipo de recurso customTimeZone
description: Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.
localization_priority: Normal
ms.openlocfilehash: 0bb961e213956ef3142df1f3d55a83918a14fa78
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515248"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="a920c-103">Tipo de recurso customTimeZone</span><span class="sxs-lookup"><span data-stu-id="a920c-103">customTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a920c-104">Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.</span><span class="sxs-lookup"><span data-stu-id="a920c-104">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="a920c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a920c-105">Properties</span></span>
| <span data-ttu-id="a920c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a920c-106">Property</span></span>     | <span data-ttu-id="a920c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a920c-107">Type</span></span>   |<span data-ttu-id="a920c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a920c-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a920c-109">bias</span><span class="sxs-lookup"><span data-stu-id="a920c-109">bias</span></span> | <span data-ttu-id="a920c-110">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="a920c-110">Edm.Int32</span></span> | <span data-ttu-id="a920c-111">A diferença de tempo em relação ao fuso horário UTC (Tempo Universal Coordenado).</span><span class="sxs-lookup"><span data-stu-id="a920c-111">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="a920c-112">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="a920c-112">This value is in minutes.</span></span><span data-ttu-id="a920c-113">Os fusos horários que estão adiantados em relação ao UTC têm uma diferença de tempo positiva, enquanto os atrasados têm uma diferença de tempo negativa.</span><span class="sxs-lookup"><span data-stu-id="a920c-113"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="a920c-114">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="a920c-114">daylightOffset</span></span> | [<span data-ttu-id="a920c-115">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="a920c-115">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="a920c-116">Especifica quando o fuso horário muda do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="a920c-116">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="a920c-117">name</span><span class="sxs-lookup"><span data-stu-id="a920c-117">name</span></span> | <span data-ttu-id="a920c-118">string</span><span class="sxs-lookup"><span data-stu-id="a920c-118">string</span></span> | <span data-ttu-id="a920c-119">O nome do fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="a920c-119">The name of the custom time zone.</span></span> |
| <span data-ttu-id="a920c-120">standardOffset</span><span class="sxs-lookup"><span data-stu-id="a920c-120">standardOffset</span></span> | [<span data-ttu-id="a920c-121">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="a920c-121">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="a920c-122">Especifica quando o fuso horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="a920c-122">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a920c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a920c-123">JSON representation</span></span>

<span data-ttu-id="a920c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a920c-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/customtimezone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
