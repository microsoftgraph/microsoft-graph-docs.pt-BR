---
title: Tipo de recurso recurrenceRange
description: 'Descreve um intervalo de datas sobre o qual um event recorrente se repete. '
ms.openlocfilehash: f3d627606dc9d0d41dd52f735ab87052d731af0d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036236"
---
# <a name="recurrencerange-resource-type"></a><span data-ttu-id="82eb6-103">Tipo de recurso recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="82eb6-103">recurrenceRange resource type</span></span>

> <span data-ttu-id="82eb6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="82eb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82eb6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="82eb6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82eb6-106">Descreve um intervalo de datas sobre o qual um [event](event.md) recorrente se repete.</span><span class="sxs-lookup"><span data-stu-id="82eb6-106">Describes a date range over which a recurring [event](event.md) repeats.</span></span> 

<span data-ttu-id="82eb6-107">É possível especificar o intervalo de datas para um evento recorrente de uma de três maneiras, dependendo do seu cenário.</span><span class="sxs-lookup"><span data-stu-id="82eb6-107">You can specify the date range for a recurring event in one of 3 ways depending on your scenario.</span></span> <span data-ttu-id="82eb6-108">Como você deve sempre especificar um valor de **startDate** para o intervalo de datas, é possível especificar um evento recorrente que termina em uma data específica, que não termina ou que termina após um número específico de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="82eb6-108">While you must always specify a **startDate** value for the date range, you can specify a recurring event that ends by a specific date, or that doesn't end, or that ends after a specific number of occurrences.</span></span> <span data-ttu-id="82eb6-109">As ocorrências reais dentro do intervalo de datas sempre seguem o padrão de recorrência que você especifica para o evento recorrente.</span><span class="sxs-lookup"><span data-stu-id="82eb6-109">Note that the actual occurrences within the date range always follow the recurrence pattern that you specify for the recurring event.</span></span> <span data-ttu-id="82eb6-110">Um evento recorrente é sempre definido por seu [recurrencePattern](recurrencepattern.md) (com que frequência o evento se repete) e seu **recurrenceRange** (por quanto tempo o evento se repete).</span><span class="sxs-lookup"><span data-stu-id="82eb6-110">A recurring event is always defined by its [recurrencePattern](recurrencepattern.md) (how frequently the event repeats), and its **recurrenceRange** (for how long the event repeats).</span></span>


## <a name="properties"></a><span data-ttu-id="82eb6-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82eb6-111">Properties</span></span>

| <span data-ttu-id="82eb6-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82eb6-112">Property</span></span>     | <span data-ttu-id="82eb6-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="82eb6-113">Type</span></span>   |<span data-ttu-id="82eb6-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="82eb6-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82eb6-115">endDate</span><span class="sxs-lookup"><span data-stu-id="82eb6-115">endDate</span></span>|<span data-ttu-id="82eb6-116">Data</span><span class="sxs-lookup"><span data-stu-id="82eb6-116">Date</span></span>|<span data-ttu-id="82eb6-117">A data para parar de aplicar o padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="82eb6-117">The date to stop applying the recurrence pattern.</span></span> <span data-ttu-id="82eb6-118">Dependendo do padrão de recorrência do evento, a última ocorrência da reunião pode não ser essa data.</span><span class="sxs-lookup"><span data-stu-id="82eb6-118">Depending on the recurrence pattern of the event, the last occurrence of the meeting may not be this date.</span></span> <span data-ttu-id="82eb6-119">Obrigatório se **type** for `endDate`.</span><span class="sxs-lookup"><span data-stu-id="82eb6-119">Required if **type** is `endDate`.</span></span>|
|<span data-ttu-id="82eb6-120">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="82eb6-120">numberOfOccurrences</span></span>|<span data-ttu-id="82eb6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="82eb6-121">Int32</span></span>|<span data-ttu-id="82eb6-122">O número de vezes para repetir o evento.</span><span class="sxs-lookup"><span data-stu-id="82eb6-122">The number of times to repeat the event.</span></span> <span data-ttu-id="82eb6-123">Obrigatório e deve ser positivo se **type** for `numbered`.</span><span class="sxs-lookup"><span data-stu-id="82eb6-123">Required and must be positive if **type** is `numbered`.</span></span>|
|<span data-ttu-id="82eb6-124">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="82eb6-124">recurrenceTimeZone</span></span>|<span data-ttu-id="82eb6-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82eb6-125">String</span></span> |<span data-ttu-id="82eb6-126">Fuso horário das propriedades **startDate** e **endDate**.</span><span class="sxs-lookup"><span data-stu-id="82eb6-126">Time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="82eb6-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="82eb6-127">Optional.</span></span> <span data-ttu-id="82eb6-128">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="82eb6-128">If not specified, the time zone of the event is used.</span></span>|
|<span data-ttu-id="82eb6-129">startDate</span><span class="sxs-lookup"><span data-stu-id="82eb6-129">startDate</span></span>|<span data-ttu-id="82eb6-130">Data</span><span class="sxs-lookup"><span data-stu-id="82eb6-130">Date</span></span>|<span data-ttu-id="82eb6-131">A data para começar a aplicar o padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="82eb6-131">The date to start applying the recurrence pattern.</span></span> <span data-ttu-id="82eb6-132">A primeira ocorrência da reunião pode ser essa data ou posterior, dependendo do padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="82eb6-132">The first occurrence of the meeting may be this date or later, depending on the recurrence pattern of the event.</span></span> <span data-ttu-id="82eb6-133">Deve ser o mesmo valor da propriedade **start** do [event](event.md) recorrente.</span><span class="sxs-lookup"><span data-stu-id="82eb6-133">Must be the same value as the **start** property of the recurring [event](event.md).</span></span> <span data-ttu-id="82eb6-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82eb6-134">Required.</span></span>|
|<span data-ttu-id="82eb6-135">type</span><span class="sxs-lookup"><span data-stu-id="82eb6-135">type</span></span>|<span data-ttu-id="82eb6-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82eb6-136">String</span></span>|<span data-ttu-id="82eb6-137">O intervalo de recorrência.</span><span class="sxs-lookup"><span data-stu-id="82eb6-137">The recurrence range.</span></span> <span data-ttu-id="82eb6-138">Os valores possíveis são: `endDate`, `noEnd`, `numbered`.</span><span class="sxs-lookup"><span data-stu-id="82eb6-138">Possible values are: `endDate`, `noEnd`, `numbered`.</span></span> <span data-ttu-id="82eb6-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82eb6-139">Required.</span></span>|

<span data-ttu-id="82eb6-140">Use a propriedade **type** para especificar os diferentes tipos de **recorrenceRange**.</span><span class="sxs-lookup"><span data-stu-id="82eb6-140">Use the **type** property to specify the different types of **recurrenceRange**.</span></span> <span data-ttu-id="82eb6-141">Observe as propriedades necessárias para cada tipo, conforme descrito na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="82eb6-141">Note the required properties for each type, as described in the following table.</span></span>

| <span data-ttu-id="82eb6-142">propriedade Type</span><span class="sxs-lookup"><span data-stu-id="82eb6-142">type property</span></span>  | <span data-ttu-id="82eb6-143">Tipo de intervalo de recorrência</span><span class="sxs-lookup"><span data-stu-id="82eb6-143">Type of recurrence range</span></span> | <span data-ttu-id="82eb6-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="82eb6-144">Description</span></span> | <span data-ttu-id="82eb6-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82eb6-145">Example</span></span> | <span data-ttu-id="82eb6-146">Propriedades necessárias</span><span class="sxs-lookup"><span data-stu-id="82eb6-146">Required properties</span></span> |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |<span data-ttu-id="82eb6-147">Intervalo com data final</span><span class="sxs-lookup"><span data-stu-id="82eb6-147">Range with end date</span></span> | <span data-ttu-id="82eb6-148">O evento se repete em todos os dias que se encaixam no padrão de recorrência correspondente entre **startDate** e **endDate**, incluindo essas datas.</span><span class="sxs-lookup"><span data-stu-id="82eb6-148">Event repeats on all the days that fit the corresponding recurrence pattern between the **startDate** and **endDate** inclusive.</span></span> | <span data-ttu-id="82eb6-149">Repita o evento no período entre 1º de junho de 2017 e 15 de junho de 2017.</span><span class="sxs-lookup"><span data-stu-id="82eb6-149">Repeat event in the date range between June 1, 2017 and June 15, 2017.</span></span> | <span data-ttu-id="82eb6-150">**type**, **startDate**, **endDate**</span><span class="sxs-lookup"><span data-stu-id="82eb6-150">**type**, **startDate**, **endDate**</span></span> | 
|`noEnd`   |<span data-ttu-id="82eb6-151">Intervalo sem uma data final</span><span class="sxs-lookup"><span data-stu-id="82eb6-151">Range without an end date</span></span> | <span data-ttu-id="82eb6-152">O evento se repete em todos os dias que se encaixam no padrão de recorrência correspondente começando em **startDate**.</span><span class="sxs-lookup"><span data-stu-id="82eb6-152">Event repeats on all the days that fit the corresponding recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="82eb6-153">Repita o evento no intervalo de datas que começa em 1º de junho de 2017, indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="82eb6-153">Repeat event in the date range starting on June 1, 2017 indefinitely.</span></span> | <span data-ttu-id="82eb6-154">**type**, **startDate**</span><span class="sxs-lookup"><span data-stu-id="82eb6-154">**type**, **startDate**</span></span> |
|`numbered`|<span data-ttu-id="82eb6-155">Intervalo com número específico de ocorrências</span><span class="sxs-lookup"><span data-stu-id="82eb6-155">Range with specific number of occurrences</span></span> | <span data-ttu-id="82eb6-156">O evento se repete para **numberOfOccurrences** com base no padrão de recorrência começando em **startDate**.</span><span class="sxs-lookup"><span data-stu-id="82eb6-156">Event repeats for the **numberOfOccurrences** based on the recurrence pattern beginning on the **startDate**.</span></span> | <span data-ttu-id="82eb6-157">Repita o evento no período que começa em 1º de junho de 2017, para dez ocorrências.</span><span class="sxs-lookup"><span data-stu-id="82eb6-157">Repeat event in the date range starting on June 1, 2017, for 10 occurrences.</span></span>  | <span data-ttu-id="82eb6-158">**type**, **startDate**, **numberOfOccurrences**</span><span class="sxs-lookup"><span data-stu-id="82eb6-158">**type**, **startDate**, **numberOfOccurrences**</span></span> |

## <a name="json-representation"></a><span data-ttu-id="82eb6-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82eb6-159">JSON representation</span></span>

<span data-ttu-id="82eb6-160">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="82eb6-160">Here is a JSON representation of the resource</span></span>

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
      "Warning: /api-reference/beta/resources/recurrencerange.md:
      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |"
  ],
  "tocPath": ""
}-->
