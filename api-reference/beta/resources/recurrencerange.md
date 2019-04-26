---
title: Tipo de recurso recurrenceRange
description: 'Descreve um intervalo de datas sobre o qual um event recorrente se repete. '
localization_priority: Normal
ms.openlocfilehash: f20d8b134f4b1e0f338b615dd3129a17d585ca94
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343883"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="fd8da-103">Tipo de recurso recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="fd8da-103">recurrenceRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd8da-104">Descreve um intervalo de datas sobre o qual um [event](event.md) recorrente se repete.</span><span class="sxs-lookup"><span data-stu-id="fd8da-104">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="fd8da-105">É possível especificar o intervalo de datas para um evento recorrente de uma de três maneiras, dependendo do seu cenário.</span><span class="sxs-lookup"><span data-stu-id="fd8da-105">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="fd8da-106">Como você deve sempre especificar um valor de **startDate** para o intervalo de datas, é possível especificar um evento recorrente que termina em uma data específica, que não termina ou que termina após um número específico de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="fd8da-106">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="fd8da-107">As ocorrências reais dentro do intervalo de datas sempre seguem o padrão de recorrência que você especifica para o evento recorrente.</span><span class="sxs-lookup"><span data-stu-id="fd8da-107">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="fd8da-108">Um evento recorrente é sempre definido por seu [recurrencePattern](recurrencepattern.md) (com que frequência o evento se repete) e seu **recurrenceRange** (por quanto tempo o evento se repete).</span><span class="sxs-lookup"><span data-stu-id="fd8da-108">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>


## <a name="properties"></a><span data-ttu-id="fd8da-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd8da-109">Properties</span></span>

| <span data-ttu-id="fd8da-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd8da-110">Property</span></span>     | <span data-ttu-id="fd8da-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd8da-111">Type</span></span>   |<span data-ttu-id="fd8da-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd8da-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd8da-113">endDate</span><span class="sxs-lookup"><span data-stu-id="fd8da-113">endDate</span></span>|<span data-ttu-id="fd8da-114">Data</span><span class="sxs-lookup"><span data-stu-id="fd8da-114">Date</span></span>|<span data-ttu-id="fd8da-115">A data para parar de aplicar o padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="fd8da-115">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="fd8da-116">Dependendo do padrão de recorrência do evento, a última ocorrência da reunião pode não ser essa data.</span><span class="sxs-lookup"><span data-stu-id="fd8da-116">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="fd8da-117">Obrigatório se **type** for `endDate`.</span><span class="sxs-lookup"><span data-stu-id="fd8da-117">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="fd8da-118">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="fd8da-118">numberOfOccurrences</span></span>|<span data-ttu-id="fd8da-119">Int32</span><span class="sxs-lookup"><span data-stu-id="fd8da-119">Int32</span></span>|<span data-ttu-id="fd8da-120">O número de vezes para repetir o evento.</span><span class="sxs-lookup"><span data-stu-id="fd8da-120">The number of times to repeat the event.</span></span> <span data-ttu-id="fd8da-121">Obrigatório e deve ser positivo se **type** for `numbered`.</span><span class="sxs-lookup"><span data-stu-id="fd8da-121">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="fd8da-122">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="fd8da-122">recurrenceTimeZone</span></span>|<span data-ttu-id="fd8da-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd8da-123">String</span></span> |<span data-ttu-id="fd8da-124">Fuso horário das propriedades **startDate** e **endDate**.</span><span class="sxs-lookup"><span data-stu-id="fd8da-124">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="fd8da-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="fd8da-125">Optional.</span></span> <span data-ttu-id="fd8da-126">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="fd8da-126">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="fd8da-127">startDate</span><span class="sxs-lookup"><span data-stu-id="fd8da-127">startDate</span></span>|<span data-ttu-id="fd8da-128">Data</span><span class="sxs-lookup"><span data-stu-id="fd8da-128">Date</span></span>|<span data-ttu-id="fd8da-129">A data para começar a aplicar o padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="fd8da-129">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="fd8da-130">A primeira ocorrência da reunião pode ser essa data ou posterior, dependendo do padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="fd8da-130">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="fd8da-131">Deve ser o mesmo valor da propriedade **start** do [event](event.md) recorrente.</span><span class="sxs-lookup"><span data-stu-id="fd8da-131">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="fd8da-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd8da-132">Required.</span></span>|
|<span data-ttu-id="fd8da-133">type</span><span class="sxs-lookup"><span data-stu-id="fd8da-133">type</span></span>|<span data-ttu-id="fd8da-134">String</span><span class="sxs-lookup"><span data-stu-id="fd8da-134">String</span></span>|<span data-ttu-id="fd8da-135">O intervalo de recorrência.</span><span class="sxs-lookup"><span data-stu-id="fd8da-135">The recurrence range.</span></span> <span data-ttu-id="fd8da-136">Os valores possíveis são: `endDate`, `noEnd`, `numbered`.</span><span class="sxs-lookup"><span data-stu-id="fd8da-136">Possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="fd8da-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd8da-137">Required.</span></span>|

<span data-ttu-id="fd8da-138">Use a propriedade **type** para especificar os diferentes tipos de **recorrenceRange**.</span><span class="sxs-lookup"><span data-stu-id="fd8da-138">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="fd8da-139">Observe as propriedades necessárias para cada tipo, conforme descrito na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="fd8da-139">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="fd8da-140">Propriedade Type</span><span class="sxs-lookup"><span data-stu-id="fd8da-140">type property</span></span>  | <span data-ttu-id="fd8da-141">Tipo de intervalo de recorrência</span><span class="sxs-lookup"><span data-stu-id="fd8da-141">Type of recurrence range</span></span> | <span data-ttu-id="fd8da-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd8da-142">Description</span></span> | <span data-ttu-id="fd8da-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd8da-143">Example</span></span> | <span data-ttu-id="fd8da-144">Propriedades necessárias</span><span class="sxs-lookup"><span data-stu-id="fd8da-144">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="fd8da-145">Intervalo com data final</span><span class="sxs-lookup"><span data-stu-id="fd8da-145">Range with end date</span></span> | <span data-ttu-id="fd8da-146">O evento se repete em todos os dias que se encaixam no padrão de recorrência correspondente entre **startDate** e **endDate**, incluindo essas datas.</span><span class="sxs-lookup"><span data-stu-id="fd8da-146">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="fd8da-147">Repita o evento no período entre 1º de junho de 2017 e 15 de junho de 2017.</span><span class="sxs-lookup"><span data-stu-id="fd8da-147">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="fd8da-148">**type**, **startDate**, **endDate**</span><span class="sxs-lookup"><span data-stu-id="fd8da-148">**type**, **startDate**, **endDate**</span></span> | 
|`noEnd`   |<span data-ttu-id="fd8da-149">Intervalo sem uma data final</span><span class="sxs-lookup"><span data-stu-id="fd8da-149">Range without an end date</span></span> | <span data-ttu-id="fd8da-150">O evento se repete em todos os dias que se encaixam no padrão de recorrência correspondente começando em **startDate**.</span><span class="sxs-lookup"><span data-stu-id="fd8da-150">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="fd8da-151">Repita o evento no intervalo de datas que começa em 1º de junho de 2017, indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="fd8da-151">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="fd8da-152">**type**, **startDate**</span><span class="sxs-lookup"><span data-stu-id="fd8da-152">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="fd8da-153">Intervalo com número específico de ocorrências</span><span class="sxs-lookup"><span data-stu-id="fd8da-153">Range with specific number of occurrences</span></span> | <span data-ttu-id="fd8da-154">O evento se repete para **numberOfOccurrences** com base no padrão de recorrência começando em **startDate**.</span><span class="sxs-lookup"><span data-stu-id="fd8da-154">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="fd8da-155">Repita o evento no período que começa em 1º de junho de 2017, para dez ocorrências.</span><span class="sxs-lookup"><span data-stu-id="fd8da-155">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="fd8da-156">**type**, **startDate**, **numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="fd8da-156">**type**, **startDate**, **numberOfOccurrences**</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fd8da-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd8da-157">JSON representation</span></span>

<span data-ttu-id="fd8da-158">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fd8da-158">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrenceRange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/resources/recurrencerange.md:\r\n      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |"
  ]
}
-->
