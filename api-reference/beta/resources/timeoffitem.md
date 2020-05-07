---
title: tipo de recurso timeOffItem
description: Representa uma versão do timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3fcd7c0e046cb9ae3df9ea371329058fa0472fc3
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154385"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="9e11b-103">tipo de recurso timeOffItem</span><span class="sxs-lookup"><span data-stu-id="9e11b-103">timeOffItem resource type</span></span>

<span data-ttu-id="9e11b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e11b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e11b-105">Representa uma versão do [timeOff](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="9e11b-105">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9e11b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e11b-106">Properties</span></span>
| <span data-ttu-id="9e11b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e11b-107">Property</span></span>                         | <span data-ttu-id="9e11b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e11b-108">Type</span></span>                    | <span data-ttu-id="9e11b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e11b-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="9e11b-110">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="9e11b-110">timeOffReasonId</span></span>               | <span data-ttu-id="9e11b-111">string</span><span class="sxs-lookup"><span data-stu-id="9e11b-111">string</span></span>                  | <span data-ttu-id="9e11b-112">ID do `timeOffReason` para isso `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="9e11b-112">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="9e11b-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e11b-113">Required.</span></span>     |
| <span data-ttu-id="9e11b-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9e11b-114">startDateTime</span></span>               | <span data-ttu-id="9e11b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e11b-115">DateTimeOffset</span></span>                  | <span data-ttu-id="9e11b-116">A data e a hora de início `timeOffItem`para o.</span><span class="sxs-lookup"><span data-stu-id="9e11b-116">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="9e11b-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e11b-117">Required.</span></span> <span data-ttu-id="9e11b-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9e11b-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e11b-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="9e11b-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="9e11b-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9e11b-120">endDateTime</span></span>               | <span data-ttu-id="9e11b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e11b-121">DateTimeOffset</span></span>                  | <span data-ttu-id="9e11b-122">A data e a hora de término `timeOffItem`para o.</span><span class="sxs-lookup"><span data-stu-id="9e11b-122">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="9e11b-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e11b-123">Required.</span></span> <span data-ttu-id="9e11b-124">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9e11b-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e11b-125">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="9e11b-125">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="9e11b-126">tema</span><span class="sxs-lookup"><span data-stu-id="9e11b-126">theme</span></span> | <span data-ttu-id="9e11b-127">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="9e11b-127">scheduleEntityTheme</span></span>   | <span data-ttu-id="9e11b-128">Cores suportadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="9e11b-128">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9e11b-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e11b-129">JSON representation</span></span>

<span data-ttu-id="9e11b-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e11b-130">Here is a JSON representation of the resource.</span></span>

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
