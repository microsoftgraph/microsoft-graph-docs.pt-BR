---
title: Agendar compromissos repetidos como eventos recorrentes no Outlook
description: Eventos recorrentes são uma parte importante do calendário do Outlook. Seja uma reunião semanal individual com seu gerente ou uma reunião de revisão de toda a divisão que ocorre na segunda terça-feira de cada mês, eventos recorrentes permitem que o evento seja criado uma fez e que o servidor preencha o restante da série.
author: harini84
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 67736178c0f1987b85bbf1004ed41df8110f512f
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470078"
---
# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="89344-104">Agendar compromissos repetidos como eventos recorrentes no Outlook</span><span class="sxs-lookup"><span data-stu-id="89344-104">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="89344-105">Eventos recorrentes são uma parte importante do calendário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="89344-105">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="89344-106">Seja uma reunião semanal individual com seu gerente ou uma reunião de revisão de toda a divisão que ocorre na segunda terça-feira de cada mês, eventos recorrentes permitem que o evento seja criado uma fez e que o servidor preencha o restante da série.</span><span class="sxs-lookup"><span data-stu-id="89344-106">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="89344-107">O principal dado que permite que os eventos recorrentes sejam "expandidos" em ocorrências individuais é a regra de recorrência.</span><span class="sxs-lookup"><span data-stu-id="89344-107">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="89344-108">A regra especifica a frequência de repetição do evento e sua duração.</span><span class="sxs-lookup"><span data-stu-id="89344-108">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="89344-109">As regras de recorrência modelam as APIs REST do Outlook na propriedade **recorrência** do [recurso de evento](/graph/api/resources/event?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="89344-109">The Outlook REST APIs model recurrence rules in the **recurrence** property of the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> 

<span data-ttu-id="89344-110">Cada recorrência é composta de duas partes: o padrão de recorrência (frequência) e o intervalo de recorrência (duração).</span><span class="sxs-lookup"><span data-stu-id="89344-110">Each recurrence is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="89344-111">Padrões de recorrência</span><span class="sxs-lookup"><span data-stu-id="89344-111">Recurrence patterns</span></span>

<span data-ttu-id="89344-112">A primeira parte de uma recorrência é o padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-112">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="89344-113">Ele especifica a frequência com que o evento se repete.</span><span class="sxs-lookup"><span data-stu-id="89344-113">This specifies how often the event repeats.</span></span> <span data-ttu-id="89344-114">Por exemplo, um evento poderia repetir "a cada 3 dias", "toda quinta-feira" ou "em 22 de julho de cada ano".</span><span class="sxs-lookup"><span data-stu-id="89344-114">For example, an event could repeat "every 3 days," "every Thursday," or "on July 22 every year."</span></span> <span data-ttu-id="89344-115">Um padrão é representado na API pelo [recurso recurrencePattern](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="89344-115">A pattern is represented in the API by the [recurrencePattern resource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span></span>

<span data-ttu-id="89344-116">Dependendo do tipo de padrão, determinados campos do **recurrencePattern** são obrigatórios, opcionais ou ignorados.</span><span class="sxs-lookup"><span data-stu-id="89344-116">Depending on the type of pattern, certain fields of the **recurrencePattern** are required, optional, or ignored.</span></span>

> <span data-ttu-id="89344-117">**Observação**: Mesmo que um campo seja ignorado, ele ainda é validado.</span><span class="sxs-lookup"><span data-stu-id="89344-117">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="89344-118">Se um campo tiver um conjunto fixo de valores possíveis, usar um valor fora do conjunto permitido causa um erro, mesmo que esse campo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="89344-118">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="89344-119">Vamos dar uma olhada em cada um dos tipos de possíveis de padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-119">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="89344-120">Diariamente</span><span class="sxs-lookup"><span data-stu-id="89344-120">Daily</span></span>

<span data-ttu-id="89344-121">O padrão de recorrência diária faz com que um evento se repita com base em um número de dias entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="89344-121">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="89344-122">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="89344-122">Relevant properties</span></span>

| <span data-ttu-id="89344-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89344-123">Property</span></span> | <span data-ttu-id="89344-124">Relevância</span><span class="sxs-lookup"><span data-stu-id="89344-124">Relevance</span></span> | <span data-ttu-id="89344-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="89344-125">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="89344-126">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="89344-126">**interval**</span></span> | <span data-ttu-id="89344-127">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-127">Required</span></span> | <span data-ttu-id="89344-128">Especifica o número de dias entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="89344-128">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="89344-129">**type**</span><span class="sxs-lookup"><span data-stu-id="89344-129">**type**</span></span> | <span data-ttu-id="89344-130">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-130">Required</span></span> | <span data-ttu-id="89344-131">Tem que ser definida como `daily`.</span><span class="sxs-lookup"><span data-stu-id="89344-131">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="89344-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89344-132">Examples</span></span>

- <span data-ttu-id="89344-133">Repita esse evento todos os dias</span><span class="sxs-lookup"><span data-stu-id="89344-133">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="89344-134">Repita esse evento a cada 3 dias</span><span class="sxs-lookup"><span data-stu-id="89344-134">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="89344-135">Semanalmente</span><span class="sxs-lookup"><span data-stu-id="89344-135">Weekly</span></span>

<span data-ttu-id="89344-136">O padrão de recorrência semanal faz com que um evento se repita no mesmo dia ou dias da semana, com base no número de semanas entre cada conjunto de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="89344-136">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="89344-137">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="89344-137">Relevant properties</span></span>

| <span data-ttu-id="89344-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89344-138">Property</span></span> | <span data-ttu-id="89344-139">Relevância</span><span class="sxs-lookup"><span data-stu-id="89344-139">Relevance</span></span> | <span data-ttu-id="89344-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="89344-140">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="89344-141">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="89344-141">**daysOfWeek**</span></span> | <span data-ttu-id="89344-142">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-142">Required</span></span> | <span data-ttu-id="89344-143">Especifica em quais dias da semana o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="89344-143">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="89344-144">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="89344-144">**firstDayOfWeek**</span></span> | <span data-ttu-id="89344-145">Opcional</span><span class="sxs-lookup"><span data-stu-id="89344-145">Optional</span></span> | <span data-ttu-id="89344-146">Especifica qual dia é considerado o primeiro dia da semana.</span><span class="sxs-lookup"><span data-stu-id="89344-146">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="89344-147">Valor padrão: `Sunday`.</span><span class="sxs-lookup"><span data-stu-id="89344-147">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="89344-148">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="89344-148">**interval**</span></span> | <span data-ttu-id="89344-149">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-149">Required</span></span> | <span data-ttu-id="89344-150">Especifica o número de semanas entre cada conjunto de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="89344-150">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="89344-151">**type**</span><span class="sxs-lookup"><span data-stu-id="89344-151">**type**</span></span> | <span data-ttu-id="89344-152">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-152">Required</span></span> | <span data-ttu-id="89344-153">Tem que ser definida como `weekly`.</span><span class="sxs-lookup"><span data-stu-id="89344-153">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="89344-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89344-154">Examples</span></span>

- <span data-ttu-id="89344-155">Repita esse evento toda quinta-feira</span><span class="sxs-lookup"><span data-stu-id="89344-155">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="89344-156">Repita esse evento em segundas e terças alternadas</span><span class="sxs-lookup"><span data-stu-id="89344-156">Repeat this event every other Monday and Tuesday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 2,
      "daysOfWeek": [
        "Monday",
        "Tuesday"
      ]
    }
  ```

### <a name="absolute-monthly"></a><span data-ttu-id="89344-157">Mensal absoluto</span><span class="sxs-lookup"><span data-stu-id="89344-157">Absolute monthly</span></span>

<span data-ttu-id="89344-158">O padrão mensal absoluto faz com que um evento se repita no mesmo dia do mês (por exemplo, dia 15), com base no número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="89344-158">The absolute monthly pattern causes an event to repeat on the same day of the month (for example, the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="89344-159">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="89344-159">Relevant properties</span></span>

| <span data-ttu-id="89344-160">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89344-160">Property</span></span> | <span data-ttu-id="89344-161">Relevância</span><span class="sxs-lookup"><span data-stu-id="89344-161">Relevance</span></span> | <span data-ttu-id="89344-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="89344-162">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="89344-163">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="89344-163">**dayOfMonth**</span></span> | <span data-ttu-id="89344-164">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-164">Required</span></span> | <span data-ttu-id="89344-165">Especifica em quais dias do mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="89344-165">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="89344-166">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="89344-166">**interval**</span></span> | <span data-ttu-id="89344-167">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-167">Required</span></span> | <span data-ttu-id="89344-168">Especifica o número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="89344-168">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="89344-169">**type**</span><span class="sxs-lookup"><span data-stu-id="89344-169">**type**</span></span> | <span data-ttu-id="89344-170">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-170">Required</span></span> | <span data-ttu-id="89344-171">Tem que ser definida como `absoluteMonthly`.</span><span class="sxs-lookup"><span data-stu-id="89344-171">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="89344-172">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89344-172">Examples</span></span>

- <span data-ttu-id="89344-173">Repita esse evento no 15º dia de cada mês</span><span class="sxs-lookup"><span data-stu-id="89344-173">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="89344-174">Repita esse evento trimestralmente (a cada 3 meses) no dia 7</span><span class="sxs-lookup"><span data-stu-id="89344-174">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="89344-175">Mensal relativo</span><span class="sxs-lookup"><span data-stu-id="89344-175">Relative monthly</span></span>

<span data-ttu-id="89344-176">O padrão mensal relativo faz com que um evento se repita no mesmo dia da semana na mesma posição relativa do mês, com base no número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="89344-176">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="89344-177">Por exemplo, "toda segunda quarta-feira do mês".</span><span class="sxs-lookup"><span data-stu-id="89344-177">For example, "every second Wednesday of the month."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="89344-178">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="89344-178">Relevant properties</span></span>

| <span data-ttu-id="89344-179">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89344-179">Property</span></span> | <span data-ttu-id="89344-180">Relevância</span><span class="sxs-lookup"><span data-stu-id="89344-180">Relevance</span></span> | <span data-ttu-id="89344-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="89344-181">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="89344-182">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="89344-182">**daysOfWeek**</span></span> | <span data-ttu-id="89344-183">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-183">Required</span></span> | <span data-ttu-id="89344-184">Especifica em quais dias da semana o evento pode ocorrer.</span><span class="sxs-lookup"><span data-stu-id="89344-184">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="89344-185">Eventos mensais relativos apenas ocorrerem uma vez por mês, portanto, se mais de um valor for especificado, o evento ocorrerá no primeiro dia que satisfaz o padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-185">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="89344-186">**índice**</span><span class="sxs-lookup"><span data-stu-id="89344-186">**index**</span></span> | <span data-ttu-id="89344-187">Opcional</span><span class="sxs-lookup"><span data-stu-id="89344-187">Optional</span></span> | <span data-ttu-id="89344-188">Especifica em qual instância dos dias permitidos especificados em **daysOfsWeek** o evento ocorre, contando a partir da primeira instância no mês.</span><span class="sxs-lookup"><span data-stu-id="89344-188">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="89344-189">Valores possíveis: `first`, `second`, `third`, `fourth` e `last`.</span><span class="sxs-lookup"><span data-stu-id="89344-189">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="89344-190">Valor padrão: `first`.</span><span class="sxs-lookup"><span data-stu-id="89344-190">Default value: `first`.</span></span> |
| <span data-ttu-id="89344-191">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="89344-191">**interval**</span></span> | <span data-ttu-id="89344-192">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-192">Required</span></span> | <span data-ttu-id="89344-193">Especifica o número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="89344-193">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="89344-194">**type**</span><span class="sxs-lookup"><span data-stu-id="89344-194">**type**</span></span> | <span data-ttu-id="89344-195">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-195">Required</span></span> | <span data-ttu-id="89344-196">Tem que ser definida como `relativeMonthly`.</span><span class="sxs-lookup"><span data-stu-id="89344-196">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="89344-197">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89344-197">Examples</span></span>

- <span data-ttu-id="89344-198">Repita esse evento na segunda quarta-feira de cada mês</span><span class="sxs-lookup"><span data-stu-id="89344-198">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="89344-199">Repita esse evento na primeira quinta ou sexta-feira de cada mês</span><span class="sxs-lookup"><span data-stu-id="89344-199">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="89344-200">Anual absoluto</span><span class="sxs-lookup"><span data-stu-id="89344-200">Absolute yearly</span></span>

<span data-ttu-id="89344-201">O padrão anual absoluto faz com que um evento se repita no mesmo mês e dia (por exemplo, dia 15 de abril), com base no número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="89344-201">The absolute yearly pattern causes an event to repeat on the same month and day (for example, April 15), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="89344-202">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="89344-202">Relevant properties</span></span>

| <span data-ttu-id="89344-203">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89344-203">Property</span></span> | <span data-ttu-id="89344-204">Relevância</span><span class="sxs-lookup"><span data-stu-id="89344-204">Relevance</span></span> | <span data-ttu-id="89344-205">Descrição</span><span class="sxs-lookup"><span data-stu-id="89344-205">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="89344-206">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="89344-206">**dayOfMonth**</span></span> | <span data-ttu-id="89344-207">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-207">Required</span></span> | <span data-ttu-id="89344-208">Especifica em quais dias do mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="89344-208">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="89344-209">**Mês**</span><span class="sxs-lookup"><span data-stu-id="89344-209">**month**</span></span> | <span data-ttu-id="89344-210">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-210">Required</span></span> | <span data-ttu-id="89344-211">Especifica em qual mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="89344-211">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="89344-212">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="89344-212">**interval**</span></span> | <span data-ttu-id="89344-213">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-213">Required</span></span> | <span data-ttu-id="89344-214">Especifica o número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="89344-214">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="89344-215">**type**</span><span class="sxs-lookup"><span data-stu-id="89344-215">**type**</span></span> | <span data-ttu-id="89344-216">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-216">Required</span></span> | <span data-ttu-id="89344-217">Tem que ser definida como `absoluteYearly`.</span><span class="sxs-lookup"><span data-stu-id="89344-217">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="89344-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89344-218">Example</span></span>

- <span data-ttu-id="89344-219">Repita esse evento em 15 de abril todo ano</span><span class="sxs-lookup"><span data-stu-id="89344-219">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="89344-220">Anual relativo</span><span class="sxs-lookup"><span data-stu-id="89344-220">Relative yearly</span></span>

<span data-ttu-id="89344-221">O padrão anual relativo faz com que um evento se repita no mesmo dia da semana na mesma posição relativa de um mês específico, com base no número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="89344-221">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="89344-222">Por exemplo, "toda última quarta-feira de novembro".</span><span class="sxs-lookup"><span data-stu-id="89344-222">For example, "every last Wednesday of November."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="89344-223">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="89344-223">Relevant properties</span></span>

| <span data-ttu-id="89344-224">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89344-224">Property</span></span> | <span data-ttu-id="89344-225">Relevância</span><span class="sxs-lookup"><span data-stu-id="89344-225">Relevance</span></span> | <span data-ttu-id="89344-226">Descrição</span><span class="sxs-lookup"><span data-stu-id="89344-226">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="89344-227">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="89344-227">**daysOfWeek**</span></span> | <span data-ttu-id="89344-228">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-228">Required</span></span> | <span data-ttu-id="89344-229">Especifica em quais dias da semana o evento pode ocorrer.</span><span class="sxs-lookup"><span data-stu-id="89344-229">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="89344-230">Eventos anuais relativos apenas ocorrerem uma vez por ano, portanto, se mais de um valor for especificado, o evento ocorrerá no primeiro dia que satisfaz o padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-230">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="89344-231">**índice**</span><span class="sxs-lookup"><span data-stu-id="89344-231">**index**</span></span> | <span data-ttu-id="89344-232">Opcional</span><span class="sxs-lookup"><span data-stu-id="89344-232">Optional</span></span> | <span data-ttu-id="89344-233">Especifica em qual instância dos dias permitidos especificados em **daysOfsWeek** o evento ocorre, contando a partir da primeira instância no mês.</span><span class="sxs-lookup"><span data-stu-id="89344-233">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="89344-234">Valores possíveis: `first`, `second`, `third`, `fourth` e `last`.</span><span class="sxs-lookup"><span data-stu-id="89344-234">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="89344-235">Valor padrão: `first`.</span><span class="sxs-lookup"><span data-stu-id="89344-235">Default value: `first`.</span></span> |
| <span data-ttu-id="89344-236">**Mês**</span><span class="sxs-lookup"><span data-stu-id="89344-236">**month**</span></span> | <span data-ttu-id="89344-237">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-237">Required</span></span> | <span data-ttu-id="89344-238">Especifica em qual mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="89344-238">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="89344-239">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="89344-239">**interval**</span></span> | <span data-ttu-id="89344-240">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-240">Required</span></span> | <span data-ttu-id="89344-241">Especifica o número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="89344-241">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="89344-242">**type**</span><span class="sxs-lookup"><span data-stu-id="89344-242">**type**</span></span> | <span data-ttu-id="89344-243">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-243">Required</span></span> | <span data-ttu-id="89344-244">Tem que ser definida como `relativeYearly`.</span><span class="sxs-lookup"><span data-stu-id="89344-244">Must be set to `relativeYearly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="89344-245">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89344-245">Examples</span></span>

- <span data-ttu-id="89344-246">Repita esse evento na última quarta-feira de novembro a cada ano</span><span class="sxs-lookup"><span data-stu-id="89344-246">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="89344-247">Intervalos de recorrência</span><span class="sxs-lookup"><span data-stu-id="89344-247">Recurrence ranges</span></span>

<span data-ttu-id="89344-248">A segunda parte de uma recorrência é o intervalo.</span><span class="sxs-lookup"><span data-stu-id="89344-248">The second part of a recurrence is the range.</span></span> <span data-ttu-id="89344-249">Especifica por quanto tempo o padrão se repete.</span><span class="sxs-lookup"><span data-stu-id="89344-249">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="89344-250">Por exemplo, um evento poderia terminar após 10 ocorrências, em uma data específica ou poderia não ter fim.</span><span class="sxs-lookup"><span data-stu-id="89344-250">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="89344-251">Um intervalo é representado na API pelo [recurso recurrenceRange](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="89344-251">A range is represented in the API by the [recurrenceRange resource](/graph/api/resources/recurrencepattern?view=graph-rest-1.0).</span></span>

<span data-ttu-id="89344-252">Dependendo do tipo de intervalo, determinados campos do **recurrenceRange** são obrigatórios ou ignorados.</span><span class="sxs-lookup"><span data-stu-id="89344-252">Depending on the type of range, certain fields of **recurrenceRange** are required or ignored.</span></span>

> <span data-ttu-id="89344-253">**Observação**: Mesmo que um campo seja ignorado, ele ainda é validado.</span><span class="sxs-lookup"><span data-stu-id="89344-253">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="89344-254">Se um campo tiver um conjunto fixo de valores possíveis, usar um valor fora do conjunto permitido causa um erro, mesmo que esse campo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="89344-254">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="89344-255">Vamos dar uma olhada em cada um dos tipos de possíveis de intervalo.</span><span class="sxs-lookup"><span data-stu-id="89344-255">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="89344-256">Intervalo numerado</span><span class="sxs-lookup"><span data-stu-id="89344-256">Numbered range</span></span>

<span data-ttu-id="89344-257">O intervalo numerado faz com que um evento ocorra um número fixo de vezes (com base no padrão) de uma data de início.</span><span class="sxs-lookup"><span data-stu-id="89344-257">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="89344-258">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="89344-258">Relevant properties</span></span>

| <span data-ttu-id="89344-259">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89344-259">Property</span></span> | <span data-ttu-id="89344-260">Relevância</span><span class="sxs-lookup"><span data-stu-id="89344-260">Relevance</span></span> | <span data-ttu-id="89344-261">Descrição</span><span class="sxs-lookup"><span data-stu-id="89344-261">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="89344-262">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="89344-262">**numberOfOccurences**</span></span> | <span data-ttu-id="89344-263">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-263">Required</span></span> | <span data-ttu-id="89344-264">Especifica o número de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="89344-264">Specifies the number of occurrences.</span></span> <span data-ttu-id="89344-265">Deve ser um número inteiro positivo.</span><span class="sxs-lookup"><span data-stu-id="89344-265">Must be a positive integer.</span></span> |
| <span data-ttu-id="89344-266">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="89344-266">**recurrenceTimeZone**</span></span> | <span data-ttu-id="89344-267">Opcional</span><span class="sxs-lookup"><span data-stu-id="89344-267">Optional</span></span> | <span data-ttu-id="89344-268">Especifica o fuso horário para a propriedade **startDate**.</span><span class="sxs-lookup"><span data-stu-id="89344-268">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="89344-269">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="89344-269">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="89344-270">**startDate**</span><span class="sxs-lookup"><span data-stu-id="89344-270">**startDate**</span></span> | <span data-ttu-id="89344-271">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-271">Required</span></span> | <span data-ttu-id="89344-272">Especifica a data para começar a aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-272">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="89344-273">O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](/graph/api/resources/event?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="89344-273">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="89344-274">Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-274">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="89344-275">**type**</span><span class="sxs-lookup"><span data-stu-id="89344-275">**type**</span></span> | <span data-ttu-id="89344-276">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-276">Required</span></span> | <span data-ttu-id="89344-277">Tem que ser definida como `numbered`.</span><span class="sxs-lookup"><span data-stu-id="89344-277">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="89344-278">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89344-278">Examples</span></span>

- <span data-ttu-id="89344-279">Repita esse evento 10 vezes</span><span class="sxs-lookup"><span data-stu-id="89344-279">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="89344-280">Intervalo de datas de término</span><span class="sxs-lookup"><span data-stu-id="89344-280">End date range</span></span>

<span data-ttu-id="89344-281">O intervalo de datas de término faz com que um evento ocorra em todos os dias que se encaixem no padrão aplicável entre uma data de início e uma data de término.</span><span class="sxs-lookup"><span data-stu-id="89344-281">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="89344-282">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="89344-282">Relevant properties</span></span>

| <span data-ttu-id="89344-283">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89344-283">Property</span></span> | <span data-ttu-id="89344-284">Relevância</span><span class="sxs-lookup"><span data-stu-id="89344-284">Relevance</span></span> | <span data-ttu-id="89344-285">Descrição</span><span class="sxs-lookup"><span data-stu-id="89344-285">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="89344-286">**endDate**</span><span class="sxs-lookup"><span data-stu-id="89344-286">**endDate**</span></span> | <span data-ttu-id="89344-287">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-287">Required</span></span> | <span data-ttu-id="89344-288">Especifica a data para parar de aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-288">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="89344-289">Observação: Esta última ocorrência da reunião pode não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-289">Note that the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="89344-290">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="89344-290">**recurrenceTimeZone**</span></span> | <span data-ttu-id="89344-291">Opcional</span><span class="sxs-lookup"><span data-stu-id="89344-291">Optional</span></span> | <span data-ttu-id="89344-292">Especifica o fuso horário das propriedades **startDate** e **endDate**.</span><span class="sxs-lookup"><span data-stu-id="89344-292">Specifies the time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="89344-293">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="89344-293">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="89344-294">**startDate**</span><span class="sxs-lookup"><span data-stu-id="89344-294">**startDate**</span></span> | <span data-ttu-id="89344-295">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-295">Required</span></span> | <span data-ttu-id="89344-296">Especifica a data para começar a aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-296">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="89344-297">O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](/graph/api/resources/event?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="89344-297">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="89344-298">Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-298">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="89344-299">**type**</span><span class="sxs-lookup"><span data-stu-id="89344-299">**type**</span></span> | <span data-ttu-id="89344-300">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-300">Required</span></span> | <span data-ttu-id="89344-301">Tem que ser definida como **endDate**.</span><span class="sxs-lookup"><span data-stu-id="89344-301">Must be set to **endDate**.</span></span> |

#### <a name="examples"></a><span data-ttu-id="89344-302">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89344-302">Examples</span></span>

- <span data-ttu-id="89344-303">Repita esse evento de 1.º de julho de 2017 a 31 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="89344-303">Repeat this event from July 1, 2017, to July 31, 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="89344-304">Intervalo sem término</span><span class="sxs-lookup"><span data-stu-id="89344-304">No end range</span></span>

<span data-ttu-id="89344-305">O intervalo sem término faz com que um evento ocorra em todos os dias que se encaixem no padrão aplicável após uma data de início.</span><span class="sxs-lookup"><span data-stu-id="89344-305">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="89344-306">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="89344-306">Relevant properties</span></span>

| <span data-ttu-id="89344-307">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89344-307">Property</span></span> | <span data-ttu-id="89344-308">Relevância</span><span class="sxs-lookup"><span data-stu-id="89344-308">Relevance</span></span> | <span data-ttu-id="89344-309">Descrição</span><span class="sxs-lookup"><span data-stu-id="89344-309">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="89344-310">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="89344-310">**recurrenceTimeZone**</span></span> | <span data-ttu-id="89344-311">Opcional</span><span class="sxs-lookup"><span data-stu-id="89344-311">Optional</span></span> | <span data-ttu-id="89344-312">Especifica o fuso horário para a propriedade **startDate**.</span><span class="sxs-lookup"><span data-stu-id="89344-312">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="89344-313">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="89344-313">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="89344-314">**startDate**</span><span class="sxs-lookup"><span data-stu-id="89344-314">**startDate**</span></span> | <span data-ttu-id="89344-315">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-315">Required</span></span> | <span data-ttu-id="89344-316">Especifica a data para começar a aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-316">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="89344-317">O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](/graph/api/resources/event?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="89344-317">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](/graph/api/resources/event?view=graph-rest-1.0).</span></span> <span data-ttu-id="89344-318">Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="89344-318">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="89344-319">**type**</span><span class="sxs-lookup"><span data-stu-id="89344-319">**type**</span></span> | <span data-ttu-id="89344-320">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="89344-320">Required</span></span> | <span data-ttu-id="89344-321">Tem que ser definida como `noEnd`.</span><span class="sxs-lookup"><span data-stu-id="89344-321">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="89344-322">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89344-322">Examples</span></span>

- <span data-ttu-id="89344-323">Repita esse evento de 15 de maio de 2017 para sempre</span><span class="sxs-lookup"><span data-stu-id="89344-323">Repeat this event from May 15, 2017, forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="89344-324">Usando padrões e intervalos para criar eventos recorrentes</span><span class="sxs-lookup"><span data-stu-id="89344-324">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="89344-325">Agora que já vimos padrões e intervalos separadamente, vamos analisar como eles funcionam juntos e como eles interagem com as propriedades **iniciar** e **encerrar** do evento.</span><span class="sxs-lookup"><span data-stu-id="89344-325">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **start** and **end** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="89344-326">Criando uma regra de recorrência</span><span class="sxs-lookup"><span data-stu-id="89344-326">Creating a recurrence rule</span></span>

<span data-ttu-id="89344-327">Para criar uma regra de recorrência, você deve especificar um padrão e um intervalo.</span><span class="sxs-lookup"><span data-stu-id="89344-327">To create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="89344-328">Qualquer tipo de padrão pode funcionar com qualquer tipo de intervalo.</span><span class="sxs-lookup"><span data-stu-id="89344-328">Any pattern type can work with any range type.</span></span> <span data-ttu-id="89344-329">Eis alguns exemplos.</span><span class="sxs-lookup"><span data-stu-id="89344-329">Here are a few examples.</span></span>

#### <a name="examples"></a><span data-ttu-id="89344-330">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89344-330">Examples</span></span>

- <span data-ttu-id="89344-331">**Reunião das 13h às 13h30 toda segunda-feira a partir de 4 de setembro de 2017 até o final do ano**</span><span class="sxs-lookup"><span data-stu-id="89344-331">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017, until the end of the year**</span></span>

  - <span data-ttu-id="89344-332">O requisito "toda segunda-feira" requisito é atendido facilmente pelo tipo de padrão de recorrência `weekly`.</span><span class="sxs-lookup"><span data-stu-id="89344-332">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="89344-333">O requisito "até o final do ano" indica um tipo de intervalo de recorrência `endDate`.</span><span class="sxs-lookup"><span data-stu-id="89344-333">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

  ```json
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1,
        "daysOfWeek": [ "Monday" ]
      },
      "range": {
        "type": "endDate",
        "startDate": "2017-09-04",
        "endDate": "2017-12-31"
      }
    }
  ```

  <span data-ttu-id="89344-334">Como 31 de dezembro de 2017 é um domingo, a última ocorrência dessa série será na segunda-feira, dia 25 de dezembro.</span><span class="sxs-lookup"><span data-stu-id="89344-334">Because December 31, 2017, is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="89344-335">**Reunião das 14h às 15h na primeira quinta-feira de cada mês a partir de 29 de agosto de 2017**</span><span class="sxs-lookup"><span data-stu-id="89344-335">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="89344-336">O requisito "primeira quinta-feira de cada mês" pode ser cumprido usando um padrão mensal relativo.</span><span class="sxs-lookup"><span data-stu-id="89344-336">The "first Thursday of every other month" requirement is achievable by using a relative monthly pattern.</span></span> <span data-ttu-id="89344-337">A parte "cada mês" indica que o **intervalo** deve ser definido como `2`.</span><span class="sxs-lookup"><span data-stu-id="89344-337">The "every other month" portion indicates that the **interval** should be set to `2`.</span></span>
  - <span data-ttu-id="89344-338">Por não existir um requisito de data de término, um tipo de intervalo `noEnd` pode ser usado.</span><span class="sxs-lookup"><span data-stu-id="89344-338">Because there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

  ```json
    "recurrence": {
      "pattern": {
        "type": "relativeMonthly",
        "interval": 2,
        "daysOfWeek": [ "Thursday" ],
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "startDate": "2017-08-29"
      }
    }
  ```

  <span data-ttu-id="89344-339">Como o valor de **starDate** é após a primeira quinta-feira de agosto, a primeira ocorrência dessa série será em setembro.</span><span class="sxs-lookup"><span data-stu-id="89344-339">Because the value of **startDate** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="89344-340">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="89344-340">Next steps</span></span>
    
- <span data-ttu-id="89344-341">Veja mais detalhes em [integração com o calendário do Outlook](outlook-calendar-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="89344-341">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
- <span data-ttu-id="89344-342">Visualize outros exemplos de eventos recorrentes na referência da API do calendário:</span><span class="sxs-lookup"><span data-stu-id="89344-342">See other recurring event examples in the calendar API reference:</span></span>
  - [<span data-ttu-id="89344-343">Crie um evento recorrente que ocorra uma vez por semana</span><span class="sxs-lookup"><span data-stu-id="89344-343">Create a recurring event that occurs once a week</span></span>](/graph/api/user-post-events?view=graph-rest-1.0#request-3)
  - [<span data-ttu-id="89344-344">Crie um evento recorrente diário</span><span class="sxs-lookup"><span data-stu-id="89344-344">Create a daily recurring event</span></span>](/graph/api/user-post-events?view=graph-rest-1.0#request-4)

