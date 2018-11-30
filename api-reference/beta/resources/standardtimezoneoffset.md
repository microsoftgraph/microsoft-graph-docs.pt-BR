---
title: Tipo de recurso standardTimeZoneOffset
description: Especifica quando um fuso horário muda do horário de verão para o horário padrão.
ms.openlocfilehash: 167ff45f4ccf1615c1560c3f2ba130cdc7747043
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036488"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="c5d04-103">Tipo de recurso standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="c5d04-103">standardTimeZoneOffset resource type</span></span>

> <span data-ttu-id="c5d04-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c5d04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5d04-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c5d04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5d04-106">Especifica quando um fuso horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c5d04-106">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="c5d04-107">Por exemplo, se um fuso horário estiver especificado com as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="c5d04-107">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="c5d04-108">**dayOccurrence** como 3</span><span class="sxs-lookup"><span data-stu-id="c5d04-108">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="c5d04-109">**dayOfWeek** como "Domingo"</span><span class="sxs-lookup"><span data-stu-id="c5d04-109">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="c5d04-110">**month** como 10</span><span class="sxs-lookup"><span data-stu-id="c5d04-110">**month** is 10</span></span>
- <span data-ttu-id="c5d04-111">**time** como 02:00:00 _ **year** como 0. Isso significa que a transição do fuso horário do horário de verão para o horário padrão ocorre às 02:00:00 da manhã no quarto domingo de maio, todos os anos.</span><span class="sxs-lookup"><span data-stu-id="c5d04-111">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="c5d04-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5d04-112">Properties</span></span>
| <span data-ttu-id="c5d04-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5d04-113">Property</span></span>     | <span data-ttu-id="c5d04-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5d04-114">Type</span></span>   |<span data-ttu-id="c5d04-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5d04-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c5d04-116">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="c5d04-116">dayOccurrence</span></span> | <span data-ttu-id="c5d04-117">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="c5d04-117">Edm.Int32</span></span> | <span data-ttu-id="c5d04-118">Representa a enésima ocorrência do dia da semana em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c5d04-118">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="c5d04-119">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="c5d04-119">dayOfWeek</span></span> | <span data-ttu-id="c5d04-120">string</span><span class="sxs-lookup"><span data-stu-id="c5d04-120">string</span></span> | <span data-ttu-id="c5d04-121">Representa o dia da semana em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c5d04-121">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="c5d04-122">month</span><span class="sxs-lookup"><span data-stu-id="c5d04-122">month</span></span> | <span data-ttu-id="c5d04-123">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="c5d04-123">Edm.Int32</span></span> | <span data-ttu-id="c5d04-124">Representa o mês do ano em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c5d04-124">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="c5d04-125">time</span><span class="sxs-lookup"><span data-stu-id="c5d04-125">time</span></span> | <span data-ttu-id="c5d04-126">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c5d04-126">Edm.TimeOfDay</span></span> | <span data-ttu-id="c5d04-127">Representa a hora do dia em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c5d04-127">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="c5d04-128">year</span><span class="sxs-lookup"><span data-stu-id="c5d04-128">year</span></span> | <span data-ttu-id="c5d04-129">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="c5d04-129">Edm.Int32</span></span> | <span data-ttu-id="c5d04-130">Representa com que frequência, em anos, ocorre a mudança do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c5d04-130">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="c5d04-131">Por exemplo, um valor 0 significa todos os anos.</span><span class="sxs-lookup"><span data-stu-id="c5d04-131">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c5d04-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5d04-132">JSON representation</span></span>

<span data-ttu-id="c5d04-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5d04-133">Here is a JSON representation of the resource.</span></span>

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