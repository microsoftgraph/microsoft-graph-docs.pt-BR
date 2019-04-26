---
title: Tipo de recurso standardTimeZoneOffset
description: Especifica quando um fuso horário muda do horário de verão para o horário padrão.
localization_priority: Normal
ms.openlocfilehash: fb6327c49c51e9bdee7e2ac5941257a45092fbb8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345697"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="eb3ee-103">Tipo de recurso standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="eb3ee-103">standardTimeZoneOffset resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb3ee-104">Especifica quando um fuso horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="eb3ee-104">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="eb3ee-105">Por exemplo, se um fuso horário estiver especificado com as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="eb3ee-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="eb3ee-106">**dayOccurrence** como 3</span><span class="sxs-lookup"><span data-stu-id="eb3ee-106">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="eb3ee-107">**dayOfWeek** como "Domingo"</span><span class="sxs-lookup"><span data-stu-id="eb3ee-107">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="eb3ee-108">**month** como 10</span><span class="sxs-lookup"><span data-stu-id="eb3ee-108">**month** is 10</span></span>
- <span data-ttu-id="eb3ee-109">**time** como 02:00:00 _ **year** como 0. Isso significa que a transição do fuso horário do horário de verão para o horário padrão ocorre às 02:00:00 da manhã no quarto domingo de maio, todos os anos.</span><span class="sxs-lookup"><span data-stu-id="eb3ee-109">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="eb3ee-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb3ee-110">Properties</span></span>
| <span data-ttu-id="eb3ee-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb3ee-111">Property</span></span>     | <span data-ttu-id="eb3ee-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb3ee-112">Type</span></span>   |<span data-ttu-id="eb3ee-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb3ee-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eb3ee-114">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="eb3ee-114">dayOccurrence</span></span> | <span data-ttu-id="eb3ee-115">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="eb3ee-115">Edm.Int32</span></span> | <span data-ttu-id="eb3ee-116">Representa a enésima ocorrência do dia da semana em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="eb3ee-116">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="eb3ee-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="eb3ee-117">dayOfWeek</span></span> | <span data-ttu-id="eb3ee-118">string</span><span class="sxs-lookup"><span data-stu-id="eb3ee-118">string</span></span> | <span data-ttu-id="eb3ee-119">Representa o dia da semana em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="eb3ee-119">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="eb3ee-120">month</span><span class="sxs-lookup"><span data-stu-id="eb3ee-120">month</span></span> | <span data-ttu-id="eb3ee-121">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="eb3ee-121">Edm.Int32</span></span> | <span data-ttu-id="eb3ee-122">Representa o mês do ano em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="eb3ee-122">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="eb3ee-123">time</span><span class="sxs-lookup"><span data-stu-id="eb3ee-123">time</span></span> | <span data-ttu-id="eb3ee-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="eb3ee-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="eb3ee-125">Representa a hora do dia em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="eb3ee-125">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="eb3ee-126">year</span><span class="sxs-lookup"><span data-stu-id="eb3ee-126">year</span></span> | <span data-ttu-id="eb3ee-127">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="eb3ee-127">Edm.Int32</span></span> | <span data-ttu-id="eb3ee-128">Representa com que frequência, em anos, ocorre a mudança do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="eb3ee-128">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="eb3ee-129">Por exemplo, um valor 0 significa todos os anos.</span><span class="sxs-lookup"><span data-stu-id="eb3ee-129">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="eb3ee-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb3ee-130">JSON representation</span></span>

<span data-ttu-id="eb3ee-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb3ee-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
