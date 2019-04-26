---
title: tipo de recurso shiftItem
description: Um shiftItem representa uma versão do turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd5b3d224e60fc3f21b4d484952c7a2643b02407
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343035"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="88273-103">tipo de recurso shiftItem</span><span class="sxs-lookup"><span data-stu-id="88273-103">shiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88273-104">Representa uma versão de um [turno](shift.md).</span><span class="sxs-lookup"><span data-stu-id="88273-104">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="88273-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88273-105">Properties</span></span>
| <span data-ttu-id="88273-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88273-106">Property</span></span>                         | <span data-ttu-id="88273-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="88273-107">Type</span></span>                    | <span data-ttu-id="88273-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="88273-108">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="88273-109">notes</span><span class="sxs-lookup"><span data-stu-id="88273-109">notes</span></span>               | <span data-ttu-id="88273-110">string</span><span class="sxs-lookup"><span data-stu-id="88273-110">string</span></span>                  | <span data-ttu-id="88273-111">As notas para o `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="88273-111">The notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="88273-112">displayName</span><span class="sxs-lookup"><span data-stu-id="88273-112">displayName</span></span>               | <span data-ttu-id="88273-113">string</span><span class="sxs-lookup"><span data-stu-id="88273-113">string</span></span>                  | <span data-ttu-id="88273-114">O nome do `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="88273-114">The name of the `shiftItem`.</span></span> |
| <span data-ttu-id="88273-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="88273-115">startDateTime</span></span>               | <span data-ttu-id="88273-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88273-116">DateTimeOffset</span></span>                  | <span data-ttu-id="88273-117">A data e a hora de início `shiftItem`para o.</span><span class="sxs-lookup"><span data-stu-id="88273-117">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="88273-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="88273-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="88273-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="88273-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="88273-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88273-120">Required.</span></span> |
| <span data-ttu-id="88273-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="88273-121">endDateTime</span></span>               | <span data-ttu-id="88273-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88273-122">DateTimeOffset</span></span>                 | <span data-ttu-id="88273-123">A data e a hora de término `shiftItem`para o.</span><span class="sxs-lookup"><span data-stu-id="88273-123">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="88273-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88273-124">Required.</span></span> <span data-ttu-id="88273-125">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="88273-125">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="88273-126">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="88273-126">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="88273-127">tema</span><span class="sxs-lookup"><span data-stu-id="88273-127">theme</span></span> | <span data-ttu-id="88273-128">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="88273-128">scheduleEntityTheme</span></span>   |  <span data-ttu-id="88273-129">Cores suPortadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="88273-129">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="88273-130">activities</span><span class="sxs-lookup"><span data-stu-id="88273-130">activities</span></span>    | <span data-ttu-id="88273-131">coleção [shiftActivity](shiftactivity.md)</span><span class="sxs-lookup"><span data-stu-id="88273-131">[shiftActivity](shiftactivity.md) collection</span></span>   | <span data-ttu-id="88273-132">Uma parte incremental de um turno que pode abranger detalhes de quando e onde um funcionário está durante o turno.</span><span class="sxs-lookup"><span data-stu-id="88273-132">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="88273-133">Por exemplo, uma atribuição ou uma quebra ou almoço agendado.</span><span class="sxs-lookup"><span data-stu-id="88273-133">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="88273-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88273-134">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="88273-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88273-135">JSON representation</span></span>

<span data-ttu-id="88273-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88273-136">Here is a JSON representation of the resource.</span></span>

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
