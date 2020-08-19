---
title: Tipo de recurso customTimeZone
description: Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 438e9ccf93899c6024eaf9dfb16cc0a6b1d61f5f
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809820"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="93145-103">Tipo de recurso customTimeZone</span><span class="sxs-lookup"><span data-stu-id="93145-103">customTimeZone resource type</span></span>

<span data-ttu-id="93145-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93145-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93145-105">Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.</span><span class="sxs-lookup"><span data-stu-id="93145-105">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="93145-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93145-106">Properties</span></span>
| <span data-ttu-id="93145-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93145-107">Property</span></span>     | <span data-ttu-id="93145-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="93145-108">Type</span></span>   |<span data-ttu-id="93145-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="93145-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="93145-110">bias</span><span class="sxs-lookup"><span data-stu-id="93145-110">bias</span></span> | <span data-ttu-id="93145-111">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="93145-111">Edm.Int32</span></span> | <span data-ttu-id="93145-112">A diferença de tempo em relação ao fuso horário UTC (Tempo Universal Coordenado).</span><span class="sxs-lookup"><span data-stu-id="93145-112">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="93145-113">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="93145-113">This value is in minutes.</span></span><span data-ttu-id="93145-114">Os fusos horários que estão adiantados em relação ao UTC têm uma diferença de tempo positiva, enquanto os atrasados têm uma diferença de tempo negativa.</span><span class="sxs-lookup"><span data-stu-id="93145-114"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="93145-115">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="93145-115">daylightOffset</span></span> | [<span data-ttu-id="93145-116">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="93145-116">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="93145-117">Especifica quando o fuso horário muda do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="93145-117">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="93145-118">nome</span><span class="sxs-lookup"><span data-stu-id="93145-118">name</span></span> | <span data-ttu-id="93145-119">string</span><span class="sxs-lookup"><span data-stu-id="93145-119">string</span></span> | <span data-ttu-id="93145-120">O nome do fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="93145-120">The name of the custom time zone.</span></span> |
| <span data-ttu-id="93145-121">standardOffset</span><span class="sxs-lookup"><span data-stu-id="93145-121">standardOffset</span></span> | [<span data-ttu-id="93145-122">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="93145-122">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="93145-123">Especifica quando o fuso horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="93145-123">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="93145-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93145-124">JSON representation</span></span>

<span data-ttu-id="93145-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93145-125">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
