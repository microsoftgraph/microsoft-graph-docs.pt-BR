---
title: tipo de recurso shiftItem
description: Um shiftItem representa uma versão do turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5b86f232d5d5c6c41c2eab873e992b2b9902c976
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154336"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="6d9e4-103">tipo de recurso shiftItem</span><span class="sxs-lookup"><span data-stu-id="6d9e4-103">shiftItem resource type</span></span>

<span data-ttu-id="6d9e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d9e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d9e4-105">Representa uma versão de um [turno](shift.md).</span><span class="sxs-lookup"><span data-stu-id="6d9e4-105">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6d9e4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d9e4-106">Properties</span></span>
| <span data-ttu-id="6d9e4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d9e4-107">Property</span></span>                         | <span data-ttu-id="6d9e4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d9e4-108">Type</span></span>                    | <span data-ttu-id="6d9e4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d9e4-109">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="6d9e4-110">notes</span><span class="sxs-lookup"><span data-stu-id="6d9e4-110">notes</span></span>               | <span data-ttu-id="6d9e4-111">string</span><span class="sxs-lookup"><span data-stu-id="6d9e4-111">string</span></span>                  | <span data-ttu-id="6d9e4-112">As notas de alternância para `shiftItem`o.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-112">The shift notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="6d9e4-113">displayName</span><span class="sxs-lookup"><span data-stu-id="6d9e4-113">displayName</span></span>               | <span data-ttu-id="6d9e4-114">string</span><span class="sxs-lookup"><span data-stu-id="6d9e4-114">string</span></span>                  | <span data-ttu-id="6d9e4-115">O rótulo Shift do `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-115">The shift label of the `shiftItem`.</span></span> |
| <span data-ttu-id="6d9e4-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6d9e4-116">startDateTime</span></span>               | <span data-ttu-id="6d9e4-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d9e4-117">DateTimeOffset</span></span>                  | <span data-ttu-id="6d9e4-118">A data e a hora de início `shiftItem`para o.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-118">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="6d9e4-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d9e4-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="6d9e4-121">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-121">Required.</span></span> |
| <span data-ttu-id="6d9e4-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6d9e4-122">endDateTime</span></span>               | <span data-ttu-id="6d9e4-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d9e4-123">DateTimeOffset</span></span>                 | <span data-ttu-id="6d9e4-124">A data e a hora de término `shiftItem`para o.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-124">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="6d9e4-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-125">Required.</span></span> <span data-ttu-id="6d9e4-126">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d9e4-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-127">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="6d9e4-128">tema</span><span class="sxs-lookup"><span data-stu-id="6d9e4-128">theme</span></span> | <span data-ttu-id="6d9e4-129">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="6d9e4-129">scheduleEntityTheme</span></span>   |  <span data-ttu-id="6d9e4-130">Cores suportadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-130">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="6d9e4-131">activities</span><span class="sxs-lookup"><span data-stu-id="6d9e4-131">activities</span></span>    | <span data-ttu-id="6d9e4-132">coleção [shiftActivity](shiftactivity.md)</span><span class="sxs-lookup"><span data-stu-id="6d9e4-132">[shiftActivity](shiftactivity.md) collection</span></span>   | <span data-ttu-id="6d9e4-133">Uma parte incremental de um turno que pode abranger detalhes de quando e onde um funcionário está durante o turno.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-133">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="6d9e4-134">Por exemplo, uma atribuição ou uma quebra ou almoço agendado.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-134">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="6d9e4-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-135">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d9e4-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d9e4-136">JSON representation</span></span>

<span data-ttu-id="6d9e4-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d9e4-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "String",
  "notes": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "activities": [{"@odata.type": "microsoft.graph.shiftActivity"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
