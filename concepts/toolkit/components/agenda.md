---
title: Componente agenda no microsoft Graph Toolkit
description: O componente web mgt-agenda é usado para representar eventos em um calendário de usuário ou grupo.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 7de172c514aea12e0f57541649b6e98ca1ded2df
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781097"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="c53ca-103">Componente agenda no microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="c53ca-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="c53ca-104">O `mgt-agenda` componente Web representa eventos em um calendário de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="c53ca-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="c53ca-105">Por padrão, o calendário exibe os eventos de usuário atuais assinados no dia atual.</span><span class="sxs-lookup"><span data-stu-id="c53ca-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="c53ca-106">O componente também pode usar qualquer ponto de extremidade que retorne eventos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c53ca-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="c53ca-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c53ca-107">Example</span></span>

<span data-ttu-id="c53ca-108">O exemplo a seguir mostra os eventos de calendário do usuário assinado exibidos usando o `mgt-agenda` componente.</span><span class="sxs-lookup"><span data-stu-id="c53ca-108">The following example shows the signed-in user's calendar events displayed using the `mgt-agenda` component.</span></span> <span data-ttu-id="c53ca-109">Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="c53ca-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[<span data-ttu-id="c53ca-110">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="c53ca-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a><span data-ttu-id="c53ca-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c53ca-111">Properties</span></span>

<span data-ttu-id="c53ca-112">Por padrão, o componente busca eventos do ponto de extremidade e `mgt-agenda` exibe eventos para o dia `/me/calendarview` atual.</span><span class="sxs-lookup"><span data-stu-id="c53ca-112">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="c53ca-113">Há várias propriedades que você pode usar para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="c53ca-113">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="c53ca-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="c53ca-114">Attribute</span></span> | <span data-ttu-id="c53ca-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c53ca-115">Property</span></span> | <span data-ttu-id="c53ca-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53ca-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="c53ca-117">data</span><span class="sxs-lookup"><span data-stu-id="c53ca-117">date</span></span> | <span data-ttu-id="c53ca-118">data</span><span class="sxs-lookup"><span data-stu-id="c53ca-118">date</span></span> | <span data-ttu-id="c53ca-119">Uma cadeia de caracteres que representa a data de início dos eventos a buscar da Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c53ca-119">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="c53ca-120">O valor deve estar em um formato que pode ser analisado pelo construtor [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - o valor não terá efeito se `event-query` o atributo for definido.</span><span class="sxs-lookup"><span data-stu-id="c53ca-120">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="c53ca-121">days</span><span class="sxs-lookup"><span data-stu-id="c53ca-121">days</span></span> | <span data-ttu-id="c53ca-122">days</span><span class="sxs-lookup"><span data-stu-id="c53ca-122">days</span></span> | <span data-ttu-id="c53ca-123">Um número de dias para buscar do Microsoft Graph - o padrão é 3 - o valor não terá efeito se `event-query` o atributo for definido.</span><span class="sxs-lookup"><span data-stu-id="c53ca-123">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="c53ca-124">show-max</span><span class="sxs-lookup"><span data-stu-id="c53ca-124">show-max</span></span> | <span data-ttu-id="c53ca-125">showMax</span><span class="sxs-lookup"><span data-stu-id="c53ca-125">showMax</span></span> | <span data-ttu-id="c53ca-126">Um número para indicar o número máximo de eventos a mostrar.</span><span class="sxs-lookup"><span data-stu-id="c53ca-126">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="c53ca-127">O valor padrão não está definido (nenhum máximo).</span><span class="sxs-lookup"><span data-stu-id="c53ca-127">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="c53ca-128">group-id</span><span class="sxs-lookup"><span data-stu-id="c53ca-128">group-id</span></span> | <span data-ttu-id="c53ca-129">groupId</span><span class="sxs-lookup"><span data-stu-id="c53ca-129">groupId</span></span> | <span data-ttu-id="c53ca-130">Uma ID de cadeia de caracteres para um calendário de grupo a ser usado em vez do calendário atual do usuário.</span><span class="sxs-lookup"><span data-stu-id="c53ca-130">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="c53ca-131">event-query</span><span class="sxs-lookup"><span data-stu-id="c53ca-131">event-query</span></span> | <span data-ttu-id="c53ca-132">eventQuery</span><span class="sxs-lookup"><span data-stu-id="c53ca-132">eventQuery</span></span> | <span data-ttu-id="c53ca-133">Uma cadeia de caracteres que representa uma consulta alternativa a ser usada ao buscar eventos da Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c53ca-133">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="c53ca-134">Opcionalmente, adicione o escopo delegado no final da cadeia de caracteres delimitando-o com `|` ( `/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all` ).</span><span class="sxs-lookup"><span data-stu-id="c53ca-134">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="c53ca-135">events</span><span class="sxs-lookup"><span data-stu-id="c53ca-135">events</span></span> | <span data-ttu-id="c53ca-136">events</span><span class="sxs-lookup"><span data-stu-id="c53ca-136">events</span></span> | <span data-ttu-id="c53ca-137">Uma matriz de eventos para obter ou definir a lista de eventos renderizados pelo componente - use essa propriedade para acessar os eventos carregados pelo componente.</span><span class="sxs-lookup"><span data-stu-id="c53ca-137">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="c53ca-138">De definir esse valor para carregar seus próprios eventos - se o valor for definido pelo desenvolvedor, `date` os atributos , ou não terão `days` `event-query` efeito.</span><span class="sxs-lookup"><span data-stu-id="c53ca-138">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="c53ca-139">group-by-day</span><span class="sxs-lookup"><span data-stu-id="c53ca-139">group-by-day</span></span> | <span data-ttu-id="c53ca-140">groupByDay</span><span class="sxs-lookup"><span data-stu-id="c53ca-140">groupByDay</span></span> | <span data-ttu-id="c53ca-141">Um valor Boolean para agrupar eventos por dia - por padrão, os eventos não são agrupados.</span><span class="sxs-lookup"><span data-stu-id="c53ca-141">A Boolean value to group events by day - by default events are not grouped.</span></span> |
| <span data-ttu-id="c53ca-142">preferred-timezone</span><span class="sxs-lookup"><span data-stu-id="c53ca-142">preferred-timezone</span></span> | <span data-ttu-id="c53ca-143">preferredTimezone</span><span class="sxs-lookup"><span data-stu-id="c53ca-143">preferredTimezone</span></span> | <span data-ttu-id="c53ca-144">Nome do fuso horário preferencial a ser usado ao recuperar eventos do Microsoft Graph; por exemplo, `Pacific Standard Time` .</span><span class="sxs-lookup"><span data-stu-id="c53ca-144">Name of the preferred time zone to use when retrieving events from Microsoft Graph; for example, `Pacific Standard Time`.</span></span> <span data-ttu-id="c53ca-145">Por padrão, esse atributo usa o fuso horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c53ca-145">By default, this attribute uses the UTC time zone.</span></span> <span data-ttu-id="c53ca-146">O fuso horário preferencial para o usuário atual pode ser recuperado chamando o ponto de extremidade e lendo o `me/mailboxSettings` valor da **propriedade timeZone.**</span><span class="sxs-lookup"><span data-stu-id="c53ca-146">The preferred time zone for the current user can be retrieved by calling the `me/mailboxSettings` endpoint and reading the value of the **timeZone** property.</span></span> |

<span data-ttu-id="c53ca-147">O exemplo a seguir altera o comportamento do componente para buscar dados para uma data específica e até três dias.</span><span class="sxs-lookup"><span data-stu-id="c53ca-147">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="c53ca-148">O exemplo a seguir altera o comportamento do componente para buscar dados de uma consulta específica.</span><span class="sxs-lookup"><span data-stu-id="c53ca-148">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="methods"></a><span data-ttu-id="c53ca-149">Métodos</span><span class="sxs-lookup"><span data-stu-id="c53ca-149">Methods</span></span>
| <span data-ttu-id="c53ca-150">Método</span><span class="sxs-lookup"><span data-stu-id="c53ca-150">Method</span></span> | <span data-ttu-id="c53ca-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53ca-151">Description</span></span> |
| --- | --- |
| <span data-ttu-id="c53ca-152">reload()</span><span class="sxs-lookup"><span data-stu-id="c53ca-152">reload()</span></span> | <span data-ttu-id="c53ca-153">Chame o método para recarregar o componente com novos dados potenciais com base em suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c53ca-153">Call the method to reload the component with potential new data based on its properties.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="c53ca-154">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="c53ca-154">CSS custom properties</span></span>

<span data-ttu-id="c53ca-155">O `mgt-agenda` componente define essas propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="c53ca-155">The `mgt-agenda` component defines these CSS custom properties</span></span>

```css
mgt-agenda {
  --event-box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.092);
  --event-margin: 0px 10px 14px 10px;
  --event-padding: 8px 0px;
  --event-background-color: #ffffff;
  --event-border: solid 2px rgba(0, 0, 0, 0);

  --agenda-header-margin: 40px 10px 14px 10px;
  --agenda-header-font-size: 24px;
  --agenda-header-color: #333333;

  --event-time-font-size: 12px;
  --event-time-color: #000000;

  --event-subject-font-size: 19px;
  --event-subject-color: #333333;

  --event-location-font-size: 12px;
  --event-location-color: #000000;
}
```

<span data-ttu-id="c53ca-156">Para saber mais, confira [componentes de estilo](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="c53ca-156">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="c53ca-157">Modelos</span><span class="sxs-lookup"><span data-stu-id="c53ca-157">Templates</span></span>

<span data-ttu-id="c53ca-158">O `mgt-agenda` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="c53ca-158">The `mgt-agenda` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="c53ca-159">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes:</span><span class="sxs-lookup"><span data-stu-id="c53ca-159">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="c53ca-160">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="c53ca-160">Data type</span></span> | <span data-ttu-id="c53ca-161">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="c53ca-161">Data context</span></span> | <span data-ttu-id="c53ca-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53ca-162">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="c53ca-163">`events`: lista de objetos de evento</span><span class="sxs-lookup"><span data-stu-id="c53ca-163">`events`: list of event objects</span></span> | <span data-ttu-id="c53ca-164">O modelo padrão substitui todo o componente por seu próprio.</span><span class="sxs-lookup"><span data-stu-id="c53ca-164">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="c53ca-165">`event`: objeto event</span><span class="sxs-lookup"><span data-stu-id="c53ca-165">`event`: event object</span></span> | <span data-ttu-id="c53ca-166">O modelo usado para renderizar cada evento.</span><span class="sxs-lookup"><span data-stu-id="c53ca-166">The template used to render each event.</span></span> |
| `event-other` | <span data-ttu-id="c53ca-167">`event`: objeto event</span><span class="sxs-lookup"><span data-stu-id="c53ca-167">`event`: event object</span></span> | <span data-ttu-id="c53ca-168">O modelo usado para renderizar conteúdo adicional para cada evento.</span><span class="sxs-lookup"><span data-stu-id="c53ca-168">The template used to render additional content for each event.</span></span> |
| `header` | <span data-ttu-id="c53ca-169">`header`: string</span><span class="sxs-lookup"><span data-stu-id="c53ca-169">`header`: string</span></span> | <span data-ttu-id="c53ca-170">O modelo usado para renderizar o header para cada dia.</span><span class="sxs-lookup"><span data-stu-id="c53ca-170">The template used to render the header for each day.</span></span> |
| `loading` | <span data-ttu-id="c53ca-171">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="c53ca-171">No data context is passed</span></span> | <span data-ttu-id="c53ca-172">O modelo usado quando os dados estão sendo carregados.</span><span class="sxs-lookup"><span data-stu-id="c53ca-172">The template used when data is loading.</span></span> |
| `no-data` | <span data-ttu-id="c53ca-173">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="c53ca-173">No data context is passed</span></span> | <span data-ttu-id="c53ca-174">O modelo usado quando nenhum evento está disponível.</span><span class="sxs-lookup"><span data-stu-id="c53ca-174">The template used when no events are available.</span></span> |

<span data-ttu-id="c53ca-175">Os exemplos a seguir ilustram como usar o `event` modelo:</span><span class="sxs-lookup"><span data-stu-id="c53ca-175">The following examples illustrates how to use the `event` template:</span></span>

```html
<mgt-agenda>
  <template data-type="event">
    <button class="eventButton">
      <div class="event-subject">{{ event.subject }}</div>
      <div data-for="attendee in event.attendees">
        <mgt-person
          person-query="{{ attendee.emailAddress.name }}"
          view="twolines">
        </mgt-person>
      </div>
    </button>
  </template>
  <template data-type="no-data">
    There are no events found!
  </template>
</mgt-agenda>
```

<span data-ttu-id="c53ca-176">Para saber mais, confira [modelos](../customize-components/templates.md).</span><span class="sxs-lookup"><span data-stu-id="c53ca-176">To learn more, see [templates](../customize-components/templates.md).</span></span>

## <a name="events"></a><span data-ttu-id="c53ca-177">Eventos</span><span class="sxs-lookup"><span data-stu-id="c53ca-177">Events</span></span>

<span data-ttu-id="c53ca-178">Os eventos a seguir são disparados do controle.</span><span class="sxs-lookup"><span data-stu-id="c53ca-178">The following events are fired from the control.</span></span>

| <span data-ttu-id="c53ca-179">Evento</span><span class="sxs-lookup"><span data-stu-id="c53ca-179">Event</span></span> | <span data-ttu-id="c53ca-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53ca-180">Description</span></span> |
| --- | --- |
| <span data-ttu-id="c53ca-181">eventClick</span><span class="sxs-lookup"><span data-stu-id="c53ca-181">eventClick</span></span> | <span data-ttu-id="c53ca-182">O usuário clica ou toca em um evento.</span><span class="sxs-lookup"><span data-stu-id="c53ca-182">The user clicks or taps an event.</span></span>|

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="c53ca-183">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c53ca-183">Microsoft Graph permissions</span></span>

<span data-ttu-id="c53ca-184">Este componente usa as seguintes APIs Graph Microsoft e permissões:</span><span class="sxs-lookup"><span data-stu-id="c53ca-184">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="c53ca-185">Configuração</span><span class="sxs-lookup"><span data-stu-id="c53ca-185">Configuration</span></span> | <span data-ttu-id="c53ca-186">Permissão</span><span class="sxs-lookup"><span data-stu-id="c53ca-186">Permission</span></span> | <span data-ttu-id="c53ca-187">API</span><span class="sxs-lookup"><span data-stu-id="c53ca-187">API</span></span>
| - | - | - |
| <span data-ttu-id="c53ca-188">Padrão.</span><span class="sxs-lookup"><span data-stu-id="c53ca-188">default</span></span> | <span data-ttu-id="c53ca-189">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c53ca-189">Calendars.Read</span></span> | [<span data-ttu-id="c53ca-190">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="c53ca-190">/me/calendarview</span></span>](/graph/api/calendar-list-calendarview) |

<span data-ttu-id="c53ca-191">O componente permite que você especifique uma consulta Graph microsoft diferente para chamar (como `/groups/{id}/calendar/calendarView` ).</span><span class="sxs-lookup"><span data-stu-id="c53ca-191">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="c53ca-192">Nesse caso, anexar a permissão ao final da cadeia de caracteres, delimitada por `|` .</span><span class="sxs-lookup"><span data-stu-id="c53ca-192">In this case, append the permission to the end of the string, delimited by `|`.</span></span>

<span data-ttu-id="c53ca-193">Ao usar o modelo padrão e o modelo padrão, APIs e permissões adicionais `renderAttendees` são necessárias.</span><span class="sxs-lookup"><span data-stu-id="c53ca-193">When using the default template and default `renderAttendees` template, additional APIs and permissions are required.</span></span> <span data-ttu-id="c53ca-194">O modelo padrão para esse componente usa um [componente mgt-people](people.md) para eventos que têm participantes e herda todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="c53ca-194">The default template for this component uses a [mgt-people](people.md) component for events that have attendees, and inherits all permissions.</span></span>

## <a name="authentication"></a><span data-ttu-id="c53ca-195">Autenticação</span><span class="sxs-lookup"><span data-stu-id="c53ca-195">Authentication</span></span>

<span data-ttu-id="c53ca-196">O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="c53ca-196">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="c53ca-197">Cache</span><span class="sxs-lookup"><span data-stu-id="c53ca-197">Cache</span></span>

<span data-ttu-id="c53ca-198">O `mgt-agenda` componente não armazena dados em cache.</span><span class="sxs-lookup"><span data-stu-id="c53ca-198">The `mgt-agenda` component doesn't cache any data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="c53ca-199">Estender para obter mais controle</span><span class="sxs-lookup"><span data-stu-id="c53ca-199">Extend for more control</span></span>

<span data-ttu-id="c53ca-200">Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos render\* para substituição `protected` em extensões de componentes.</span><span class="sxs-lookup"><span data-stu-id="c53ca-200">For more complex scenarios or a truly custom UX, this component exposes several `protected` render\* methods for override in component extensions.</span></span>

| <span data-ttu-id="c53ca-201">Método</span><span class="sxs-lookup"><span data-stu-id="c53ca-201">Method</span></span> | <span data-ttu-id="c53ca-202">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53ca-202">Description</span></span> |
| - | - |
| <span data-ttu-id="c53ca-203">renderLoading</span><span class="sxs-lookup"><span data-stu-id="c53ca-203">renderLoading</span></span> | <span data-ttu-id="c53ca-204">Renderiza um estado de carregamento enquanto o componente é carregado.</span><span class="sxs-lookup"><span data-stu-id="c53ca-204">Renders a loading state while the component loads.</span></span> |
| <span data-ttu-id="c53ca-205">renderNoData</span><span class="sxs-lookup"><span data-stu-id="c53ca-205">renderNoData</span></span> | <span data-ttu-id="c53ca-206">Renderiza um estado de dados vazio.</span><span class="sxs-lookup"><span data-stu-id="c53ca-206">Renders an empty data state.</span></span> |
| <span data-ttu-id="c53ca-207">renderGroups</span><span class="sxs-lookup"><span data-stu-id="c53ca-207">renderGroups</span></span> | <span data-ttu-id="c53ca-208">Classifica os dados de eventos em grupos e os renderiza com os headers de grupo.</span><span class="sxs-lookup"><span data-stu-id="c53ca-208">Sorts event data into groups and renders them with group headers.</span></span> |
| <span data-ttu-id="c53ca-209">renderHeader</span><span class="sxs-lookup"><span data-stu-id="c53ca-209">renderHeader</span></span> | <span data-ttu-id="c53ca-210">Renderiza um header de grupo.</span><span class="sxs-lookup"><span data-stu-id="c53ca-210">Renders a group header.</span></span> |
| <span data-ttu-id="c53ca-211">renderEvents</span><span class="sxs-lookup"><span data-stu-id="c53ca-211">renderEvents</span></span> | <span data-ttu-id="c53ca-212">Renderiza uma lista de objetos de evento.</span><span class="sxs-lookup"><span data-stu-id="c53ca-212">Renders a list of event objects.</span></span> |
| <span data-ttu-id="c53ca-213">renderEvent</span><span class="sxs-lookup"><span data-stu-id="c53ca-213">renderEvent</span></span> | <span data-ttu-id="c53ca-214">Renderiza um evento singular e todas as suas partes.</span><span class="sxs-lookup"><span data-stu-id="c53ca-214">Renders a singular event and all of its parts.</span></span>
| <span data-ttu-id="c53ca-215">renderTitle</span><span class="sxs-lookup"><span data-stu-id="c53ca-215">renderTitle</span></span> | <span data-ttu-id="c53ca-216">Renderiza a parte do título do evento.</span><span class="sxs-lookup"><span data-stu-id="c53ca-216">Renders the event title part.</span></span> |
| <span data-ttu-id="c53ca-217">renderLocation</span><span class="sxs-lookup"><span data-stu-id="c53ca-217">renderLocation</span></span> | <span data-ttu-id="c53ca-218">Renderiza a parte do local do evento.</span><span class="sxs-lookup"><span data-stu-id="c53ca-218">Renders the event location part.</span></span> |
| <span data-ttu-id="c53ca-219">renderAttendees</span><span class="sxs-lookup"><span data-stu-id="c53ca-219">renderAttendees</span></span> | <span data-ttu-id="c53ca-220">Renderiza a parte dos participantes do evento.</span><span class="sxs-lookup"><span data-stu-id="c53ca-220">Renders the event attendees part.</span></span> |
| <span data-ttu-id="c53ca-221">renderOther</span><span class="sxs-lookup"><span data-stu-id="c53ca-221">renderOther</span></span> | <span data-ttu-id="c53ca-222">Renderiza conteúdo de evento adicional.</span><span class="sxs-lookup"><span data-stu-id="c53ca-222">Renders additional event content.</span></span> |
