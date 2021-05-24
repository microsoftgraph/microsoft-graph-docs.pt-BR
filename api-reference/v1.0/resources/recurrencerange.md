---
title: Tipo de recurso recurrenceRange
description: 'Descreve um intervalo de datas sobre o qual um event recorrente se repete. '
localization_priority: Normal
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0b7aa184981549f45c9c5d00e5c32cd5431123c2
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547257"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="226d9-103">Tipo de recurso recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="226d9-103">recurrenceRange resource type</span></span>

<span data-ttu-id="226d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="226d9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="226d9-105">Descreve um intervalo de datas sobre o qual um [event](event.md) recorrente se repete.</span><span class="sxs-lookup"><span data-stu-id="226d9-105">Describes a date range over which a recurring [event](event.md) repeats.</span></span>

<span data-ttu-id="226d9-106">É possível especificar o intervalo de datas para um evento recorrente de uma de três maneiras, dependendo do seu cenário.</span><span class="sxs-lookup"><span data-stu-id="226d9-106">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="226d9-107">Como você deve sempre especificar um valor de **startDate** para o intervalo de datas, é possível especificar um evento recorrente que termina em uma data específica, que não termina ou que termina após um número específico de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="226d9-107">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="226d9-108">As ocorrências reais dentro do intervalo de datas sempre seguem o padrão de recorrência que você especifica para o evento recorrente.</span><span class="sxs-lookup"><span data-stu-id="226d9-108">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="226d9-109">Um evento recorrente é sempre definido por seu [recurrencePattern](recurrencepattern.md) (com que frequência o evento se repete) e seu **recurrenceRange** (por quanto tempo o evento se repete).</span><span class="sxs-lookup"><span data-stu-id="226d9-109">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>

## <a name="properties"></a><span data-ttu-id="226d9-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="226d9-110">Properties</span></span>

| <span data-ttu-id="226d9-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="226d9-111">Property</span></span>     | <span data-ttu-id="226d9-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="226d9-112">Type</span></span>   |<span data-ttu-id="226d9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="226d9-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="226d9-114">endDate</span><span class="sxs-lookup"><span data-stu-id="226d9-114">endDate</span></span>|<span data-ttu-id="226d9-115">Data</span><span class="sxs-lookup"><span data-stu-id="226d9-115">Date</span></span>|<span data-ttu-id="226d9-116">A data para parar de aplicar o padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="226d9-116">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="226d9-117">Dependendo do padrão de recorrência do evento, a última ocorrência da reunião pode não ser essa data.</span><span class="sxs-lookup"><span data-stu-id="226d9-117">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="226d9-118">Obrigatório se **type** for `endDate`.</span><span class="sxs-lookup"><span data-stu-id="226d9-118">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="226d9-119">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="226d9-119">numberOfOccurrences</span></span>|<span data-ttu-id="226d9-120">Int32</span><span class="sxs-lookup"><span data-stu-id="226d9-120">Int32</span></span>|<span data-ttu-id="226d9-121">O número de vezes para repetir o evento.</span><span class="sxs-lookup"><span data-stu-id="226d9-121">The number of times to repeat the event.</span></span> <span data-ttu-id="226d9-122">Obrigatório e deve ser positivo se **type** for `numbered`.</span><span class="sxs-lookup"><span data-stu-id="226d9-122">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="226d9-123">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="226d9-123">recurrenceTimeZone</span></span>|<span data-ttu-id="226d9-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="226d9-124">String</span></span> |<span data-ttu-id="226d9-125">Fuso horário das propriedades **startDate** e **endDate**.</span><span class="sxs-lookup"><span data-stu-id="226d9-125">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="226d9-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="226d9-126">Optional.</span></span> <span data-ttu-id="226d9-127">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="226d9-127">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="226d9-128">startDate</span><span class="sxs-lookup"><span data-stu-id="226d9-128">startDate</span></span>|<span data-ttu-id="226d9-129">Data</span><span class="sxs-lookup"><span data-stu-id="226d9-129">Date</span></span>|<span data-ttu-id="226d9-130">A data para começar a aplicar o padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="226d9-130">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="226d9-131">A primeira ocorrência da reunião pode ser essa data ou posterior, dependendo do padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="226d9-131">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="226d9-132">Deve ser o mesmo valor da propriedade **start** do [event](event.md) recorrente.</span><span class="sxs-lookup"><span data-stu-id="226d9-132">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="226d9-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="226d9-133">Required.</span></span>|
|<span data-ttu-id="226d9-134">type</span><span class="sxs-lookup"><span data-stu-id="226d9-134">type</span></span>|<span data-ttu-id="226d9-135">recurrenceRangeType</span><span class="sxs-lookup"><span data-stu-id="226d9-135">recurrenceRangeType</span></span>|<span data-ttu-id="226d9-136">O intervalo de recorrência.</span><span class="sxs-lookup"><span data-stu-id="226d9-136">The recurrence range.</span></span> <span data-ttu-id="226d9-137">Os valores possíveis são: `endDate`, `noEnd`, `numbered`.</span><span class="sxs-lookup"><span data-stu-id="226d9-137">The possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="226d9-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="226d9-138">Required.</span></span>|

<span data-ttu-id="226d9-139">Use a propriedade **type** para especificar os diferentes tipos de **recorrenceRange**.</span><span class="sxs-lookup"><span data-stu-id="226d9-139">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="226d9-140">Observe as propriedades necessárias para cada tipo, conforme descrito na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="226d9-140">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="226d9-141">propriedade type</span><span class="sxs-lookup"><span data-stu-id="226d9-141">type property</span></span>  | <span data-ttu-id="226d9-142">Tipo de intervalo de recorrência</span><span class="sxs-lookup"><span data-stu-id="226d9-142">Type of recurrence range</span></span> | <span data-ttu-id="226d9-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="226d9-143">Description</span></span> | <span data-ttu-id="226d9-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="226d9-144">Example</span></span> | <span data-ttu-id="226d9-145">Propriedades necessárias</span><span class="sxs-lookup"><span data-stu-id="226d9-145">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="226d9-146">Intervalo com data final</span><span class="sxs-lookup"><span data-stu-id="226d9-146">Range with end date</span></span> | <span data-ttu-id="226d9-147">O evento se repete em todos os dias que se encaixam no padrão de recorrência correspondente entre **startDate** e **endDate**, incluindo essas datas.</span><span class="sxs-lookup"><span data-stu-id="226d9-147">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="226d9-148">Repita o evento no período entre 1º de junho de 2017 e 15 de junho de 2017.</span><span class="sxs-lookup"><span data-stu-id="226d9-148">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="226d9-149">**type**, **startDate**, **endDate**</span><span class="sxs-lookup"><span data-stu-id="226d9-149">**type**, **startDate**, **endDate**</span></span> |
|`noEnd`  |<span data-ttu-id="226d9-150">Intervalo sem uma data final</span><span class="sxs-lookup"><span data-stu-id="226d9-150">Range without an end date</span></span> | <span data-ttu-id="226d9-151">O evento se repete em todos os dias que se encaixam no padrão de recorrência correspondente começando em **startDate**.</span><span class="sxs-lookup"><span data-stu-id="226d9-151">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="226d9-152">Repita o evento no intervalo de datas que começa em 1º de junho de 2017, indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="226d9-152">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="226d9-153">**type**, **startDate**</span><span class="sxs-lookup"><span data-stu-id="226d9-153">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="226d9-154">Intervalo com número específico de ocorrências</span><span class="sxs-lookup"><span data-stu-id="226d9-154">Range with specific number of occurrences</span></span> | <span data-ttu-id="226d9-155">O evento se repete para **numberOfOccurrences** com base no padrão de recorrência começando em **startDate**.</span><span class="sxs-lookup"><span data-stu-id="226d9-155">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="226d9-156">Repita o evento no período que começa em 1º de junho de 2017, para dez ocorrências.</span><span class="sxs-lookup"><span data-stu-id="226d9-156">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="226d9-157">**type**, **startDate**, **numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="226d9-157">**type**, **startDate**, **numberOfOccurrences**</span></span> |


## <a name="json-representation"></a><span data-ttu-id="226d9-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="226d9-158">JSON representation</span></span>

<span data-ttu-id="226d9-159">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="226d9-159">Here is a JSON representation of the resource</span></span>

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
  ],
  "tocPath": ""
}-->

