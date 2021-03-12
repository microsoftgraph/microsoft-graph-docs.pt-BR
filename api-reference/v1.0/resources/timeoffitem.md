---
title: Tipo de recurso timeOffItem
description: Representa uma versão do timeOff.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: a710c1c2de9a2ff127b19a083a3c90d5bfface5a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720839"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="62d2e-103">Tipo de recurso timeOffItem</span><span class="sxs-lookup"><span data-stu-id="62d2e-103">timeOffItem resource type</span></span>

<span data-ttu-id="62d2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62d2e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62d2e-105">Representa uma versão do [timeOff](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="62d2e-105">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="62d2e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62d2e-106">Properties</span></span>
| <span data-ttu-id="62d2e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62d2e-107">Property</span></span>                         | <span data-ttu-id="62d2e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="62d2e-108">Type</span></span>                    | <span data-ttu-id="62d2e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="62d2e-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="62d2e-110">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="62d2e-110">timeOffReasonId</span></span>               | <span data-ttu-id="62d2e-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62d2e-111">string</span></span>                  | <span data-ttu-id="62d2e-112">ID do `timeOffReason` para isso `timeOffItem` .</span><span class="sxs-lookup"><span data-stu-id="62d2e-112">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="62d2e-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62d2e-113">Required.</span></span>     |
| <span data-ttu-id="62d2e-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="62d2e-114">startDateTime</span></span>               | <span data-ttu-id="62d2e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62d2e-115">DateTimeOffset</span></span>                  | <span data-ttu-id="62d2e-116">A data e a hora de início do `timeOffItem` .</span><span class="sxs-lookup"><span data-stu-id="62d2e-116">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="62d2e-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62d2e-117">Required.</span></span> <span data-ttu-id="62d2e-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="62d2e-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="62d2e-119">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="62d2e-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="62d2e-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="62d2e-120">endDateTime</span></span>               | <span data-ttu-id="62d2e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62d2e-121">DateTimeOffset</span></span>                  | <span data-ttu-id="62d2e-122">A data e a hora de término do `timeOffItem` .</span><span class="sxs-lookup"><span data-stu-id="62d2e-122">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="62d2e-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62d2e-123">Required.</span></span> <span data-ttu-id="62d2e-124">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="62d2e-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="62d2e-125">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="62d2e-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="62d2e-126">tema</span><span class="sxs-lookup"><span data-stu-id="62d2e-126">theme</span></span> | <span data-ttu-id="62d2e-127">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="62d2e-127">scheduleEntityTheme</span></span>   | <span data-ttu-id="62d2e-128">Cores com suporte: branco; azul; verde; roxo; rosa; amarelo; cinza; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="62d2e-128">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="62d2e-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62d2e-129">JSON representation</span></span>

<span data-ttu-id="62d2e-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62d2e-130">Here is a JSON representation of the resource.</span></span>

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

