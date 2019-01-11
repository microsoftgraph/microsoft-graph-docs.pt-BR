---
title: Tipo de recurso recurrenceRange
description: 'Descreve um intervalo de datas sobre o qual um event recorrente se repete. '
localization_priority: Normal
ms.openlocfilehash: 4129b698e48b01e0208b88fbdc57fb777835cd4e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872983"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="7481b-103">Tipo de recurso recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="7481b-103">recurrenceRange resource type</span></span>

<span data-ttu-id="7481b-104">Descreve um intervalo de datas sobre o qual um [event](event.md) recorrente se repete.</span><span class="sxs-lookup"><span data-stu-id="7481b-104">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="7481b-105">É possível especificar o intervalo de datas para um evento recorrente de uma de três maneiras, dependendo do seu cenário.</span><span class="sxs-lookup"><span data-stu-id="7481b-105">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="7481b-106">Como você deve sempre especificar um valor de **startDate** para o intervalo de datas, é possível especificar um evento recorrente que termina em uma data específica, que não termina ou que termina após um número específico de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="7481b-106">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="7481b-107">As ocorrências reais dentro do intervalo de datas sempre seguem o padrão de recorrência que você especifica para o evento recorrente.</span><span class="sxs-lookup"><span data-stu-id="7481b-107">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="7481b-108">Um evento recorrente é sempre definido por seu [recurrencePattern](recurrencepattern.md) (com que frequência o evento se repete) e seu **recurrenceRange** (por quanto tempo o evento se repete).</span><span class="sxs-lookup"><span data-stu-id="7481b-108">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>

## <a name="properties"></a><span data-ttu-id="7481b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7481b-109">Properties</span></span>

| <span data-ttu-id="7481b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7481b-110">Property</span></span>     | <span data-ttu-id="7481b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7481b-111">Type</span></span>   |<span data-ttu-id="7481b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7481b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7481b-113">endDate</span><span class="sxs-lookup"><span data-stu-id="7481b-113">endDate</span></span>|<span data-ttu-id="7481b-114">Data</span><span class="sxs-lookup"><span data-stu-id="7481b-114">Date</span></span>|<span data-ttu-id="7481b-115">A data para parar de aplicar o padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="7481b-115">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="7481b-116">Dependendo do padrão de recorrência do evento, a última ocorrência da reunião pode não ser essa data.</span><span class="sxs-lookup"><span data-stu-id="7481b-116">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="7481b-117">Obrigatório se **type** for `endDate`.</span><span class="sxs-lookup"><span data-stu-id="7481b-117">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="7481b-118">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="7481b-118">numberOfOccurrences</span></span>|<span data-ttu-id="7481b-119">Int32</span><span class="sxs-lookup"><span data-stu-id="7481b-119">Int32</span></span>|<span data-ttu-id="7481b-120">O número de vezes para repetir o evento.</span><span class="sxs-lookup"><span data-stu-id="7481b-120">The number of times to repeat the event.</span></span> <span data-ttu-id="7481b-121">Obrigatório e deve ser positivo se **type** for `numbered`.</span><span class="sxs-lookup"><span data-stu-id="7481b-121">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="7481b-122">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="7481b-122">recurrenceTimeZone</span></span>|<span data-ttu-id="7481b-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7481b-123">String</span></span> |<span data-ttu-id="7481b-124">Fuso horário das propriedades **startDate** e **endDate**.</span><span class="sxs-lookup"><span data-stu-id="7481b-124">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="7481b-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7481b-125">Optional.</span></span> <span data-ttu-id="7481b-126">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="7481b-126">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="7481b-127">startDate</span><span class="sxs-lookup"><span data-stu-id="7481b-127">startDate</span></span>|<span data-ttu-id="7481b-128">Data</span><span class="sxs-lookup"><span data-stu-id="7481b-128">Date</span></span>|<span data-ttu-id="7481b-129">A data para começar a aplicar o padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="7481b-129">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="7481b-130">A primeira ocorrência da reunião pode ser essa data ou posterior, dependendo do padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="7481b-130">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="7481b-131">Deve ser o mesmo valor da propriedade **start** do [event](event.md) recorrente.</span><span class="sxs-lookup"><span data-stu-id="7481b-131">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="7481b-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7481b-132">Required.</span></span>|
|<span data-ttu-id="7481b-133">type</span><span class="sxs-lookup"><span data-stu-id="7481b-133">type</span></span>|<span data-ttu-id="7481b-134">recurrenceRangeType</span><span class="sxs-lookup"><span data-stu-id="7481b-134">recurrenceRangeType</span></span>|<span data-ttu-id="7481b-135">O intervalo de recorrência.</span><span class="sxs-lookup"><span data-stu-id="7481b-135">The recurrence range.</span></span> <span data-ttu-id="7481b-136">Os valores possíveis são: `endDate`, `noEnd`, `numbered`.</span><span class="sxs-lookup"><span data-stu-id="7481b-136">The possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="7481b-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7481b-137">Required.</span></span>|

<span data-ttu-id="7481b-138">Use a propriedade **type** para especificar os diferentes tipos de **recorrenceRange**.</span><span class="sxs-lookup"><span data-stu-id="7481b-138">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="7481b-139">Observe as propriedades necessárias para cada tipo, conforme descrito na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="7481b-139">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="7481b-140">propriedade Type</span><span class="sxs-lookup"><span data-stu-id="7481b-140">type property</span></span>  | <span data-ttu-id="7481b-141">Tipo de intervalo de recorrência</span><span class="sxs-lookup"><span data-stu-id="7481b-141">Type of recurrence range</span></span> | <span data-ttu-id="7481b-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="7481b-142">Description</span></span> | <span data-ttu-id="7481b-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7481b-143">Example</span></span> | <span data-ttu-id="7481b-144">Propriedades necessárias</span><span class="sxs-lookup"><span data-stu-id="7481b-144">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="7481b-145">Intervalo com data final</span><span class="sxs-lookup"><span data-stu-id="7481b-145">Range with end date</span></span> | <span data-ttu-id="7481b-146">O evento se repete em todos os dias que se encaixam no padrão de recorrência correspondente entre **startDate** e **endDate**, incluindo essas datas.</span><span class="sxs-lookup"><span data-stu-id="7481b-146">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="7481b-147">Repita o evento no período entre 1º de junho de 2017 e 15 de junho de 2017.</span><span class="sxs-lookup"><span data-stu-id="7481b-147">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="7481b-148">**type**, **startDate**, **endDate**</span><span class="sxs-lookup"><span data-stu-id="7481b-148">**type**, **startDate**, **endDate**</span></span> | 
|`noEnd`  |<span data-ttu-id="7481b-149">Intervalo sem uma data final</span><span class="sxs-lookup"><span data-stu-id="7481b-149">Range without an end date</span></span> | <span data-ttu-id="7481b-150">O evento se repete em todos os dias que se encaixam no padrão de recorrência correspondente começando em **startDate**.</span><span class="sxs-lookup"><span data-stu-id="7481b-150">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="7481b-151">Repita o evento no intervalo de datas que começa em 1º de junho de 2017, indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="7481b-151">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="7481b-152">**type**, **startDate**</span><span class="sxs-lookup"><span data-stu-id="7481b-152">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="7481b-153">Intervalo com número específico de ocorrências</span><span class="sxs-lookup"><span data-stu-id="7481b-153">Range with specific number of occurrences</span></span> | <span data-ttu-id="7481b-154">O evento se repete para **numberOfOccurrences** com base no padrão de recorrência começando em **startDate**.</span><span class="sxs-lookup"><span data-stu-id="7481b-154">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="7481b-155">Repita o evento no período que começa em 1º de junho de 2017, para dez ocorrências.</span><span class="sxs-lookup"><span data-stu-id="7481b-155">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="7481b-156">**type**, **startDate**, **numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="7481b-156">**type**, **startDate**, **numberOfOccurrences**</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7481b-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7481b-157">JSON representation</span></span>

<span data-ttu-id="7481b-158">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7481b-158">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/resources/recurrencerange.md:
      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |"
  ],
  "tocPath": ""
}-->
