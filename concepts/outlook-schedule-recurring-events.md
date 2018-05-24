# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="c53a7-101">Agendar compromissos repetidos como eventos recorrentes no Outlook</span><span class="sxs-lookup"><span data-stu-id="c53a7-101">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="c53a7-102">Eventos recorrentes são uma parte importante do calendário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="c53a7-102">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="c53a7-103">Seja uma reunião semanal individual com seu gerente ou uma reunião de revisão de toda a divisão que ocorre na segunda terça-feira de cada mês, eventos recorrentes permitem que o evento seja criado uma fez e que o servidor preencha o restante da série.</span><span class="sxs-lookup"><span data-stu-id="c53a7-103">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="c53a7-104">O principal dado que permite que os eventos recorrentes sejam "expandidos" em ocorrências individuais é a regra de recorrência.</span><span class="sxs-lookup"><span data-stu-id="c53a7-104">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="c53a7-105">A regra especifica a frequência de repetição do evento e sua duração.</span><span class="sxs-lookup"><span data-stu-id="c53a7-105">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="c53a7-106">As regras de recorrência modelam as APIs REST do Outlook na propriedade **recorrência** do [recurso de evento](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="c53a7-106">The Outlook REST APIs model recurrence rules in the **** property of the [event resource](../api-reference/v1.0/resources/event.md).</span></span> 

<span data-ttu-id="c53a7-107">Cada recorrência é composta de duas partes: o padrão de recorrência (frequência) e o intervalo de recorrência (duração).</span><span class="sxs-lookup"><span data-stu-id="c53a7-107">Each  is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="c53a7-108">Padrões de recorrência</span><span class="sxs-lookup"><span data-stu-id="c53a7-108">Recurrence patterns</span></span>

<span data-ttu-id="c53a7-109">A primeira parte de uma recorrência é o padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-109">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="c53a7-110">Ele especifica a frequência com que o evento se repete.</span><span class="sxs-lookup"><span data-stu-id="c53a7-110">This specifies how often the event repeats.</span></span> <span data-ttu-id="c53a7-111">Por exemplo, um evento poderia repetir "a cada 3 dias", "toda quinta-feira" ou "em 22 de julho de cada ano".</span><span class="sxs-lookup"><span data-stu-id="c53a7-111">For example, an event could repeat "every 3 days", "every Thursday", or "on July 22 every year".</span></span> <span data-ttu-id="c53a7-112">Um padrão é representado na API pelo [recurso recurrencePattern](../api-reference/v1.0/resources/recurrencepattern.md).</span><span class="sxs-lookup"><span data-stu-id="c53a7-112">A pattern is represented in the API by the [recurrencePattern resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="c53a7-113">Dependendo do tipo de padrão, determinados campos do **recurrencePattern** são obrigatórios, opcionais ou ignorados.</span><span class="sxs-lookup"><span data-stu-id="c53a7-113">Depending on the type of pattern, certain fields of the **** are required, optional, or ignored.</span></span>

> <span data-ttu-id="c53a7-114">**Observação**: Mesmo que um campo seja ignorado, ele ainda é validado.</span><span class="sxs-lookup"><span data-stu-id="c53a7-114">Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="c53a7-115">Se um campo tiver um conjunto fixo de valores possíveis, usar um valor fora do conjunto permitido causa um erro, mesmo que esse campo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="c53a7-115">If a field has a set list of possible values, using a value outside the allowed set will cause an error, even if that field is ignored.</span></span>

<span data-ttu-id="c53a7-116">Vamos dar uma olhada em cada um dos tipos de possíveis de padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-116">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="c53a7-117">Diariamente</span><span class="sxs-lookup"><span data-stu-id="c53a7-117">Daily</span></span>

<span data-ttu-id="c53a7-118">O padrão de recorrência diária faz com que um evento se repita com base em um número de dias entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="c53a7-118">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c53a7-119">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="c53a7-119">Relevant properties</span></span>

| <span data-ttu-id="c53a7-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c53a7-120">Property</span></span> | <span data-ttu-id="c53a7-121">Relevância</span><span class="sxs-lookup"><span data-stu-id="c53a7-121">Relevance</span></span> | <span data-ttu-id="c53a7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53a7-122">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c53a7-123">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="c53a7-123">**interval**</span></span> | <span data-ttu-id="c53a7-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-124">Required</span></span> | <span data-ttu-id="c53a7-125">Especifica o número de dias entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="c53a7-125">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="c53a7-126">**type**</span><span class="sxs-lookup"><span data-stu-id="c53a7-126">**type**</span></span> | <span data-ttu-id="c53a7-127">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-127">Required</span></span> | <span data-ttu-id="c53a7-128">Tem que ser definida como `daily`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-128">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c53a7-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c53a7-129">Examples</span></span>

- <span data-ttu-id="c53a7-130">Repita esse evento todos os dias</span><span class="sxs-lookup"><span data-stu-id="c53a7-130">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="c53a7-131">Repita esse evento a cada 3 dias</span><span class="sxs-lookup"><span data-stu-id="c53a7-131">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="c53a7-132">Semanalmente</span><span class="sxs-lookup"><span data-stu-id="c53a7-132">Weekly</span></span>

<span data-ttu-id="c53a7-133">O padrão de recorrência semanal faz com que um evento se repita no mesmo dia ou dias da semana, com base no número de semanas entre cada conjunto de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="c53a7-133">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c53a7-134">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="c53a7-134">Relevant properties</span></span>

| <span data-ttu-id="c53a7-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c53a7-135">Property</span></span> | <span data-ttu-id="c53a7-136">Relevância</span><span class="sxs-lookup"><span data-stu-id="c53a7-136">Relevance</span></span> | <span data-ttu-id="c53a7-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53a7-137">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c53a7-138">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="c53a7-138">**daysOfWeek**</span></span> | <span data-ttu-id="c53a7-139">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-139">Required</span></span> | <span data-ttu-id="c53a7-140">Especifica em quais dias da semana o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="c53a7-140">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="c53a7-141">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="c53a7-141">**firstDayOfWeek**</span></span> | <span data-ttu-id="c53a7-142">Opcional</span><span class="sxs-lookup"><span data-stu-id="c53a7-142">Optional</span></span> | <span data-ttu-id="c53a7-143">Especifica qual dia é considerado o primeiro dia da semana.</span><span class="sxs-lookup"><span data-stu-id="c53a7-143">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="c53a7-144">Valor padrão: `Sunday`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-144">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="c53a7-145">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="c53a7-145">**Interval**</span></span> | <span data-ttu-id="c53a7-146">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-146">Required</span></span> | <span data-ttu-id="c53a7-147">Especifica o número de semanas entre cada conjunto de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="c53a7-147">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="c53a7-148">**type**</span><span class="sxs-lookup"><span data-stu-id="c53a7-148">**type**</span></span> | <span data-ttu-id="c53a7-149">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-149">Required</span></span> | <span data-ttu-id="c53a7-150">Tem que ser definida como `weekly`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-150">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c53a7-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c53a7-151">Examples</span></span>

- <span data-ttu-id="c53a7-152">Repita esse evento toda quinta-feira</span><span class="sxs-lookup"><span data-stu-id="c53a7-152">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="c53a7-153">Repita esse evento em segundas e terças alternadas</span><span class="sxs-lookup"><span data-stu-id="c53a7-153">Repeat this event every other Monday and Tuesday</span></span>

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

### <a name="absolute-monthly"></a><span data-ttu-id="c53a7-154">Mensal absoluto</span><span class="sxs-lookup"><span data-stu-id="c53a7-154">Absolute monthly</span></span>

<span data-ttu-id="c53a7-155">O padrão mensal absoluto faz com que um evento se repita no mesmo dia do mês (por exemplo, dia 15), com base no número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="c53a7-155">The absolute monthly pattern causes an event to repeat on the same day of the month (e.g. the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c53a7-156">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="c53a7-156">Relevant properties</span></span>

| <span data-ttu-id="c53a7-157">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c53a7-157">Property</span></span> | <span data-ttu-id="c53a7-158">Relevância</span><span class="sxs-lookup"><span data-stu-id="c53a7-158">Relevance</span></span> | <span data-ttu-id="c53a7-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53a7-159">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c53a7-160">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="c53a7-160">**dayOfMonth**</span></span> | <span data-ttu-id="c53a7-161">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-161">Required</span></span> | <span data-ttu-id="c53a7-162">Especifica em quais dias do mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="c53a7-162">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="c53a7-163">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="c53a7-163">**Interval**</span></span> | <span data-ttu-id="c53a7-164">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-164">Required</span></span> | <span data-ttu-id="c53a7-165">Especifica o número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="c53a7-165">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="c53a7-166">**type**</span><span class="sxs-lookup"><span data-stu-id="c53a7-166">**type**</span></span> | <span data-ttu-id="c53a7-167">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-167">Required</span></span> | <span data-ttu-id="c53a7-168">Tem que ser definida como `absoluteMonthly`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-168">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c53a7-169">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c53a7-169">Examples</span></span>

- <span data-ttu-id="c53a7-170">Repita esse evento no 15º dia de cada mês</span><span class="sxs-lookup"><span data-stu-id="c53a7-170">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="c53a7-171">Repita esse evento trimestralmente (a cada 3 meses) no dia 7</span><span class="sxs-lookup"><span data-stu-id="c53a7-171">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="c53a7-172">Mensal relativo</span><span class="sxs-lookup"><span data-stu-id="c53a7-172">Relative monthly</span></span>

<span data-ttu-id="c53a7-173">O padrão mensal relativo faz com que um evento se repita no mesmo dia da semana na mesma posição relativa do mês, com base no número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="c53a7-173">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="c53a7-174">Por exemplo, "toda segunda quarta-feira do mês".</span><span class="sxs-lookup"><span data-stu-id="c53a7-174">For example, "every second Wednesday of the month".</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c53a7-175">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="c53a7-175">Relevant properties</span></span>

| <span data-ttu-id="c53a7-176">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c53a7-176">Property</span></span> | <span data-ttu-id="c53a7-177">Relevância</span><span class="sxs-lookup"><span data-stu-id="c53a7-177">Relevance</span></span> | <span data-ttu-id="c53a7-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53a7-178">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c53a7-179">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="c53a7-179">**daysOfWeek**</span></span> | <span data-ttu-id="c53a7-180">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-180">Required</span></span> | <span data-ttu-id="c53a7-181">Especifica em quais dias da semana o evento pode ocorrer.</span><span class="sxs-lookup"><span data-stu-id="c53a7-181">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="c53a7-182">Eventos mensais relativos apenas ocorrerem uma vez por mês, portanto, se mais de um valor for especificado, o evento ocorrerá no primeiro dia que satisfaz o padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-182">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="c53a7-183">**índice**</span><span class="sxs-lookup"><span data-stu-id="c53a7-183">**index**</span></span> | <span data-ttu-id="c53a7-184">Opcional</span><span class="sxs-lookup"><span data-stu-id="c53a7-184">Optional</span></span> | <span data-ttu-id="c53a7-185">Especifica em qual instância dos dias permitidos especificados em **daysOfsWeek** o evento ocorre, contando a partir da primeira instância no mês.</span><span class="sxs-lookup"><span data-stu-id="c53a7-185">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="c53a7-186">Valores possíveis: `first`, `second`, `third`, `fourth` e `last`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-186">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="c53a7-187">Valor padrão: `first`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-187">Default value: `first`.</span></span> |
| <span data-ttu-id="c53a7-188">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="c53a7-188">**Interval**</span></span> | <span data-ttu-id="c53a7-189">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-189">Required</span></span> | <span data-ttu-id="c53a7-190">Especifica o número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="c53a7-190">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="c53a7-191">**type**</span><span class="sxs-lookup"><span data-stu-id="c53a7-191">**type**</span></span> | <span data-ttu-id="c53a7-192">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-192">Required</span></span> | <span data-ttu-id="c53a7-193">Tem que ser definida como `relativeMonthly`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-193">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c53a7-194">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c53a7-194">Examples</span></span>

- <span data-ttu-id="c53a7-195">Repita esse evento na segunda quarta-feira de cada mês</span><span class="sxs-lookup"><span data-stu-id="c53a7-195">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="c53a7-196">Repita esse evento na primeira quinta ou sexta-feira de cada mês</span><span class="sxs-lookup"><span data-stu-id="c53a7-196">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="c53a7-197">Anual absoluto</span><span class="sxs-lookup"><span data-stu-id="c53a7-197">Absolute yearly</span></span>

<span data-ttu-id="c53a7-198">O padrão anual absoluto faz com que um evento se repita no mesmo mês e dia (por exemplo, dia 15 de abril), com base no número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="c53a7-198">The absolute yearly pattern causes an event to repeat on the same month and day (e.g. April 15th), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c53a7-199">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="c53a7-199">Relevant properties</span></span>

| <span data-ttu-id="c53a7-200">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c53a7-200">Property</span></span> | <span data-ttu-id="c53a7-201">Relevância</span><span class="sxs-lookup"><span data-stu-id="c53a7-201">Relevance</span></span> | <span data-ttu-id="c53a7-202">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53a7-202">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c53a7-203">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="c53a7-203">**dayOfMonth**</span></span> | <span data-ttu-id="c53a7-204">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-204">Required</span></span> | <span data-ttu-id="c53a7-205">Especifica em quais dias do mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="c53a7-205">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="c53a7-206">**Mês**</span><span class="sxs-lookup"><span data-stu-id="c53a7-206">**month**</span></span> | <span data-ttu-id="c53a7-207">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-207">Required</span></span> | <span data-ttu-id="c53a7-208">Especifica em qual mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="c53a7-208">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="c53a7-209">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="c53a7-209">**Interval**</span></span> | <span data-ttu-id="c53a7-210">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-210">Required</span></span> | <span data-ttu-id="c53a7-211">Especifica o número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="c53a7-211">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="c53a7-212">**type**</span><span class="sxs-lookup"><span data-stu-id="c53a7-212">**type**</span></span> | <span data-ttu-id="c53a7-213">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-213">Required</span></span> | <span data-ttu-id="c53a7-214">Tem que ser definida como `absoluteYearly`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-214">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="c53a7-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c53a7-215">Example</span></span>

- <span data-ttu-id="c53a7-216">Repita esse evento em 15 de abril todo ano</span><span class="sxs-lookup"><span data-stu-id="c53a7-216">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="c53a7-217">Anual relativo</span><span class="sxs-lookup"><span data-stu-id="c53a7-217">Relative yearly</span></span>

<span data-ttu-id="c53a7-218">O padrão anual relativo faz com que um evento se repita no mesmo dia da semana na mesma posição relativa de um mês específico, com base no número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="c53a7-218">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="c53a7-219">Por exemplo, "toda última quarta-feira de novembro".</span><span class="sxs-lookup"><span data-stu-id="c53a7-219">For example, "every last Wednesday of November".</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c53a7-220">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="c53a7-220">Relevant properties</span></span>

| <span data-ttu-id="c53a7-221">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c53a7-221">Property</span></span> | <span data-ttu-id="c53a7-222">Relevância</span><span class="sxs-lookup"><span data-stu-id="c53a7-222">Relevance</span></span> | <span data-ttu-id="c53a7-223">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53a7-223">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c53a7-224">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="c53a7-224">**daysOfWeek**</span></span> | <span data-ttu-id="c53a7-225">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-225">Required</span></span> | <span data-ttu-id="c53a7-226">Especifica em quais dias da semana o evento pode ocorrer.</span><span class="sxs-lookup"><span data-stu-id="c53a7-226">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="c53a7-227">Eventos anuais relativos apenas ocorrerem uma vez por ano, portanto, se mais de um valor for especificado, o evento ocorrerá no primeiro dia que satisfaz o padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-227">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="c53a7-228">**índice**</span><span class="sxs-lookup"><span data-stu-id="c53a7-228">**index**</span></span> | <span data-ttu-id="c53a7-229">Opcional</span><span class="sxs-lookup"><span data-stu-id="c53a7-229">Optional</span></span> | <span data-ttu-id="c53a7-230">Especifica em qual instância dos dias permitidos especificados em **daysOfsWeek** o evento ocorre, contando a partir da primeira instância no mês.</span><span class="sxs-lookup"><span data-stu-id="c53a7-230">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="c53a7-231">Valores possíveis: `first`, `second`, `third`, `fourth` e `last`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-231">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="c53a7-232">Valor padrão: `first`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-232">Default value: `first`.</span></span> |
| <span data-ttu-id="c53a7-233">**Mês**</span><span class="sxs-lookup"><span data-stu-id="c53a7-233">**month**</span></span> | <span data-ttu-id="c53a7-234">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-234">Required</span></span> | <span data-ttu-id="c53a7-235">Especifica em qual mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="c53a7-235">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="c53a7-236">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="c53a7-236">**Interval**</span></span> | <span data-ttu-id="c53a7-237">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-237">Required</span></span> | <span data-ttu-id="c53a7-238">Especifica o número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="c53a7-238">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="c53a7-239">**type**</span><span class="sxs-lookup"><span data-stu-id="c53a7-239">**type**</span></span> | <span data-ttu-id="c53a7-240">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-240">Required</span></span> | <span data-ttu-id="c53a7-241">Tem que ser definida como `relativeMonthly`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-241">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c53a7-242">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c53a7-242">Examples</span></span>

- <span data-ttu-id="c53a7-243">Repita esse evento na última quarta-feira de novembro a cada ano</span><span class="sxs-lookup"><span data-stu-id="c53a7-243">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="c53a7-244">Intervalos de recorrência</span><span class="sxs-lookup"><span data-stu-id="c53a7-244">Recurrence ranges</span></span>

<span data-ttu-id="c53a7-245">A segunda parte de uma recorrência é o intervalo.</span><span class="sxs-lookup"><span data-stu-id="c53a7-245">The second part of a recurrence is the range.</span></span> <span data-ttu-id="c53a7-246">Especifica por quanto tempo o padrão se repete.</span><span class="sxs-lookup"><span data-stu-id="c53a7-246">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="c53a7-247">Por exemplo, um evento poderia terminar após 10 ocorrências, em uma data específica ou poderia não ter fim.</span><span class="sxs-lookup"><span data-stu-id="c53a7-247">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="c53a7-248">Um intervalo é representado na API pelo [recurso recurrenceRange](../api-reference/v1.0/resources/recurrencepattern.md).</span><span class="sxs-lookup"><span data-stu-id="c53a7-248">A range is represented in the API by the [recurrenceRange resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="c53a7-249">Dependendo do tipo de intervalo, determinados campos do **recurrenceRange** são obrigatórios ou ignorados.</span><span class="sxs-lookup"><span data-stu-id="c53a7-249">Depending on the type of range, certain fields of the **** are required or ignored.</span></span>

> <span data-ttu-id="c53a7-250">**Observação**: Mesmo que um campo seja ignorado, ele ainda é validado.</span><span class="sxs-lookup"><span data-stu-id="c53a7-250">Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="c53a7-251">Se um campo tiver um conjunto fixo de valores possíveis, usar um valor fora do conjunto permitido causa um erro, mesmo que esse campo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="c53a7-251">If a field has a set list of possible values, using a value outside the allowed set will cause an error, even if that field is ignored.</span></span>

<span data-ttu-id="c53a7-252">Vamos dar uma olhada em cada um dos tipos de possíveis de intervalo.</span><span class="sxs-lookup"><span data-stu-id="c53a7-252">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="c53a7-253">Intervalo numerado</span><span class="sxs-lookup"><span data-stu-id="c53a7-253">Numbered range</span></span>

<span data-ttu-id="c53a7-254">O intervalo numerado faz com que um evento ocorra um número fixo de vezes (com base no padrão) de uma data de início.</span><span class="sxs-lookup"><span data-stu-id="c53a7-254">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c53a7-255">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="c53a7-255">Relevant properties</span></span>

| <span data-ttu-id="c53a7-256">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c53a7-256">Property</span></span> | <span data-ttu-id="c53a7-257">Relevância</span><span class="sxs-lookup"><span data-stu-id="c53a7-257">Relevance</span></span> | <span data-ttu-id="c53a7-258">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53a7-258">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c53a7-259">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="c53a7-259">**numberOfOccurences**</span></span> | <span data-ttu-id="c53a7-260">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-260">Required</span></span> | <span data-ttu-id="c53a7-261">Especifica o número de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="c53a7-261">Specifies the number of occurrences.</span></span> <span data-ttu-id="c53a7-262">Deve ser um número inteiro positivo.</span><span class="sxs-lookup"><span data-stu-id="c53a7-262">Must be a positive integer.</span></span> |
| <span data-ttu-id="c53a7-263">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="c53a7-263">**recurrenceTimeZone**</span></span> | <span data-ttu-id="c53a7-264">Opcional</span><span class="sxs-lookup"><span data-stu-id="c53a7-264">Optional</span></span> | <span data-ttu-id="c53a7-265">Especifica o fuso horário para a propriedade **startDate**.</span><span class="sxs-lookup"><span data-stu-id="c53a7-265">Specifies the time zone for the **** property.</span></span> <span data-ttu-id="c53a7-266">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="c53a7-266">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="c53a7-267">**startDate**</span><span class="sxs-lookup"><span data-stu-id="c53a7-267">**startDate**</span></span> | <span data-ttu-id="c53a7-268">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-268">Required</span></span> | <span data-ttu-id="c53a7-269">Especifica a data para começar a aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-269">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="c53a7-270">O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="c53a7-270">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="c53a7-271">Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-271">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="c53a7-272">**type**</span><span class="sxs-lookup"><span data-stu-id="c53a7-272">**type**</span></span> | <span data-ttu-id="c53a7-273">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-273">Required</span></span> | <span data-ttu-id="c53a7-274">Tem que ser definida como `numbered`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-274">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c53a7-275">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c53a7-275">Examples</span></span>

- <span data-ttu-id="c53a7-276">Repita esse evento 10 vezes</span><span class="sxs-lookup"><span data-stu-id="c53a7-276">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="c53a7-277">Intervalo de datas de término</span><span class="sxs-lookup"><span data-stu-id="c53a7-277">End date range</span></span>

<span data-ttu-id="c53a7-278">O intervalo de datas de término faz com que um evento ocorra em todos os dias que se encaixem no padrão aplicável entre uma data de início e uma data de término.</span><span class="sxs-lookup"><span data-stu-id="c53a7-278">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c53a7-279">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="c53a7-279">Relevant properties</span></span>

| <span data-ttu-id="c53a7-280">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c53a7-280">Property</span></span> | <span data-ttu-id="c53a7-281">Relevância</span><span class="sxs-lookup"><span data-stu-id="c53a7-281">Relevance</span></span> | <span data-ttu-id="c53a7-282">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53a7-282">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c53a7-283">**endDate**</span><span class="sxs-lookup"><span data-stu-id="c53a7-283">**endDate**</span></span> | <span data-ttu-id="c53a7-284">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-284">Required</span></span> | <span data-ttu-id="c53a7-285">Especifica a data para parar de aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-285">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="c53a7-286">Observação: Esta última ocorrência da reunião pode não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-286">Note: the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="c53a7-287">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="c53a7-287">**recurrenceTimeZone**</span></span> | <span data-ttu-id="c53a7-288">Opcional</span><span class="sxs-lookup"><span data-stu-id="c53a7-288">Optional</span></span> | <span data-ttu-id="c53a7-289">Especifica o fuso horário das propriedades **startDate** e **endDate**.</span><span class="sxs-lookup"><span data-stu-id="c53a7-289">Specifies the time zone for the **** and **** properties.</span></span> <span data-ttu-id="c53a7-290">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="c53a7-290">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="c53a7-291">**startDate**</span><span class="sxs-lookup"><span data-stu-id="c53a7-291">**startDate**</span></span> | <span data-ttu-id="c53a7-292">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-292">Required</span></span> | <span data-ttu-id="c53a7-293">Especifica a data para começar a aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-293">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="c53a7-294">O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="c53a7-294">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="c53a7-295">Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-295">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="c53a7-296">**type**</span><span class="sxs-lookup"><span data-stu-id="c53a7-296">**type**</span></span> | <span data-ttu-id="c53a7-297">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-297">Required</span></span> | <span data-ttu-id="c53a7-298">Tem que ser definida como **endDate**.</span><span class="sxs-lookup"><span data-stu-id="c53a7-298">Must be set to ****.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c53a7-299">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c53a7-299">Examples</span></span>

- <span data-ttu-id="c53a7-300">Repita esse evento de 1.º de julho de 2017 a 31 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="c53a7-300">Repeat this event from July 1 2017 to July 31 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="c53a7-301">Intervalo sem término</span><span class="sxs-lookup"><span data-stu-id="c53a7-301">No end range</span></span>

<span data-ttu-id="c53a7-302">O intervalo sem término faz com que um evento ocorra em todos os dias que se encaixem no padrão aplicável após uma data de início.</span><span class="sxs-lookup"><span data-stu-id="c53a7-302">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="c53a7-303">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="c53a7-303">Relevant properties</span></span>

| <span data-ttu-id="c53a7-304">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c53a7-304">Property</span></span> | <span data-ttu-id="c53a7-305">Relevância</span><span class="sxs-lookup"><span data-stu-id="c53a7-305">Relevance</span></span> | <span data-ttu-id="c53a7-306">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53a7-306">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="c53a7-307">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="c53a7-307">**recurrenceTimeZone**</span></span> | <span data-ttu-id="c53a7-308">Opcional</span><span class="sxs-lookup"><span data-stu-id="c53a7-308">Optional</span></span> | <span data-ttu-id="c53a7-309">Especifica o fuso horário para a propriedade **startDate**.</span><span class="sxs-lookup"><span data-stu-id="c53a7-309">Specifies the time zone for the **** property.</span></span> <span data-ttu-id="c53a7-310">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="c53a7-310">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="c53a7-311">**startDate**</span><span class="sxs-lookup"><span data-stu-id="c53a7-311">**startDate**</span></span> | <span data-ttu-id="c53a7-312">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-312">Required</span></span> | <span data-ttu-id="c53a7-313">Especifica a data para começar a aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-313">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="c53a7-314">O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="c53a7-314">The value of **** MUST correspond to the date value of the **** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="c53a7-315">Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="c53a7-315">Note: the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="c53a7-316">**type**</span><span class="sxs-lookup"><span data-stu-id="c53a7-316">**type**</span></span> | <span data-ttu-id="c53a7-317">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c53a7-317">Required</span></span> | <span data-ttu-id="c53a7-318">Tem que ser definida como `noEnd`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-318">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="c53a7-319">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c53a7-319">Examples</span></span>

- <span data-ttu-id="c53a7-320">Repita esse evento de 15 de maio de 2017 para sempre</span><span class="sxs-lookup"><span data-stu-id="c53a7-320">Repeat this event from May 15 2017 forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="c53a7-321">Usando padrões e intervalos para criar eventos recorrentes</span><span class="sxs-lookup"><span data-stu-id="c53a7-321">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="c53a7-322">Agora que já vimos padrões e intervalos separadamente, vamos analisar como eles funcionam juntos e como eles interagem com as propriedades **iniciar** e **encerrar** do evento.</span><span class="sxs-lookup"><span data-stu-id="c53a7-322">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **** and **** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="c53a7-323">Criando uma regra de recorrência</span><span class="sxs-lookup"><span data-stu-id="c53a7-323">Creating a recurrence rule</span></span>

<span data-ttu-id="c53a7-324">Para criar uma regra de recorrência, você deve especificar um padrão e um intervalo.</span><span class="sxs-lookup"><span data-stu-id="c53a7-324">In order to create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="c53a7-325">Qualquer tipo de padrão pode funcionar com qualquer tipo de intervalo.</span><span class="sxs-lookup"><span data-stu-id="c53a7-325">Any pattern type can work with any range type.</span></span> <span data-ttu-id="c53a7-326">Eis alguns exemplos.</span><span class="sxs-lookup"><span data-stu-id="c53a7-326">Here are a few suggestions:</span></span>

#### <a name="examples"></a><span data-ttu-id="c53a7-327">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c53a7-327">Examples</span></span>

- <span data-ttu-id="c53a7-328">**Reunião das 13h às 13h30 toda segunda-feira a partir de 4 de setembro de 2017 até o final do ano**</span><span class="sxs-lookup"><span data-stu-id="c53a7-328">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017 until the end of the year**</span></span>

  - <span data-ttu-id="c53a7-329">O requisito "toda segunda-feira" requisito é atendido facilmente pelo tipo de padrão de recorrência `weekly`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-329">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="c53a7-330">O requisito "até o final do ano" indica um tipo de intervalo de recorrência `endDate`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-330">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

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

  <span data-ttu-id="c53a7-331">Como 31 de dezembro de 2017 é um domingo, a última ocorrência dessa série será na segunda-feira, dia 25 de dezembro.</span><span class="sxs-lookup"><span data-stu-id="c53a7-331">Because December 31, 2017 is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="c53a7-332">**Reunião das 14h às 15h na primeira quinta-feira de cada mês a partir de 29 de agosto de 2017**</span><span class="sxs-lookup"><span data-stu-id="c53a7-332">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="c53a7-333">O requisito "primeira quinta-feira de cada mês" pode ser cumprido usando um padrão mensal relativo.</span><span class="sxs-lookup"><span data-stu-id="c53a7-333">The "first Thursday of every other month" requirement is achievable using a relative monthly pattern.</span></span> <span data-ttu-id="c53a7-334">A parte "cada mês" indica que o **intervalo** deve ser definido como `2`.</span><span class="sxs-lookup"><span data-stu-id="c53a7-334">The "every other month" portion indicates the **** should be set to `2`.</span></span>
  - <span data-ttu-id="c53a7-335">Por não existir um requisito de data de término, um tipo de intervalo `noEnd` pode ser usado.</span><span class="sxs-lookup"><span data-stu-id="c53a7-335">Since there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

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

  <span data-ttu-id="c53a7-336">Como o valor de **starDate** é após a primeira quinta-feira de agosto, a primeira ocorrência dessa série será em setembro.</span><span class="sxs-lookup"><span data-stu-id="c53a7-336">Because the value of **** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c53a7-337">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="c53a7-337">Next steps</span></span>
    
<span data-ttu-id="c53a7-338">Veja mais detalhes em [integração com o calendário do Outlook](outlook-calendar-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c53a7-338">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
