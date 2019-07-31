---
title: tipo de recurso timeOffItem
description: Representa uma versão do timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 6b240f587e20e2da178f9afa3e8d712cf2ae114d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964302"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="b911f-103">tipo de recurso timeOffItem</span><span class="sxs-lookup"><span data-stu-id="b911f-103">timeOffItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b911f-104">Representa uma versão do [timeOff](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="b911f-104">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b911f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b911f-105">Properties</span></span>
| <span data-ttu-id="b911f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b911f-106">Property</span></span>                         | <span data-ttu-id="b911f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b911f-107">Type</span></span>                    | <span data-ttu-id="b911f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b911f-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="b911f-109">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="b911f-109">timeOffReasonId</span></span>               | <span data-ttu-id="b911f-110">string</span><span class="sxs-lookup"><span data-stu-id="b911f-110">string</span></span>                  | <span data-ttu-id="b911f-111">ID do `timeOffReason` para isso `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="b911f-111">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="b911f-112">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b911f-112">Required.</span></span>     |
| <span data-ttu-id="b911f-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b911f-113">startDateTime</span></span>               | <span data-ttu-id="b911f-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b911f-114">DateTimeOffset</span></span>                  | <span data-ttu-id="b911f-115">A data e a hora de início `timeOffItem`para o.</span><span class="sxs-lookup"><span data-stu-id="b911f-115">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="b911f-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b911f-116">Required.</span></span> <span data-ttu-id="b911f-117">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b911f-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b911f-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="b911f-118">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b911f-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b911f-119">endDateTime</span></span>               | <span data-ttu-id="b911f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b911f-120">DateTimeOffset</span></span>                  | <span data-ttu-id="b911f-121">A data e a hora de término `timeOffItem`para o.</span><span class="sxs-lookup"><span data-stu-id="b911f-121">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="b911f-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b911f-122">Required.</span></span> <span data-ttu-id="b911f-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b911f-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b911f-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="b911f-124">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b911f-125">tema</span><span class="sxs-lookup"><span data-stu-id="b911f-125">theme</span></span> | <span data-ttu-id="b911f-126">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="b911f-126">scheduleEntityTheme</span></span>   | <span data-ttu-id="b911f-127">Cores suportadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="b911f-127">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b911f-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b911f-128">JSON representation</span></span>

<span data-ttu-id="b911f-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b911f-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "pink"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
