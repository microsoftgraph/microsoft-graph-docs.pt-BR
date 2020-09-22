---
title: tipo de recurso shiftItem
description: Um shiftItem representa uma versão do turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7b1522ee4b1819b168d5e261a5e8a53138a69ea4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036965"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="7c412-103">tipo de recurso shiftItem</span><span class="sxs-lookup"><span data-stu-id="7c412-103">shiftItem resource type</span></span>

<span data-ttu-id="7c412-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c412-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c412-105">Representa uma versão de um [turno](shift.md).</span><span class="sxs-lookup"><span data-stu-id="7c412-105">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7c412-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c412-106">Properties</span></span>
| <span data-ttu-id="7c412-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c412-107">Property</span></span>                         | <span data-ttu-id="7c412-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c412-108">Type</span></span>                    | <span data-ttu-id="7c412-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c412-109">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="7c412-110">notes</span><span class="sxs-lookup"><span data-stu-id="7c412-110">notes</span></span>               | <span data-ttu-id="7c412-111">string</span><span class="sxs-lookup"><span data-stu-id="7c412-111">string</span></span>                  | <span data-ttu-id="7c412-112">As notas de alternância para o `shiftItem` .</span><span class="sxs-lookup"><span data-stu-id="7c412-112">The shift notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="7c412-113">displayName</span><span class="sxs-lookup"><span data-stu-id="7c412-113">displayName</span></span>               | <span data-ttu-id="7c412-114">string</span><span class="sxs-lookup"><span data-stu-id="7c412-114">string</span></span>                  | <span data-ttu-id="7c412-115">O rótulo Shift do `shiftItem` .</span><span class="sxs-lookup"><span data-stu-id="7c412-115">The shift label of the `shiftItem`.</span></span> |
| <span data-ttu-id="7c412-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7c412-116">startDateTime</span></span>               | <span data-ttu-id="7c412-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c412-117">DateTimeOffset</span></span>                  | <span data-ttu-id="7c412-118">A data e a hora de início para o `shiftItem` .</span><span class="sxs-lookup"><span data-stu-id="7c412-118">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="7c412-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7c412-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7c412-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="7c412-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="7c412-121">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c412-121">Required.</span></span> |
| <span data-ttu-id="7c412-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7c412-122">endDateTime</span></span>               | <span data-ttu-id="7c412-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c412-123">DateTimeOffset</span></span>                 | <span data-ttu-id="7c412-124">A data e a hora de término para o `shiftItem` .</span><span class="sxs-lookup"><span data-stu-id="7c412-124">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="7c412-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c412-125">Required.</span></span> <span data-ttu-id="7c412-126">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7c412-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7c412-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="7c412-127">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="7c412-128">tema</span><span class="sxs-lookup"><span data-stu-id="7c412-128">theme</span></span> | <span data-ttu-id="7c412-129">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="7c412-129">scheduleEntityTheme</span></span>   |  <span data-ttu-id="7c412-130">Cores suportadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="7c412-130">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="7c412-131">activities</span><span class="sxs-lookup"><span data-stu-id="7c412-131">activities</span></span>    | <span data-ttu-id="7c412-132">coleção [shiftActivity](shiftactivity.md)</span><span class="sxs-lookup"><span data-stu-id="7c412-132">[shiftActivity](shiftactivity.md) collection</span></span>   | <span data-ttu-id="7c412-133">Uma parte incremental de um turno que pode abranger detalhes de quando e onde um funcionário está durante o turno.</span><span class="sxs-lookup"><span data-stu-id="7c412-133">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="7c412-134">Por exemplo, uma atribuição ou uma quebra ou almoço agendado.</span><span class="sxs-lookup"><span data-stu-id="7c412-134">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="7c412-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c412-135">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7c412-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c412-136">JSON representation</span></span>

<span data-ttu-id="7c412-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c412-137">Here is a JSON representation of the resource.</span></span>

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

