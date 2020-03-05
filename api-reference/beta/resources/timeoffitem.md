---
title: tipo de recurso timeOffItem
description: Representa uma versão do timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 019bb366ad9d960fd2eff6365ef987f186a0d6c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519726"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="c096f-103">tipo de recurso timeOffItem</span><span class="sxs-lookup"><span data-stu-id="c096f-103">timeOffItem resource type</span></span>

<span data-ttu-id="c096f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c096f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c096f-105">Representa uma versão do [timeOff](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="c096f-105">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c096f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c096f-106">Properties</span></span>
| <span data-ttu-id="c096f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c096f-107">Property</span></span>                         | <span data-ttu-id="c096f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c096f-108">Type</span></span>                    | <span data-ttu-id="c096f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c096f-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="c096f-110">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="c096f-110">timeOffReasonId</span></span>               | <span data-ttu-id="c096f-111">string</span><span class="sxs-lookup"><span data-stu-id="c096f-111">string</span></span>                  | <span data-ttu-id="c096f-112">ID do `timeOffReason` para isso `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="c096f-112">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="c096f-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c096f-113">Required.</span></span>     |
| <span data-ttu-id="c096f-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c096f-114">startDateTime</span></span>               | <span data-ttu-id="c096f-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c096f-115">DateTimeOffset</span></span>                  | <span data-ttu-id="c096f-116">A data e a hora de início `timeOffItem`para o.</span><span class="sxs-lookup"><span data-stu-id="c096f-116">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="c096f-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c096f-117">Required.</span></span> <span data-ttu-id="c096f-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c096f-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c096f-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="c096f-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="c096f-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c096f-120">endDateTime</span></span>               | <span data-ttu-id="c096f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c096f-121">DateTimeOffset</span></span>                  | <span data-ttu-id="c096f-122">A data e a hora de término `timeOffItem`para o.</span><span class="sxs-lookup"><span data-stu-id="c096f-122">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="c096f-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c096f-123">Required.</span></span> <span data-ttu-id="c096f-124">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c096f-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c096f-125">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="c096f-125">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="c096f-126">tema</span><span class="sxs-lookup"><span data-stu-id="c096f-126">theme</span></span> | <span data-ttu-id="c096f-127">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="c096f-127">scheduleEntityTheme</span></span>   | <span data-ttu-id="c096f-128">Cores suportadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="c096f-128">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c096f-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c096f-129">JSON representation</span></span>

<span data-ttu-id="c096f-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c096f-130">Here is a JSON representation of the resource.</span></span>

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
