---
title: Tipo de recurso standardTimeZoneOffset
description: Especifica quando um fuso horário muda do horário de verão para o horário padrão.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: a4e17da5e05afaef312e951c3cfe52a7e6ca4e69
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128817"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="f6167-103">Tipo de recurso standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="f6167-103">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="f6167-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6167-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6167-105">Especifica quando um fuso horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="f6167-105">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="f6167-106">Por exemplo, se um fuso horário estiver especificado com as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="f6167-106">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="f6167-107">**dayOccurrence** como 3</span><span class="sxs-lookup"><span data-stu-id="f6167-107">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="f6167-108">**dayOfWeek** como "Domingo"</span><span class="sxs-lookup"><span data-stu-id="f6167-108">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="f6167-109">**month** como 10</span><span class="sxs-lookup"><span data-stu-id="f6167-109">**month** is 10</span></span>
- <span data-ttu-id="f6167-110">**time** como 02:00:00 _ **year** como 0. Isso significa que a transição do fuso horário do horário de verão para o horário padrão ocorre às 02:00:00 da manhã no quarto domingo de maio, todos os anos.</span><span class="sxs-lookup"><span data-stu-id="f6167-110">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="f6167-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6167-111">Properties</span></span>
| <span data-ttu-id="f6167-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6167-112">Property</span></span>     | <span data-ttu-id="f6167-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6167-113">Type</span></span>   |<span data-ttu-id="f6167-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6167-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f6167-115">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="f6167-115">dayOccurrence</span></span> | <span data-ttu-id="f6167-116">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="f6167-116">Edm.Int32</span></span> | <span data-ttu-id="f6167-117">Representa a enésima ocorrência do dia da semana em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="f6167-117">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="f6167-118">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="f6167-118">dayOfWeek</span></span> | <span data-ttu-id="f6167-119">string</span><span class="sxs-lookup"><span data-stu-id="f6167-119">string</span></span> | <span data-ttu-id="f6167-120">Representa o dia da semana em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="f6167-120">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="f6167-121">month</span><span class="sxs-lookup"><span data-stu-id="f6167-121">month</span></span> | <span data-ttu-id="f6167-122">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="f6167-122">Edm.Int32</span></span> | <span data-ttu-id="f6167-123">Representa o mês do ano em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="f6167-123">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="f6167-124">time</span><span class="sxs-lookup"><span data-stu-id="f6167-124">time</span></span> | <span data-ttu-id="f6167-125">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f6167-125">Edm.TimeOfDay</span></span> | <span data-ttu-id="f6167-126">Representa a hora do dia em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="f6167-126">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="f6167-127">year</span><span class="sxs-lookup"><span data-stu-id="f6167-127">year</span></span> | <span data-ttu-id="f6167-128">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="f6167-128">Edm.Int32</span></span> | <span data-ttu-id="f6167-129">Representa com que frequência, em anos, ocorre a mudança do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="f6167-129">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="f6167-130">Por exemplo, um valor 0 significa todos os anos.</span><span class="sxs-lookup"><span data-stu-id="f6167-130">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f6167-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6167-131">JSON representation</span></span>

<span data-ttu-id="f6167-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6167-132">Here is a JSON representation of the resource.</span></span>

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


