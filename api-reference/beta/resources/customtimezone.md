---
title: Tipo de recurso customTimeZone
description: Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.
ms.openlocfilehash: 83375c96e4247cb0ddf2d17b1bede2c295f0b27f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033248"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="3cfb7-103">Tipo de recurso customTimeZone</span><span class="sxs-lookup"><span data-stu-id="3cfb7-103">customTimeZone resource type</span></span>

> <span data-ttu-id="3cfb7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3cfb7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3cfb7-106">Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-106">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="3cfb7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3cfb7-107">Properties</span></span>
| <span data-ttu-id="3cfb7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cfb7-108">Property</span></span>     | <span data-ttu-id="3cfb7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cfb7-109">Type</span></span>   |<span data-ttu-id="3cfb7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cfb7-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3cfb7-111">bias</span><span class="sxs-lookup"><span data-stu-id="3cfb7-111">bias</span></span> | <span data-ttu-id="3cfb7-112">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="3cfb7-112">Edm.Int32</span></span> | <span data-ttu-id="3cfb7-113">A diferença de tempo em relação ao fuso horário UTC (Tempo Universal Coordenado).</span><span class="sxs-lookup"><span data-stu-id="3cfb7-113">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="3cfb7-114">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-114">This value is in minutes.</span></span><span data-ttu-id="3cfb7-115">Os fusos horários que estão adiantados em relação ao UTC têm uma diferença de tempo positiva, enquanto os atrasados têm uma diferença de tempo negativa.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-115"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="3cfb7-116">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="3cfb7-116">daylightOffset</span></span> | [<span data-ttu-id="3cfb7-117">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="3cfb7-117">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="3cfb7-118">Especifica quando o fuso horário muda do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-118">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="3cfb7-119">name</span><span class="sxs-lookup"><span data-stu-id="3cfb7-119">name</span></span> | <span data-ttu-id="3cfb7-120">string</span><span class="sxs-lookup"><span data-stu-id="3cfb7-120">string</span></span> | <span data-ttu-id="3cfb7-121">O nome do fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-121">The name of the custom time zone.</span></span> |
| <span data-ttu-id="3cfb7-122">standardOffset</span><span class="sxs-lookup"><span data-stu-id="3cfb7-122">standardOffset</span></span> | [<span data-ttu-id="3cfb7-123">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="3cfb7-123">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="3cfb7-124">Especifica quando o fuso horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-124">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3cfb7-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3cfb7-125">JSON representation</span></span>

<span data-ttu-id="3cfb7-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3cfb7-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->