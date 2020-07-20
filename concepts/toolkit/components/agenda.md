---
title: Componente de agenda no kit de ferramentas do Microsoft Graph
description: O componente de gerenciamento de agenda da Web é usado para representar eventos em um calendário de usuário ou grupo.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c42b62241f5eee7fef51bf57bf8617dd6e89b8c6
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183922"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="ecc96-103">Componente de agenda no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ecc96-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ecc96-104">O `mgt-agenda` componente da Web representa eventos em um calendário de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="ecc96-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="ecc96-105">Por padrão, o calendário exibe o atual eventos de usuário conectado para o dia atual.</span><span class="sxs-lookup"><span data-stu-id="ecc96-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="ecc96-106">O componente também pode usar qualquer ponto de extremidade que retorne eventos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ecc96-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="ecc96-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecc96-107">Example</span></span>

<span data-ttu-id="ecc96-108">O exemplo a seguir mostra os eventos de calendário do usuário conectado exibidos usando o `mgt-agenda` componente.</span><span class="sxs-lookup"><span data-stu-id="ecc96-108">The following example shows the signed-in user's calendar events displayed using the `mgt-agenda` component.</span></span> <span data-ttu-id="ecc96-109">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="ecc96-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[<span data-ttu-id="ecc96-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="ecc96-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a><span data-ttu-id="ecc96-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ecc96-111">Properties</span></span>

<span data-ttu-id="ecc96-112">Por padrão, o `mgt-agenda` componente busca eventos do ponto de `/me/calendarview` extremidade e exibe eventos para o dia atual.</span><span class="sxs-lookup"><span data-stu-id="ecc96-112">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="ecc96-113">Há várias propriedades que você pode usar para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="ecc96-113">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="ecc96-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="ecc96-114">Attribute</span></span> | <span data-ttu-id="ecc96-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecc96-115">Property</span></span> | <span data-ttu-id="ecc96-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecc96-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="ecc96-117">data</span><span class="sxs-lookup"><span data-stu-id="ecc96-117">date</span></span> | <span data-ttu-id="ecc96-118">data</span><span class="sxs-lookup"><span data-stu-id="ecc96-118">date</span></span> | <span data-ttu-id="ecc96-119">Uma cadeia de caracteres que representa a data de início dos eventos a serem buscados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ecc96-119">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="ecc96-120">O valor deve estar em um formato que pode ser analisado pelo [Construtor de data](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) -o valor não tem efeito se o `event-query` atributo for definido.</span><span class="sxs-lookup"><span data-stu-id="ecc96-120">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="ecc96-121">durante</span><span class="sxs-lookup"><span data-stu-id="ecc96-121">days</span></span> | <span data-ttu-id="ecc96-122">durante</span><span class="sxs-lookup"><span data-stu-id="ecc96-122">days</span></span> | <span data-ttu-id="ecc96-123">Um número de dias para buscar do Microsoft Graph-padrão é de 3 valores não tem efeito se o `event-query` atributo for definido.</span><span class="sxs-lookup"><span data-stu-id="ecc96-123">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="ecc96-124">show-Max</span><span class="sxs-lookup"><span data-stu-id="ecc96-124">show-max</span></span> | <span data-ttu-id="ecc96-125">showMax</span><span class="sxs-lookup"><span data-stu-id="ecc96-125">showMax</span></span> | <span data-ttu-id="ecc96-126">Um número para indicar o número máximo de eventos a serem exibidos.</span><span class="sxs-lookup"><span data-stu-id="ecc96-126">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="ecc96-127">O valor padrão não é definido (sem máximo).</span><span class="sxs-lookup"><span data-stu-id="ecc96-127">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="ecc96-128">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="ecc96-128">group-id</span></span> | <span data-ttu-id="ecc96-129">groupId</span><span class="sxs-lookup"><span data-stu-id="ecc96-129">groupId</span></span> | <span data-ttu-id="ecc96-130">Uma ID de cadeia de caracteres para um calendário de grupo a ser usado em vez do calendário do usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="ecc96-130">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="ecc96-131">evento-consulta</span><span class="sxs-lookup"><span data-stu-id="ecc96-131">event-query</span></span> | <span data-ttu-id="ecc96-132">eventQuery</span><span class="sxs-lookup"><span data-stu-id="ecc96-132">eventQuery</span></span> | <span data-ttu-id="ecc96-133">Uma cadeia de caracteres que representa uma consulta alternativa a ser usada ao buscar eventos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ecc96-133">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="ecc96-134">Opcionalmente, adicione o escopo delegado no final da cadeia de caracteres, delimitadondo-o com `|` ( `/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all` ).</span><span class="sxs-lookup"><span data-stu-id="ecc96-134">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="ecc96-135">eventos</span><span class="sxs-lookup"><span data-stu-id="ecc96-135">events</span></span> | <span data-ttu-id="ecc96-136">eventos</span><span class="sxs-lookup"><span data-stu-id="ecc96-136">events</span></span> | <span data-ttu-id="ecc96-137">Uma matriz de eventos para obter ou definir a lista de eventos renderizados pelo componente-Use essa propriedade para acessar os eventos carregados pelo componente.</span><span class="sxs-lookup"><span data-stu-id="ecc96-137">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="ecc96-138">Defina esse valor para carregar seus próprios eventos, se o valor for definido por desenvolvedor, `date` os `days` atributos, ou `event-query` não terão efeito.</span><span class="sxs-lookup"><span data-stu-id="ecc96-138">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="ecc96-139">grupo por dia</span><span class="sxs-lookup"><span data-stu-id="ecc96-139">group-by-day</span></span> | <span data-ttu-id="ecc96-140">groupByDay</span><span class="sxs-lookup"><span data-stu-id="ecc96-140">groupByDay</span></span> | <span data-ttu-id="ecc96-141">Um valor Boolean para agrupar eventos por dia-por eventos padrão não são agrupados.</span><span class="sxs-lookup"><span data-stu-id="ecc96-141">A Boolean value to group events by day - by default events are not grouped.</span></span> |

<span data-ttu-id="ecc96-142">O exemplo a seguir altera o comportamento do componente para buscar dados de uma data específica e até três dias.</span><span class="sxs-lookup"><span data-stu-id="ecc96-142">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="ecc96-143">O exemplo a seguir altera o comportamento do componente para buscar dados de uma consulta específica.</span><span class="sxs-lookup"><span data-stu-id="ecc96-143">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a><span data-ttu-id="ecc96-144">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="ecc96-144">CSS custom properties</span></span>

<span data-ttu-id="ecc96-145">O `mgt-agenda` componente define essas propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="ecc96-145">The `mgt-agenda` component defines these CSS custom properties</span></span>

```css
mgt-agenda {
  --event-box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.092);
  --event-margin: 0px 10px 14px 10px;
  --event-padding: 8px 0px;
  --event-background: #ffffff;
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

<span data-ttu-id="ecc96-146">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="ecc96-146">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="ecc96-147">Modelos</span><span class="sxs-lookup"><span data-stu-id="ecc96-147">Templates</span></span>

<span data-ttu-id="ecc96-148">O `mgt-agenda` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="ecc96-148">The `mgt-agenda` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="ecc96-149">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="ecc96-149">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="ecc96-150">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="ecc96-150">Data type</span></span> | <span data-ttu-id="ecc96-151">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="ecc96-151">Data context</span></span> | <span data-ttu-id="ecc96-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecc96-152">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="ecc96-153">`events`: lista de objetos Event</span><span class="sxs-lookup"><span data-stu-id="ecc96-153">`events`: list of event objects</span></span> | <span data-ttu-id="ecc96-154">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="ecc96-154">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="ecc96-155">`event`: objeto Event</span><span class="sxs-lookup"><span data-stu-id="ecc96-155">`event`: event object</span></span> | <span data-ttu-id="ecc96-156">O modelo usado para renderizar cada evento.</span><span class="sxs-lookup"><span data-stu-id="ecc96-156">The template used to render each event.</span></span> |
| `event-other` | <span data-ttu-id="ecc96-157">`event`: objeto Event</span><span class="sxs-lookup"><span data-stu-id="ecc96-157">`event`: event object</span></span> | <span data-ttu-id="ecc96-158">O modelo usado para renderizar o conteúdo adicional de cada evento.</span><span class="sxs-lookup"><span data-stu-id="ecc96-158">The template used to render additional content for each event.</span></span> |
| `header` | <span data-ttu-id="ecc96-159">`header`: String</span><span class="sxs-lookup"><span data-stu-id="ecc96-159">`header`: string</span></span> | <span data-ttu-id="ecc96-160">O modelo usado para renderizar o cabeçalho de cada dia.</span><span class="sxs-lookup"><span data-stu-id="ecc96-160">The template used to render the header for each day.</span></span> |
| `loading` | <span data-ttu-id="ecc96-161">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="ecc96-161">No data context is passed</span></span> | <span data-ttu-id="ecc96-162">O modelo usado quando os dados estão sendo carregados.</span><span class="sxs-lookup"><span data-stu-id="ecc96-162">The template used when data is loading.</span></span> |
| `no-data` | <span data-ttu-id="ecc96-163">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="ecc96-163">No data context is passed</span></span> | <span data-ttu-id="ecc96-164">O modelo usado quando não há eventos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="ecc96-164">The template used when no events are available.</span></span> |

<span data-ttu-id="ecc96-165">Os exemplos a seguir ilustram como usar o `event` modelo:</span><span class="sxs-lookup"><span data-stu-id="ecc96-165">The following examples illustrates how to use the `event` template:</span></span>

```html
<mgt-agenda>
  <template data-type="event">
    <button class="eventButton">
      <div class="event-subject">{{ event.subject }}</div>
      <div data-for="attendee in event.attendees">
        <mgt-person
          person-query="{{ attendee.emailAddress.name }}"
          show-name
          show-email>
        </mgt-person>
      </div>
    </button>
  </template>
  <template data-type="no-data">
    There are no events found!
  </template>
</mgt-agenda>
```

<span data-ttu-id="ecc96-166">Para saber mais, confira [modelos](../templates.md).</span><span class="sxs-lookup"><span data-stu-id="ecc96-166">To learn more, see [templates](../templates.md).</span></span>

## <a name="events"></a><span data-ttu-id="ecc96-167">Eventos</span><span class="sxs-lookup"><span data-stu-id="ecc96-167">Events</span></span>

<span data-ttu-id="ecc96-168">Os eventos a seguir são acionados do controle.</span><span class="sxs-lookup"><span data-stu-id="ecc96-168">The following events are fired from the control.</span></span>

| <span data-ttu-id="ecc96-169">Evento</span><span class="sxs-lookup"><span data-stu-id="ecc96-169">Event</span></span> | <span data-ttu-id="ecc96-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecc96-170">Description</span></span> |
| --- | --- |
| <span data-ttu-id="ecc96-171">eventClick</span><span class="sxs-lookup"><span data-stu-id="ecc96-171">eventClick</span></span> | <span data-ttu-id="ecc96-172">O usuário clica ou toca em um evento.</span><span class="sxs-lookup"><span data-stu-id="ecc96-172">The user clicks or taps an event.</span></span>|

## <a name="permissions"></a><span data-ttu-id="ecc96-173">Permissões</span><span class="sxs-lookup"><span data-stu-id="ecc96-173">Permissions</span></span>

<span data-ttu-id="ecc96-174">Este componente usa as seguintes APIs e permissões do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="ecc96-174">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="ecc96-175">Recurso</span><span class="sxs-lookup"><span data-stu-id="ecc96-175">Resource</span></span> | <span data-ttu-id="ecc96-176">Permissão</span><span class="sxs-lookup"><span data-stu-id="ecc96-176">Permission</span></span> |
| - | - |
| [<span data-ttu-id="ecc96-177">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="ecc96-177">/me/calendarview</span></span>](/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | <span data-ttu-id="ecc96-178">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ecc96-178">Calendars.Read</span></span> |

<span data-ttu-id="ecc96-179">O componente permite que você especifique uma consulta diferente do Microsoft Graph para chamar (como `/groups/{id}/calendar/calendarView` ).</span><span class="sxs-lookup"><span data-stu-id="ecc96-179">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="ecc96-180">Nesse caso, acrescente a permissão ao final da cadeia de caracteres, delimitado por `|` .</span><span class="sxs-lookup"><span data-stu-id="ecc96-180">In this case, append the permission to the end of the string, delimited by `|`.</span></span>

<span data-ttu-id="ecc96-181">Ao usar o modelo padrão e o `renderAttendees` modelo padrão, são necessárias APIs e permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="ecc96-181">When using the default template and default `renderAttendees` template, additional APIs and permissions are required.</span></span> <span data-ttu-id="ecc96-182">O modelo padrão para esse componente usa um componente de [Gerenciamento de pessoas](people.md) para eventos que têm participantes, o que requer o seguinte.</span><span class="sxs-lookup"><span data-stu-id="ecc96-182">The default template for this component uses a [mgt-people](people.md) component for events that have attendees, which requires the following.</span></span>

| <span data-ttu-id="ecc96-183">Recurso</span><span class="sxs-lookup"><span data-stu-id="ecc96-183">Resource</span></span> | <span data-ttu-id="ecc96-184">Permissão</span><span class="sxs-lookup"><span data-stu-id="ecc96-184">Permission</span></span> |
| - | - |
| [<span data-ttu-id="ecc96-185">/Users</span><span class="sxs-lookup"><span data-stu-id="ecc96-185">/users</span></span>](/graph/api/user-list?view=graph-rest-1.0) | <span data-ttu-id="ecc96-186">Users. ReadBasic. All</span><span class="sxs-lookup"><span data-stu-id="ecc96-186">Users.ReadBasic.All</span></span> |
| [<span data-ttu-id="ecc96-187">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="ecc96-187">/me/calendarview</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="ecc96-188">People.Read</span><span class="sxs-lookup"><span data-stu-id="ecc96-188">People.Read</span></span> |
| [<span data-ttu-id="ecc96-189">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="ecc96-189">/me/calendarview</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0) | <span data-ttu-id="ecc96-190">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ecc96-190">Contacts.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="ecc96-191">Autenticação</span><span class="sxs-lookup"><span data-stu-id="ecc96-191">Authentication</span></span>

<span data-ttu-id="ecc96-192">O controle de logon aproveita o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="ecc96-192">The login control leverages the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="ecc96-193">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="ecc96-193">Extend for more control</span></span>

<span data-ttu-id="ecc96-194">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected` métodos render \* para substituição em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="ecc96-194">For more complex scenarios or a truly custom UX, this component exposes several `protected` render\* methods for override in component extensions.</span></span>

| <span data-ttu-id="ecc96-195">Método</span><span class="sxs-lookup"><span data-stu-id="ecc96-195">Method</span></span> | <span data-ttu-id="ecc96-196">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecc96-196">Description</span></span> |
| - | - |
| <span data-ttu-id="ecc96-197">renderLoading</span><span class="sxs-lookup"><span data-stu-id="ecc96-197">renderLoading</span></span> | <span data-ttu-id="ecc96-198">Renderiza um estado de carregamento enquanto o componente é carregado.</span><span class="sxs-lookup"><span data-stu-id="ecc96-198">Renders a loading state while the component loads.</span></span> |
| <span data-ttu-id="ecc96-199">renderNoData</span><span class="sxs-lookup"><span data-stu-id="ecc96-199">renderNoData</span></span> | <span data-ttu-id="ecc96-200">Renderiza um estado de dados vazio.</span><span class="sxs-lookup"><span data-stu-id="ecc96-200">Renders an empty data state.</span></span> |
| <span data-ttu-id="ecc96-201">renderGroups</span><span class="sxs-lookup"><span data-stu-id="ecc96-201">renderGroups</span></span> | <span data-ttu-id="ecc96-202">Classifica dados de eventos em grupos e os renderiza com cabeçalhos de grupo.</span><span class="sxs-lookup"><span data-stu-id="ecc96-202">Sorts event data into groups and renders them with group headers.</span></span> |
| <span data-ttu-id="ecc96-203">renderHeader</span><span class="sxs-lookup"><span data-stu-id="ecc96-203">renderHeader</span></span> | <span data-ttu-id="ecc96-204">Renderiza um cabeçalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="ecc96-204">Renders a group header.</span></span> |
| <span data-ttu-id="ecc96-205">renderEvents</span><span class="sxs-lookup"><span data-stu-id="ecc96-205">renderEvents</span></span> | <span data-ttu-id="ecc96-206">Renderiza uma lista de objetos Event.</span><span class="sxs-lookup"><span data-stu-id="ecc96-206">Renders a list of event objects.</span></span> |
| <span data-ttu-id="ecc96-207">renderEvent</span><span class="sxs-lookup"><span data-stu-id="ecc96-207">renderEvent</span></span> | <span data-ttu-id="ecc96-208">Renderiza um evento singular e todas as suas partes.</span><span class="sxs-lookup"><span data-stu-id="ecc96-208">Renders a singular event and all of its parts.</span></span>
| <span data-ttu-id="ecc96-209">renderTitle</span><span class="sxs-lookup"><span data-stu-id="ecc96-209">renderTitle</span></span> | <span data-ttu-id="ecc96-210">Renderiza a parte do título do evento.</span><span class="sxs-lookup"><span data-stu-id="ecc96-210">Renders the event title part.</span></span> |
| <span data-ttu-id="ecc96-211">renderLocation</span><span class="sxs-lookup"><span data-stu-id="ecc96-211">renderLocation</span></span> | <span data-ttu-id="ecc96-212">Renderiza a parte do local do evento.</span><span class="sxs-lookup"><span data-stu-id="ecc96-212">Renders the event location part.</span></span> |
| <span data-ttu-id="ecc96-213">renderAttendees</span><span class="sxs-lookup"><span data-stu-id="ecc96-213">renderAttendees</span></span> | <span data-ttu-id="ecc96-214">Renderiza a parte dos participantes do evento.</span><span class="sxs-lookup"><span data-stu-id="ecc96-214">Renders the event attendees part.</span></span> |
| <span data-ttu-id="ecc96-215">renderOther</span><span class="sxs-lookup"><span data-stu-id="ecc96-215">renderOther</span></span> | <span data-ttu-id="ecc96-216">Renderiza o conteúdo do evento adicional.</span><span class="sxs-lookup"><span data-stu-id="ecc96-216">Renders additional event content.</span></span> |
