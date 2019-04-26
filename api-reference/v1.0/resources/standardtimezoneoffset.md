---
title: Tipo de recurso standardTimeZoneOffset
description: Especifica quando um fuso horário muda do horário de verão para o horário padrão.
localization_priority: Normal
ms.openlocfilehash: 5e224865f201041b72fb943bc3a76e8a67f7975a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555889"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="b35f0-103">Tipo de recurso standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="b35f0-103">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="b35f0-104">Especifica quando um fuso horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="b35f0-104">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="b35f0-105">Por exemplo, se um fuso horário estiver especificado com as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="b35f0-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="b35f0-106">**dayOccurrence** como 3</span><span class="sxs-lookup"><span data-stu-id="b35f0-106">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="b35f0-107">**dayOfWeek** como "Domingo"</span><span class="sxs-lookup"><span data-stu-id="b35f0-107">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="b35f0-108">**month** como 10</span><span class="sxs-lookup"><span data-stu-id="b35f0-108">**month** is 10</span></span>
- <span data-ttu-id="b35f0-109">**time** como 02:00:00 _ **year** como 0. Isso significa que a transição do fuso horário do horário de verão para o horário padrão ocorre às 02:00:00 da manhã no quarto domingo de maio, todos os anos.</span><span class="sxs-lookup"><span data-stu-id="b35f0-109">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="b35f0-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b35f0-110">Properties</span></span>
| <span data-ttu-id="b35f0-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b35f0-111">Property</span></span>     | <span data-ttu-id="b35f0-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="b35f0-112">Type</span></span>   |<span data-ttu-id="b35f0-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b35f0-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b35f0-114">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="b35f0-114">dayOccurrence</span></span> | <span data-ttu-id="b35f0-115">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b35f0-115">Edm.Int32</span></span> | <span data-ttu-id="b35f0-116">Representa a enésima ocorrência do dia da semana em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="b35f0-116">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="b35f0-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="b35f0-117">dayOfWeek</span></span> | <span data-ttu-id="b35f0-118">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="b35f0-118">dayOfWeek</span></span> | <span data-ttu-id="b35f0-119">Representa o dia da semana em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="b35f0-119">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="b35f0-120">month</span><span class="sxs-lookup"><span data-stu-id="b35f0-120">month</span></span> | <span data-ttu-id="b35f0-121">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b35f0-121">Edm.Int32</span></span> | <span data-ttu-id="b35f0-122">Representa o mês do ano em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="b35f0-122">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="b35f0-123">time</span><span class="sxs-lookup"><span data-stu-id="b35f0-123">time</span></span> | <span data-ttu-id="b35f0-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b35f0-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="b35f0-125">Representa a hora do dia em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="b35f0-125">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="b35f0-126">year</span><span class="sxs-lookup"><span data-stu-id="b35f0-126">year</span></span> | <span data-ttu-id="b35f0-127">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b35f0-127">Edm.Int32</span></span> | <span data-ttu-id="b35f0-128">Representa com que frequência, em anos, ocorre a mudança do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="b35f0-128">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="b35f0-129">Por exemplo, um valor 0 significa todos os anos.</span><span class="sxs-lookup"><span data-stu-id="b35f0-129">For example, a value of 0 means every year.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b35f0-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b35f0-130">JSON representation</span></span>

<span data-ttu-id="b35f0-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b35f0-131">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
