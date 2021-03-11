---
title: Tipo de recurso shiftItem
description: Um shiftItem representa uma versão do shift.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3998176fbd001e1136a107dd3aa53ff8442fe8f3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721108"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="4eecc-103">Tipo de recurso shiftItem</span><span class="sxs-lookup"><span data-stu-id="4eecc-103">shiftItem resource type</span></span>

<span data-ttu-id="4eecc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eecc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eecc-105">Representa uma versão de um [turno](shift.md).</span><span class="sxs-lookup"><span data-stu-id="4eecc-105">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4eecc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4eecc-106">Properties</span></span>
| <span data-ttu-id="4eecc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4eecc-107">Property</span></span>                         | <span data-ttu-id="4eecc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4eecc-108">Type</span></span>                    | <span data-ttu-id="4eecc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eecc-109">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="4eecc-110">notes</span><span class="sxs-lookup"><span data-stu-id="4eecc-110">notes</span></span>               | <span data-ttu-id="4eecc-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4eecc-111">string</span></span>                  | <span data-ttu-id="4eecc-112">As notas de turno para `shiftItem` o .</span><span class="sxs-lookup"><span data-stu-id="4eecc-112">The shift notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="4eecc-113">displayName</span><span class="sxs-lookup"><span data-stu-id="4eecc-113">displayName</span></span>               | <span data-ttu-id="4eecc-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4eecc-114">string</span></span>                  | <span data-ttu-id="4eecc-115">O rótulo de turno do `shiftItem` .</span><span class="sxs-lookup"><span data-stu-id="4eecc-115">The shift label of the `shiftItem`.</span></span> |
| <span data-ttu-id="4eecc-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4eecc-116">startDateTime</span></span>               | <span data-ttu-id="4eecc-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eecc-117">DateTimeOffset</span></span>                  | <span data-ttu-id="4eecc-118">A data e a hora de início do `shiftItem` .</span><span class="sxs-lookup"><span data-stu-id="4eecc-118">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="4eecc-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4eecc-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4eecc-120">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4eecc-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="4eecc-121">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4eecc-121">Required.</span></span> |
| <span data-ttu-id="4eecc-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4eecc-122">endDateTime</span></span>               | <span data-ttu-id="4eecc-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eecc-123">DateTimeOffset</span></span>                 | <span data-ttu-id="4eecc-124">A data e a hora de término do `shiftItem` .</span><span class="sxs-lookup"><span data-stu-id="4eecc-124">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="4eecc-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4eecc-125">Required.</span></span> <span data-ttu-id="4eecc-126">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4eecc-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4eecc-127">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4eecc-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="4eecc-128">tema</span><span class="sxs-lookup"><span data-stu-id="4eecc-128">theme</span></span> | <span data-ttu-id="4eecc-129">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="4eecc-129">scheduleEntityTheme</span></span>   |  <span data-ttu-id="4eecc-130">Cores com suporte: branco; azul; verde; roxo; rosa; amarelo; cinza; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="4eecc-130">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="4eecc-131">activities</span><span class="sxs-lookup"><span data-stu-id="4eecc-131">activities</span></span>    | <span data-ttu-id="4eecc-132">[Coleção shiftActivity](shiftactivity.md)</span><span class="sxs-lookup"><span data-stu-id="4eecc-132">[shiftActivity](shiftactivity.md) collection</span></span>   | <span data-ttu-id="4eecc-133">Uma parte incremental de um turno que pode abranger detalhes de quando e onde um funcionário está durante o turno.</span><span class="sxs-lookup"><span data-stu-id="4eecc-133">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="4eecc-134">Por exemplo, uma atribuição ou uma pausa ou almoço agendado.</span><span class="sxs-lookup"><span data-stu-id="4eecc-134">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="4eecc-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4eecc-135">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4eecc-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4eecc-136">JSON representation</span></span>

<span data-ttu-id="4eecc-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4eecc-137">Here is a JSON representation of the resource.</span></span>

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


