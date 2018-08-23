# <a name="schedule-repeating-appointments-as-recurring-events-in-outlook"></a><span data-ttu-id="4645c-101">Agendar compromissos repetidos como eventos recorrentes no Outlook</span><span class="sxs-lookup"><span data-stu-id="4645c-101">Schedule repeating appointments as recurring events in Outlook</span></span>

<span data-ttu-id="4645c-102">Eventos recorrentes são uma parte importante do calendário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="4645c-102">Recurring events are an important part of Outlook calendaring.</span></span> <span data-ttu-id="4645c-103">Seja uma reunião semanal individual com seu gerente ou uma reunião de revisão de toda a divisão que ocorre na segunda terça-feira de cada mês, eventos recorrentes permitem que o evento seja criado uma fez e que o servidor preencha o restante da série.</span><span class="sxs-lookup"><span data-stu-id="4645c-103">Whether it's a weekly one-on-one meeting with your manager, or a division-wide review meeting that happens on the second Tuesday of each month, recurring events make it easy to create the event once, and let the server fill in the rest of the series.</span></span>

<span data-ttu-id="4645c-104">O principal dado que permite que os eventos recorrentes sejam "expandidos" em ocorrências individuais é a regra de recorrência.</span><span class="sxs-lookup"><span data-stu-id="4645c-104">The key bit of information that allows recurring events to "expand" into individual occurrences is the recurrence rule.</span></span> <span data-ttu-id="4645c-105">A regra especifica a frequência de repetição do evento e sua duração.</span><span class="sxs-lookup"><span data-stu-id="4645c-105">The rule specifies both how often an event repeats, and for how long.</span></span> <span data-ttu-id="4645c-106">As regras de recorrência modelam as APIs REST do Outlook na propriedade **recorrência** do [recurso de evento](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="4645c-106">The Outlook REST APIs model recurrence rules in the **recurrence** property of the [event resource](../api-reference/v1.0/resources/event.md).</span></span> 

<span data-ttu-id="4645c-107">Cada recorrência é composta de duas partes: o padrão de recorrência (frequência) e o intervalo de recorrência (duração).</span><span class="sxs-lookup"><span data-stu-id="4645c-107">Each recurrence is made up of two parts: the recurrence pattern (how often), and the recurrence range (for how long).</span></span>

## <a name="recurrence-patterns"></a><span data-ttu-id="4645c-108">Padrões de recorrência</span><span class="sxs-lookup"><span data-stu-id="4645c-108">Recurrence patterns</span></span>

<span data-ttu-id="4645c-109">A primeira parte de uma recorrência é o padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-109">The first part of a recurrence is the pattern.</span></span> <span data-ttu-id="4645c-110">Ele especifica a frequência com que o evento se repete.</span><span class="sxs-lookup"><span data-stu-id="4645c-110">This specifies how often the event repeats.</span></span> <span data-ttu-id="4645c-111">Por exemplo, um evento poderia repetir "a cada 3 dias", "toda quinta-feira" ou "em 22 de julho de cada ano".</span><span class="sxs-lookup"><span data-stu-id="4645c-111">For example, an event could repeat "every 3 days," "every Thursday," or "on July 22 every year."</span></span> <span data-ttu-id="4645c-112">Um padrão é representado na API pelo [recurso recurrencePattern](../api-reference/v1.0/resources/recurrencepattern.md).</span><span class="sxs-lookup"><span data-stu-id="4645c-112">A pattern is represented in the API by the [recurrencePattern resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="4645c-113">Dependendo do tipo de padrão, determinados campos do **recurrencePattern** são obrigatórios, opcionais ou ignorados.</span><span class="sxs-lookup"><span data-stu-id="4645c-113">Depending on the type of pattern, certain fields of the **recurrencePattern** are required, optional, or ignored.</span></span>

> <span data-ttu-id="4645c-114">**Observação**: Mesmo que um campo seja ignorado, ele ainda é validado.</span><span class="sxs-lookup"><span data-stu-id="4645c-114">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="4645c-115">Se um campo tiver um conjunto fixo de valores possíveis, usar um valor fora do conjunto permitido causa um erro, mesmo que esse campo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="4645c-115">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="4645c-116">Vamos dar uma olhada em cada um dos tipos de possíveis de padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-116">Let's take a look at each of the possible pattern types.</span></span>

### <a name="daily"></a><span data-ttu-id="4645c-117">Diariamente</span><span class="sxs-lookup"><span data-stu-id="4645c-117">Daily</span></span>

<span data-ttu-id="4645c-118">O padrão de recorrência diária faz com que um evento se repita com base em um número de dias entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="4645c-118">The daily recurrence pattern causes an event to repeat based on a number of days between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="4645c-119">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="4645c-119">Relevant properties</span></span>

| <span data-ttu-id="4645c-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4645c-120">Property</span></span> | <span data-ttu-id="4645c-121">Relevância</span><span class="sxs-lookup"><span data-stu-id="4645c-121">Relevance</span></span> | <span data-ttu-id="4645c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4645c-122">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="4645c-123">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="4645c-123">**interval**</span></span> | <span data-ttu-id="4645c-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-124">Required</span></span> | <span data-ttu-id="4645c-125">Especifica o número de dias entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="4645c-125">Specifies the number of days between each occurrence.</span></span> |
| <span data-ttu-id="4645c-126">**type**</span><span class="sxs-lookup"><span data-stu-id="4645c-126">**type**</span></span> | <span data-ttu-id="4645c-127">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-127">Required</span></span> | <span data-ttu-id="4645c-128">Tem que ser definida como `daily`.</span><span class="sxs-lookup"><span data-stu-id="4645c-128">Must be set to `daily`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="4645c-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4645c-129">Examples</span></span>

- <span data-ttu-id="4645c-130">Repita esse evento todos os dias</span><span class="sxs-lookup"><span data-stu-id="4645c-130">Repeat this event every day</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 1
    }
  ```
- <span data-ttu-id="4645c-131">Repita esse evento a cada 3 dias</span><span class="sxs-lookup"><span data-stu-id="4645c-131">Repeat this event every three days</span></span>

  ```json
    "pattern": {
      "type": "daily",
      "interval": 3
    }
  ```

### <a name="weekly"></a><span data-ttu-id="4645c-132">Semanalmente</span><span class="sxs-lookup"><span data-stu-id="4645c-132">Weekly</span></span>

<span data-ttu-id="4645c-133">O padrão de recorrência semanal faz com que um evento se repita no mesmo dia ou dias da semana, com base no número de semanas entre cada conjunto de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="4645c-133">The weekly recurrence pattern causes an event to repeat on the same day or days of the week, based on the number of weeks between each set of occurrences.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="4645c-134">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="4645c-134">Relevant properties</span></span>

| <span data-ttu-id="4645c-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4645c-135">Property</span></span> | <span data-ttu-id="4645c-136">Relevância</span><span class="sxs-lookup"><span data-stu-id="4645c-136">Relevance</span></span> | <span data-ttu-id="4645c-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="4645c-137">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="4645c-138">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="4645c-138">**daysOfWeek**</span></span> | <span data-ttu-id="4645c-139">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-139">Required</span></span> | <span data-ttu-id="4645c-140">Especifica em quais dias da semana o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="4645c-140">Specifies on which day(s) of the week the event occurs.</span></span> |
| <span data-ttu-id="4645c-141">**firstDayOfWeek**</span><span class="sxs-lookup"><span data-stu-id="4645c-141">**firstDayOfWeek**</span></span> | <span data-ttu-id="4645c-142">Opcional</span><span class="sxs-lookup"><span data-stu-id="4645c-142">Optional</span></span> | <span data-ttu-id="4645c-143">Especifica qual dia é considerado o primeiro dia da semana.</span><span class="sxs-lookup"><span data-stu-id="4645c-143">Specifies which day is considered the first day of the week.</span></span> <span data-ttu-id="4645c-144">Valor padrão: `Sunday`.</span><span class="sxs-lookup"><span data-stu-id="4645c-144">Default value: `Sunday`.</span></span> |
| <span data-ttu-id="4645c-145">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="4645c-145">**interval**</span></span> | <span data-ttu-id="4645c-146">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-146">Required</span></span> | <span data-ttu-id="4645c-147">Especifica o número de semanas entre cada conjunto de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="4645c-147">Specifies the number of weeks between each set of occurrences.</span></span> |
| <span data-ttu-id="4645c-148">**type**</span><span class="sxs-lookup"><span data-stu-id="4645c-148">**type**</span></span> | <span data-ttu-id="4645c-149">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-149">Required</span></span> | <span data-ttu-id="4645c-150">Tem que ser definida como `weekly`.</span><span class="sxs-lookup"><span data-stu-id="4645c-150">Must be set to `weekly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="4645c-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4645c-151">Examples</span></span>

- <span data-ttu-id="4645c-152">Repita esse evento toda quinta-feira</span><span class="sxs-lookup"><span data-stu-id="4645c-152">Repeat this event every Thursday</span></span>

  ```json
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Thursday" ]
    }
  ```
- <span data-ttu-id="4645c-153">Repita esse evento em segundas e terças alternadas</span><span class="sxs-lookup"><span data-stu-id="4645c-153">Repeat this event every other Monday and Tuesday</span></span>

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

### <a name="absolute-monthly"></a><span data-ttu-id="4645c-154">Mensal absoluto</span><span class="sxs-lookup"><span data-stu-id="4645c-154">Absolute monthly</span></span>

<span data-ttu-id="4645c-155">O padrão mensal absoluto faz com que um evento se repita no mesmo dia do mês (por exemplo, dia 15), com base no número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="4645c-155">The absolute monthly pattern causes an event to repeat on the same day of the month (for example, the 15th), based on the number of months between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="4645c-156">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="4645c-156">Relevant properties</span></span>

| <span data-ttu-id="4645c-157">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4645c-157">Property</span></span> | <span data-ttu-id="4645c-158">Relevância</span><span class="sxs-lookup"><span data-stu-id="4645c-158">Relevance</span></span> | <span data-ttu-id="4645c-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="4645c-159">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="4645c-160">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="4645c-160">**dayOfMonth**</span></span> | <span data-ttu-id="4645c-161">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-161">Required</span></span> | <span data-ttu-id="4645c-162">Especifica em quais dias do mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="4645c-162">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="4645c-163">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="4645c-163">**interval**</span></span> | <span data-ttu-id="4645c-164">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-164">Required</span></span> | <span data-ttu-id="4645c-165">Especifica o número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="4645c-165">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="4645c-166">**type**</span><span class="sxs-lookup"><span data-stu-id="4645c-166">**type**</span></span> | <span data-ttu-id="4645c-167">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-167">Required</span></span> | <span data-ttu-id="4645c-168">Tem que ser definida como `absoluteMonthly`.</span><span class="sxs-lookup"><span data-stu-id="4645c-168">Must be set to `absoluteMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="4645c-169">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4645c-169">Examples</span></span>

- <span data-ttu-id="4645c-170">Repita esse evento no 15º dia de cada mês</span><span class="sxs-lookup"><span data-stu-id="4645c-170">Repeat this event on the 15th of every month</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 1,
      "dayOfMonth": 15
    }
  ```
- <span data-ttu-id="4645c-171">Repita esse evento trimestralmente (a cada 3 meses) no dia 7</span><span class="sxs-lookup"><span data-stu-id="4645c-171">Repeat this event quarterly (every 3 months) on the 7th</span></span>

  ```json
    "pattern": {
      "type": "absoluteMonthly",
      "interval": 3,
      "dayOfMonth": 7
    }
  ```

### <a name="relative-monthly"></a><span data-ttu-id="4645c-172">Mensal relativo</span><span class="sxs-lookup"><span data-stu-id="4645c-172">Relative monthly</span></span>

<span data-ttu-id="4645c-173">O padrão mensal relativo faz com que um evento se repita no mesmo dia da semana na mesma posição relativa do mês, com base no número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="4645c-173">The relative monthly pattern causes an event to repeat on the same day of the week in the same relative position in the month, based on the number of months between each occurrence.</span></span> <span data-ttu-id="4645c-174">Por exemplo, "toda segunda quarta-feira do mês".</span><span class="sxs-lookup"><span data-stu-id="4645c-174">For example, "every second Wednesday of the month."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="4645c-175">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="4645c-175">Relevant properties</span></span>

| <span data-ttu-id="4645c-176">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4645c-176">Property</span></span> | <span data-ttu-id="4645c-177">Relevância</span><span class="sxs-lookup"><span data-stu-id="4645c-177">Relevance</span></span> | <span data-ttu-id="4645c-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="4645c-178">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="4645c-179">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="4645c-179">**daysOfWeek**</span></span> | <span data-ttu-id="4645c-180">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-180">Required</span></span> | <span data-ttu-id="4645c-181">Especifica em quais dias da semana o evento pode ocorrer.</span><span class="sxs-lookup"><span data-stu-id="4645c-181">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="4645c-182">Eventos mensais relativos apenas ocorrerem uma vez por mês, portanto, se mais de um valor for especificado, o evento ocorrerá no primeiro dia que satisfaz o padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-182">Relative monthly events only occur once per month, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="4645c-183">**índice**</span><span class="sxs-lookup"><span data-stu-id="4645c-183">**index**</span></span> | <span data-ttu-id="4645c-184">Opcional</span><span class="sxs-lookup"><span data-stu-id="4645c-184">Optional</span></span> | <span data-ttu-id="4645c-185">Especifica em qual instância dos dias permitidos especificados em **daysOfsWeek** o evento ocorre, contando a partir da primeira instância no mês.</span><span class="sxs-lookup"><span data-stu-id="4645c-185">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="4645c-186">Valores possíveis: `first`, `second`, `third`, `fourth` e `last`.</span><span class="sxs-lookup"><span data-stu-id="4645c-186">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="4645c-187">Valor padrão: `first`.</span><span class="sxs-lookup"><span data-stu-id="4645c-187">Default value: `first`.</span></span> |
| <span data-ttu-id="4645c-188">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="4645c-188">**interval**</span></span> | <span data-ttu-id="4645c-189">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-189">Required</span></span> | <span data-ttu-id="4645c-190">Especifica o número de meses entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="4645c-190">Specifies the number of months between each occurrence.</span></span> |
| <span data-ttu-id="4645c-191">**type**</span><span class="sxs-lookup"><span data-stu-id="4645c-191">**type**</span></span> | <span data-ttu-id="4645c-192">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-192">Required</span></span> | <span data-ttu-id="4645c-193">Tem que ser definida como `relativeMonthly`.</span><span class="sxs-lookup"><span data-stu-id="4645c-193">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="4645c-194">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4645c-194">Examples</span></span>

- <span data-ttu-id="4645c-195">Repita esse evento na segunda quarta-feira de cada mês</span><span class="sxs-lookup"><span data-stu-id="4645c-195">Repeat this event on the second Wednesday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "second"
    }
  ```
- <span data-ttu-id="4645c-196">Repita esse evento na primeira quinta ou sexta-feira de cada mês</span><span class="sxs-lookup"><span data-stu-id="4645c-196">Repeat this event on the first Thursday or Friday of every month</span></span>

  ```json
    "pattern": {
      "type": "relativeMonthly",
      "interval": 1,
      "daysOfWeek": [ "Thursday", "Friday" ],
      "index": "first"
    }
  ```

### <a name="absolute-yearly"></a><span data-ttu-id="4645c-197">Anual absoluto</span><span class="sxs-lookup"><span data-stu-id="4645c-197">Absolute yearly</span></span>

<span data-ttu-id="4645c-198">O padrão anual absoluto faz com que um evento se repita no mesmo mês e dia (por exemplo, dia 15 de abril), com base no número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="4645c-198">The absolute yearly pattern causes an event to repeat on the same month and day (for example, April 15), based on the number of years between each occurrence.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="4645c-199">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="4645c-199">Relevant properties</span></span>

| <span data-ttu-id="4645c-200">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4645c-200">Property</span></span> | <span data-ttu-id="4645c-201">Relevância</span><span class="sxs-lookup"><span data-stu-id="4645c-201">Relevance</span></span> | <span data-ttu-id="4645c-202">Descrição</span><span class="sxs-lookup"><span data-stu-id="4645c-202">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="4645c-203">**dayOfMonth**</span><span class="sxs-lookup"><span data-stu-id="4645c-203">**dayOfMonth**</span></span> | <span data-ttu-id="4645c-204">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-204">Required</span></span> | <span data-ttu-id="4645c-205">Especifica em quais dias do mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="4645c-205">Specifies on which day of the month the event occurs.</span></span> |
| <span data-ttu-id="4645c-206">**Mês**</span><span class="sxs-lookup"><span data-stu-id="4645c-206">**month**</span></span> | <span data-ttu-id="4645c-207">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-207">Required</span></span> | <span data-ttu-id="4645c-208">Especifica em qual mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="4645c-208">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="4645c-209">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="4645c-209">**interval**</span></span> | <span data-ttu-id="4645c-210">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-210">Required</span></span> | <span data-ttu-id="4645c-211">Especifica o número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="4645c-211">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="4645c-212">**type**</span><span class="sxs-lookup"><span data-stu-id="4645c-212">**type**</span></span> | <span data-ttu-id="4645c-213">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-213">Required</span></span> | <span data-ttu-id="4645c-214">Tem que ser definida como `absoluteYearly`.</span><span class="sxs-lookup"><span data-stu-id="4645c-214">Must be set to `absoluteYearly`.</span></span> |

#### <a name="example"></a><span data-ttu-id="4645c-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4645c-215">Example</span></span>

- <span data-ttu-id="4645c-216">Repita esse evento em 15 de abril todo ano</span><span class="sxs-lookup"><span data-stu-id="4645c-216">Repeat this event on April 15 every year</span></span>

  ```json
    "pattern": {
      "type": "absoluteYearly",
      "interval": 1,
      "dayOfMonth": 15,
      "month": 4
    }
  ```

### <a name="relative-yearly"></a><span data-ttu-id="4645c-217">Anual relativo</span><span class="sxs-lookup"><span data-stu-id="4645c-217">Relative yearly</span></span>

<span data-ttu-id="4645c-218">O padrão anual relativo faz com que um evento se repita no mesmo dia da semana na mesma posição relativa de um mês específico, com base no número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="4645c-218">The relative yearly pattern causes an event to repeat on the same day of the week in the same relative position in a specific month, based on the number of years between each occurrence.</span></span> <span data-ttu-id="4645c-219">Por exemplo, "toda última quarta-feira de novembro".</span><span class="sxs-lookup"><span data-stu-id="4645c-219">For example, "every last Wednesday of November."</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="4645c-220">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="4645c-220">Relevant properties</span></span>

| <span data-ttu-id="4645c-221">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4645c-221">Property</span></span> | <span data-ttu-id="4645c-222">Relevância</span><span class="sxs-lookup"><span data-stu-id="4645c-222">Relevance</span></span> | <span data-ttu-id="4645c-223">Descrição</span><span class="sxs-lookup"><span data-stu-id="4645c-223">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="4645c-224">**daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="4645c-224">**daysOfWeek**</span></span> | <span data-ttu-id="4645c-225">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-225">Required</span></span> | <span data-ttu-id="4645c-226">Especifica em quais dias da semana o evento pode ocorrer.</span><span class="sxs-lookup"><span data-stu-id="4645c-226">Specifies on which day(s) of the week the event can occur.</span></span> <span data-ttu-id="4645c-227">Eventos anuais relativos apenas ocorrerem uma vez por ano, portanto, se mais de um valor for especificado, o evento ocorrerá no primeiro dia que satisfaz o padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-227">Relative yearly events only occur once per year, so if more than one value is specified, the event falls on the first day that satisfies the pattern.</span></span> |
| <span data-ttu-id="4645c-228">**índice**</span><span class="sxs-lookup"><span data-stu-id="4645c-228">**index**</span></span> | <span data-ttu-id="4645c-229">Opcional</span><span class="sxs-lookup"><span data-stu-id="4645c-229">Optional</span></span> | <span data-ttu-id="4645c-230">Especifica em qual instância dos dias permitidos especificados em **daysOfsWeek** o evento ocorre, contando a partir da primeira instância no mês.</span><span class="sxs-lookup"><span data-stu-id="4645c-230">Specifies on which instance of the allowed days specified in **daysOfsWeek** the event occurs, counted from the first instance in the month.</span></span> <span data-ttu-id="4645c-231">Valores possíveis: `first`, `second`, `third`, `fourth` e `last`.</span><span class="sxs-lookup"><span data-stu-id="4645c-231">Possible values: `first`, `second`, `third`, `fourth`, and `last`.</span></span> <span data-ttu-id="4645c-232">Valor padrão: `first`.</span><span class="sxs-lookup"><span data-stu-id="4645c-232">Default value: `first`.</span></span> |
| <span data-ttu-id="4645c-233">**Mês**</span><span class="sxs-lookup"><span data-stu-id="4645c-233">**month**</span></span> | <span data-ttu-id="4645c-234">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-234">Required</span></span> | <span data-ttu-id="4645c-235">Especifica em qual mês o evento ocorre.</span><span class="sxs-lookup"><span data-stu-id="4645c-235">Specifies in which month the event occurs.</span></span> |
| <span data-ttu-id="4645c-236">**intervalo**</span><span class="sxs-lookup"><span data-stu-id="4645c-236">**interval**</span></span> | <span data-ttu-id="4645c-237">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-237">Required</span></span> | <span data-ttu-id="4645c-238">Especifica o número de anos entre cada ocorrência.</span><span class="sxs-lookup"><span data-stu-id="4645c-238">Specifies the number of years between each occurrence.</span></span> |
| <span data-ttu-id="4645c-239">**type**</span><span class="sxs-lookup"><span data-stu-id="4645c-239">**type**</span></span> | <span data-ttu-id="4645c-240">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-240">Required</span></span> | <span data-ttu-id="4645c-241">Tem que ser definida como `relativeMonthly`.</span><span class="sxs-lookup"><span data-stu-id="4645c-241">Must be set to `relativeMonthly`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="4645c-242">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4645c-242">Examples</span></span>

- <span data-ttu-id="4645c-243">Repita esse evento na última quarta-feira de novembro a cada ano</span><span class="sxs-lookup"><span data-stu-id="4645c-243">Repeat this event on the last Wednesday of November every year</span></span>

  ```json
    "pattern": {
      "type": "relativeYearly",
      "interval": 1,
      "daysOfWeek": [ "Wednesday" ],
      "index": "last",
      "month": 11
    }
  ```

## <a name="recurrence-ranges"></a><span data-ttu-id="4645c-244">Intervalos de recorrência</span><span class="sxs-lookup"><span data-stu-id="4645c-244">Recurrence ranges</span></span>

<span data-ttu-id="4645c-245">A segunda parte de uma recorrência é o intervalo.</span><span class="sxs-lookup"><span data-stu-id="4645c-245">The second part of a recurrence is the range.</span></span> <span data-ttu-id="4645c-246">Especifica por quanto tempo o padrão se repete.</span><span class="sxs-lookup"><span data-stu-id="4645c-246">This specifies how long the pattern repeats.</span></span> <span data-ttu-id="4645c-247">Por exemplo, um evento poderia terminar após 10 ocorrências, em uma data específica ou poderia não ter fim.</span><span class="sxs-lookup"><span data-stu-id="4645c-247">For example, an event could end after 10 occurrences, by a specific date, or could have no end.</span></span> <span data-ttu-id="4645c-248">Um intervalo é representado na API pelo [recurso recurrenceRange](../api-reference/v1.0/resources/recurrencepattern.md).</span><span class="sxs-lookup"><span data-stu-id="4645c-248">A range is represented in the API by the [recurrenceRange resource](../api-reference/v1.0/resources/recurrencepattern.md).</span></span>

<span data-ttu-id="4645c-249">Dependendo do tipo de intervalo, determinados campos do **recurrenceRange** são obrigatórios ou ignorados.</span><span class="sxs-lookup"><span data-stu-id="4645c-249">Depending on the type of range, certain fields of **recurrenceRange** are required or ignored.</span></span>

> <span data-ttu-id="4645c-250">**Observação**: Mesmo que um campo seja ignorado, ele ainda é validado.</span><span class="sxs-lookup"><span data-stu-id="4645c-250">**Note**: Even if a field is ignored, it is still validated.</span></span> <span data-ttu-id="4645c-251">Se um campo tiver um conjunto fixo de valores possíveis, usar um valor fora do conjunto permitido causa um erro, mesmo que esse campo seja ignorado.</span><span class="sxs-lookup"><span data-stu-id="4645c-251">If a field has a set list of possible values, using a value outside the allowed set causes an error, even if that field is ignored.</span></span>

<span data-ttu-id="4645c-252">Vamos dar uma olhada em cada um dos tipos de possíveis de intervalo.</span><span class="sxs-lookup"><span data-stu-id="4645c-252">Let's take a look at each of the possible range types.</span></span>

### <a name="numbered-range"></a><span data-ttu-id="4645c-253">Intervalo numerado</span><span class="sxs-lookup"><span data-stu-id="4645c-253">Numbered range</span></span>

<span data-ttu-id="4645c-254">O intervalo numerado faz com que um evento ocorra um número fixo de vezes (com base no padrão) de uma data de início.</span><span class="sxs-lookup"><span data-stu-id="4645c-254">The numbered range causes an event to occur a fixed number of times (based on the pattern) from a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="4645c-255">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="4645c-255">Relevant properties</span></span>

| <span data-ttu-id="4645c-256">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4645c-256">Property</span></span> | <span data-ttu-id="4645c-257">Relevância</span><span class="sxs-lookup"><span data-stu-id="4645c-257">Relevance</span></span> | <span data-ttu-id="4645c-258">Descrição</span><span class="sxs-lookup"><span data-stu-id="4645c-258">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="4645c-259">**numberOfOccurences**</span><span class="sxs-lookup"><span data-stu-id="4645c-259">**numberOfOccurences**</span></span> | <span data-ttu-id="4645c-260">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-260">Required</span></span> | <span data-ttu-id="4645c-261">Especifica o número de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="4645c-261">Specifies the number of occurrences.</span></span> <span data-ttu-id="4645c-262">Deve ser um número inteiro positivo.</span><span class="sxs-lookup"><span data-stu-id="4645c-262">Must be a positive integer.</span></span> |
| <span data-ttu-id="4645c-263">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="4645c-263">**recurrenceTimeZone**</span></span> | <span data-ttu-id="4645c-264">Opcional</span><span class="sxs-lookup"><span data-stu-id="4645c-264">Optional</span></span> | <span data-ttu-id="4645c-265">Especifica o fuso horário para a propriedade **startDate**.</span><span class="sxs-lookup"><span data-stu-id="4645c-265">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="4645c-266">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="4645c-266">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="4645c-267">**startDate**</span><span class="sxs-lookup"><span data-stu-id="4645c-267">**startDate**</span></span> | <span data-ttu-id="4645c-268">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-268">Required</span></span> | <span data-ttu-id="4645c-269">Especifica a data para começar a aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-269">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="4645c-270">O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="4645c-270">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="4645c-271">Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-271">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="4645c-272">**type**</span><span class="sxs-lookup"><span data-stu-id="4645c-272">**type**</span></span> | <span data-ttu-id="4645c-273">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-273">Required</span></span> | <span data-ttu-id="4645c-274">Tem que ser definida como `numbered`.</span><span class="sxs-lookup"><span data-stu-id="4645c-274">Must be set to `numbered`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="4645c-275">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4645c-275">Examples</span></span>

- <span data-ttu-id="4645c-276">Repita esse evento 10 vezes</span><span class="sxs-lookup"><span data-stu-id="4645c-276">Repeat this event 10 times</span></span>

  ```json
    "range": {
      "type": "numbered",
      "startDate": "2017-04-02",
      "numberOfOccurrences": 10
    }
  ```

### <a name="end-date-range"></a><span data-ttu-id="4645c-277">Intervalo de datas de término</span><span class="sxs-lookup"><span data-stu-id="4645c-277">End date range</span></span>

<span data-ttu-id="4645c-278">O intervalo de datas de término faz com que um evento ocorra em todos os dias que se encaixem no padrão aplicável entre uma data de início e uma data de término.</span><span class="sxs-lookup"><span data-stu-id="4645c-278">The end date range causes an event to occur on all days that fit the applicable pattern between a start date and an end date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="4645c-279">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="4645c-279">Relevant properties</span></span>

| <span data-ttu-id="4645c-280">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4645c-280">Property</span></span> | <span data-ttu-id="4645c-281">Relevância</span><span class="sxs-lookup"><span data-stu-id="4645c-281">Relevance</span></span> | <span data-ttu-id="4645c-282">Descrição</span><span class="sxs-lookup"><span data-stu-id="4645c-282">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="4645c-283">**endDate**</span><span class="sxs-lookup"><span data-stu-id="4645c-283">**endDate**</span></span> | <span data-ttu-id="4645c-284">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-284">Required</span></span> | <span data-ttu-id="4645c-285">Especifica a data para parar de aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-285">Specifies the date to stop applying the pattern.</span></span> <span data-ttu-id="4645c-286">Observação: Esta última ocorrência da reunião pode não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-286">Note that the last occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="4645c-287">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="4645c-287">**recurrenceTimeZone**</span></span> | <span data-ttu-id="4645c-288">Opcional</span><span class="sxs-lookup"><span data-stu-id="4645c-288">Optional</span></span> | <span data-ttu-id="4645c-289">Especifica o fuso horário das propriedades **startDate** e **endDate**.</span><span class="sxs-lookup"><span data-stu-id="4645c-289">Specifies the time zone for the **startDate** and **endDate** properties.</span></span> <span data-ttu-id="4645c-290">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="4645c-290">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="4645c-291">**startDate**</span><span class="sxs-lookup"><span data-stu-id="4645c-291">**startDate**</span></span> | <span data-ttu-id="4645c-292">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-292">Required</span></span> | <span data-ttu-id="4645c-293">Especifica a data para começar a aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-293">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="4645c-294">O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="4645c-294">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="4645c-295">Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-295">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="4645c-296">**type**</span><span class="sxs-lookup"><span data-stu-id="4645c-296">**type**</span></span> | <span data-ttu-id="4645c-297">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-297">Required</span></span> | <span data-ttu-id="4645c-298">Tem que ser definida como **endDate**.</span><span class="sxs-lookup"><span data-stu-id="4645c-298">Must be set to **endDate**.</span></span> |

#### <a name="examples"></a><span data-ttu-id="4645c-299">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4645c-299">Examples</span></span>

- <span data-ttu-id="4645c-300">Repita esse evento de 1.º de julho de 2017 a 31 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="4645c-300">Repeat this event from July 1, 2017, to July 31, 2017</span></span>

  ```json
    "range": {
      "type": "endDate",
      "startDate": "2017-07-01",
      "endDate": "2017-07-31"
    }
  ```

### <a name="no-end-range"></a><span data-ttu-id="4645c-301">Intervalo sem término</span><span class="sxs-lookup"><span data-stu-id="4645c-301">No end range</span></span>

<span data-ttu-id="4645c-302">O intervalo sem término faz com que um evento ocorra em todos os dias que se encaixem no padrão aplicável após uma data de início.</span><span class="sxs-lookup"><span data-stu-id="4645c-302">The no end range causes an event to occur on all days that fit the applicable pattern after a start date.</span></span>

#### <a name="relevant-properties"></a><span data-ttu-id="4645c-303">Propriedades relevantes</span><span class="sxs-lookup"><span data-stu-id="4645c-303">Relevant properties</span></span>

| <span data-ttu-id="4645c-304">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4645c-304">Property</span></span> | <span data-ttu-id="4645c-305">Relevância</span><span class="sxs-lookup"><span data-stu-id="4645c-305">Relevance</span></span> | <span data-ttu-id="4645c-306">Descrição</span><span class="sxs-lookup"><span data-stu-id="4645c-306">Description</span></span> |
|----------|-----------|-------------|
| <span data-ttu-id="4645c-307">**recurrenceTimeZone**</span><span class="sxs-lookup"><span data-stu-id="4645c-307">**recurrenceTimeZone**</span></span> | <span data-ttu-id="4645c-308">Opcional</span><span class="sxs-lookup"><span data-stu-id="4645c-308">Optional</span></span> | <span data-ttu-id="4645c-309">Especifica o fuso horário para a propriedade **startDate**.</span><span class="sxs-lookup"><span data-stu-id="4645c-309">Specifies the time zone for the **startDate** property.</span></span> <span data-ttu-id="4645c-310">Se a propriedade não for especificada, será usado o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="4645c-310">If not specified, the time zone of the event is used.</span></span> |
| <span data-ttu-id="4645c-311">**startDate**</span><span class="sxs-lookup"><span data-stu-id="4645c-311">**startDate**</span></span> | <span data-ttu-id="4645c-312">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-312">Required</span></span> | <span data-ttu-id="4645c-313">Especifica a data para começar a aplicar o padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-313">Specifies the date to start applying the pattern.</span></span> <span data-ttu-id="4645c-314">O valor de **startDate** DEVE corresponder ao valor da data da propriedade **iniciar** no [recurso de evento](../api-reference/v1.0/resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="4645c-314">The value of **startDate** MUST correspond to the date value of the **start** property on the [event resource](../api-reference/v1.0/resources/event.md).</span></span> <span data-ttu-id="4645c-315">Observação: Esta primeira ocorrência da reunião poderá não ocorrer nessa data se ela não se encaixar no padrão.</span><span class="sxs-lookup"><span data-stu-id="4645c-315">Note that the first occurrence of the meeting may not occur on this date if it does not fit the pattern.</span></span> |
| <span data-ttu-id="4645c-316">**type**</span><span class="sxs-lookup"><span data-stu-id="4645c-316">**type**</span></span> | <span data-ttu-id="4645c-317">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="4645c-317">Required</span></span> | <span data-ttu-id="4645c-318">Tem que ser definida como `noEnd`.</span><span class="sxs-lookup"><span data-stu-id="4645c-318">Must be set to `noEnd`.</span></span> |

#### <a name="examples"></a><span data-ttu-id="4645c-319">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4645c-319">Examples</span></span>

- <span data-ttu-id="4645c-320">Repita esse evento de 15 de maio de 2017 para sempre</span><span class="sxs-lookup"><span data-stu-id="4645c-320">Repeat this event from May 15, 2017, forever</span></span>

  ```json
    "range": {
      "type": "noEnd",
      "startDate": "2017-05-15"
    }
  ```

## <a name="using-patterns-and-ranges-to-create-recurring-events"></a><span data-ttu-id="4645c-321">Usando padrões e intervalos para criar eventos recorrentes</span><span class="sxs-lookup"><span data-stu-id="4645c-321">Using patterns and ranges to create recurring events</span></span>

<span data-ttu-id="4645c-322">Agora que já vimos padrões e intervalos separadamente, vamos analisar como eles funcionam juntos e como eles interagem com as propriedades **iniciar** e **encerrar** do evento.</span><span class="sxs-lookup"><span data-stu-id="4645c-322">Now that we've looked at patterns and ranges separately, let's look at how they work together and how they interact with the **start** and **end** properties on the event.</span></span>

### <a name="creating-a-recurrence-rule"></a><span data-ttu-id="4645c-323">Criando uma regra de recorrência</span><span class="sxs-lookup"><span data-stu-id="4645c-323">Creating a recurrence rule</span></span>

<span data-ttu-id="4645c-324">Para criar uma regra de recorrência, você deve especificar um padrão e um intervalo.</span><span class="sxs-lookup"><span data-stu-id="4645c-324">To create a recurrence rule, you must specify both a pattern and a range.</span></span> <span data-ttu-id="4645c-325">Qualquer tipo de padrão pode funcionar com qualquer tipo de intervalo.</span><span class="sxs-lookup"><span data-stu-id="4645c-325">Any pattern type can work with any range type.</span></span> <span data-ttu-id="4645c-326">Eis alguns exemplos.</span><span class="sxs-lookup"><span data-stu-id="4645c-326">Here are a few examples.</span></span>

#### <a name="examples"></a><span data-ttu-id="4645c-327">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4645c-327">Examples</span></span>

- <span data-ttu-id="4645c-328">**Reunião das 13h às 13h30 toda segunda-feira a partir de 4 de setembro de 2017 até o final do ano**</span><span class="sxs-lookup"><span data-stu-id="4645c-328">**Meet from 1:00 PM to 1:30 PM every Monday starting September 4, 2017, until the end of the year**</span></span>

  - <span data-ttu-id="4645c-329">O requisito "toda segunda-feira" requisito é atendido facilmente pelo tipo de padrão de recorrência `weekly`.</span><span class="sxs-lookup"><span data-stu-id="4645c-329">The "every Monday" requirement is easily met by the `weekly` recurrence pattern type.</span></span>
  - <span data-ttu-id="4645c-330">O requisito "até o final do ano" indica um tipo de intervalo de recorrência `endDate`.</span><span class="sxs-lookup"><span data-stu-id="4645c-330">The "until the end of the year" requirement indicates an `endDate` recurrence range type.</span></span>

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

  <span data-ttu-id="4645c-331">Como 31 de dezembro de 2017 é um domingo, a última ocorrência dessa série será na segunda-feira, dia 25 de dezembro.</span><span class="sxs-lookup"><span data-stu-id="4645c-331">Because December 31, 2017, is on a Sunday, the last occurrence in this series will be on Monday, December 25.</span></span>

- <span data-ttu-id="4645c-332">**Reunião das 14h às 15h na primeira quinta-feira de cada mês a partir de 29 de agosto de 2017**</span><span class="sxs-lookup"><span data-stu-id="4645c-332">**Meet from 2:00 PM to 3:00 PM on the first Thursday of every other month starting August 29, 2017**</span></span>

  - <span data-ttu-id="4645c-333">O requisito "primeira quinta-feira de cada mês" pode ser cumprido usando um padrão mensal relativo.</span><span class="sxs-lookup"><span data-stu-id="4645c-333">The "first Thursday of every other month" requirement is achievable by using a relative monthly pattern.</span></span> <span data-ttu-id="4645c-334">A parte "cada mês" indica que o **intervalo** deve ser definido como `2`.</span><span class="sxs-lookup"><span data-stu-id="4645c-334">The "every other month" portion indicates that the **interval** should be set to `2`.</span></span>
  - <span data-ttu-id="4645c-335">Por não existir um requisito de data de término, um tipo de intervalo `noEnd` pode ser usado.</span><span class="sxs-lookup"><span data-stu-id="4645c-335">Because there is no requirement on an end date, a `noEnd` range type can be used.</span></span>

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

  <span data-ttu-id="4645c-336">Como o valor de **starDate** é após a primeira quinta-feira de agosto, a primeira ocorrência dessa série será em setembro.</span><span class="sxs-lookup"><span data-stu-id="4645c-336">Because the value of **startDate** is after the first Thursday in August, the first occurrence of this series will be in September.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4645c-337">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="4645c-337">Next steps</span></span>
    
<span data-ttu-id="4645c-338">Veja mais detalhes em [integração com o calendário do Outlook](outlook-calendar-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="4645c-338">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
