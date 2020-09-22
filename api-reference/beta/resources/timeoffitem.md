---
title: tipo de recurso timeOffItem
description: Representa uma versão do timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 166f1fe569301f6c2805867ff85b3c6354377128
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075487"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="e75f4-103">tipo de recurso timeOffItem</span><span class="sxs-lookup"><span data-stu-id="e75f4-103">timeOffItem resource type</span></span>

<span data-ttu-id="e75f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e75f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e75f4-105">Representa uma versão do [timeOff](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="e75f4-105">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e75f4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e75f4-106">Properties</span></span>
| <span data-ttu-id="e75f4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e75f4-107">Property</span></span>                         | <span data-ttu-id="e75f4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e75f4-108">Type</span></span>                    | <span data-ttu-id="e75f4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e75f4-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="e75f4-110">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="e75f4-110">timeOffReasonId</span></span>               | <span data-ttu-id="e75f4-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e75f4-111">string</span></span>                  | <span data-ttu-id="e75f4-112">ID do `timeOffReason` para isso `timeOffItem` .</span><span class="sxs-lookup"><span data-stu-id="e75f4-112">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="e75f4-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e75f4-113">Required.</span></span>     |
| <span data-ttu-id="e75f4-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e75f4-114">startDateTime</span></span>               | <span data-ttu-id="e75f4-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e75f4-115">DateTimeOffset</span></span>                  | <span data-ttu-id="e75f4-116">A data e a hora de início para o `timeOffItem` .</span><span class="sxs-lookup"><span data-stu-id="e75f4-116">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="e75f4-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e75f4-117">Required.</span></span> <span data-ttu-id="e75f4-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e75f4-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e75f4-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="e75f4-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="e75f4-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e75f4-120">endDateTime</span></span>               | <span data-ttu-id="e75f4-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e75f4-121">DateTimeOffset</span></span>                  | <span data-ttu-id="e75f4-122">A data e a hora de término para o `timeOffItem` .</span><span class="sxs-lookup"><span data-stu-id="e75f4-122">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="e75f4-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e75f4-123">Required.</span></span> <span data-ttu-id="e75f4-124">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e75f4-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e75f4-125">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="e75f4-125">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="e75f4-126">tema</span><span class="sxs-lookup"><span data-stu-id="e75f4-126">theme</span></span> | <span data-ttu-id="e75f4-127">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="e75f4-127">scheduleEntityTheme</span></span>   | <span data-ttu-id="e75f4-128">Cores suportadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="e75f4-128">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e75f4-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e75f4-129">JSON representation</span></span>

<span data-ttu-id="e75f4-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e75f4-130">Here is a JSON representation of the resource.</span></span>

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


