---
title: Componente de agenda no kit de ferramentas do Microsoft Graph
description: O componente de gerenciamento de agenda da Web é usado para representar eventos em um calendário de usuário ou grupo.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e66ffed1f10de5c4c9b9b322d9070074ec707000
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659545"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="9db1e-103">Componente de agenda no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9db1e-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9db1e-104">O `mgt-agenda` componente da Web representa eventos em um calendário de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="9db1e-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="9db1e-105">Por padrão, o calendário exibe o atual eventos de usuário conectado para o dia atual.</span><span class="sxs-lookup"><span data-stu-id="9db1e-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="9db1e-106">O componente também pode usar qualquer ponto de extremidade que retorne eventos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9db1e-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="9db1e-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9db1e-107">Example</span></span>

<span data-ttu-id="9db1e-108">O exemplo a seguir mostra os eventos de calendário do usuário conectado exibidos usando o `mgt-agenda` componente.</span><span class="sxs-lookup"><span data-stu-id="9db1e-108">The following example shows the signed-in user's calendar events displayed using the `mgt-agenda` component.</span></span> <span data-ttu-id="9db1e-109">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="9db1e-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[<span data-ttu-id="9db1e-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="9db1e-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a><span data-ttu-id="9db1e-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9db1e-111">Properties</span></span>

<span data-ttu-id="9db1e-112">Por padrão, o `mgt-agenda` componente busca eventos do ponto de `/me/calendarview` extremidade e exibe eventos para o dia atual.</span><span class="sxs-lookup"><span data-stu-id="9db1e-112">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="9db1e-113">Há várias propriedades que você pode usar para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="9db1e-113">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="9db1e-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="9db1e-114">Attribute</span></span> | <span data-ttu-id="9db1e-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9db1e-115">Property</span></span> | <span data-ttu-id="9db1e-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="9db1e-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="9db1e-117">data</span><span class="sxs-lookup"><span data-stu-id="9db1e-117">date</span></span> | <span data-ttu-id="9db1e-118">data</span><span class="sxs-lookup"><span data-stu-id="9db1e-118">date</span></span> | <span data-ttu-id="9db1e-119">Uma cadeia de caracteres que representa a data de início dos eventos a serem buscados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9db1e-119">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="9db1e-120">O valor deve estar em um formato que pode ser analisado pelo [Construtor de data](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) -o valor não tem efeito se o `event-query` atributo for definido.</span><span class="sxs-lookup"><span data-stu-id="9db1e-120">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="9db1e-121">durante</span><span class="sxs-lookup"><span data-stu-id="9db1e-121">days</span></span> | <span data-ttu-id="9db1e-122">durante</span><span class="sxs-lookup"><span data-stu-id="9db1e-122">days</span></span> | <span data-ttu-id="9db1e-123">Um número de dias para buscar do Microsoft Graph-padrão é de 3 valores não tem efeito se o `event-query` atributo for definido.</span><span class="sxs-lookup"><span data-stu-id="9db1e-123">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="9db1e-124">show-Max</span><span class="sxs-lookup"><span data-stu-id="9db1e-124">show-max</span></span> | <span data-ttu-id="9db1e-125">showMax</span><span class="sxs-lookup"><span data-stu-id="9db1e-125">showMax</span></span> | <span data-ttu-id="9db1e-126">Um número para indicar o número máximo de eventos a serem exibidos.</span><span class="sxs-lookup"><span data-stu-id="9db1e-126">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="9db1e-127">O valor padrão não é definido (sem máximo).</span><span class="sxs-lookup"><span data-stu-id="9db1e-127">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="9db1e-128">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="9db1e-128">group-id</span></span> | <span data-ttu-id="9db1e-129">groupId</span><span class="sxs-lookup"><span data-stu-id="9db1e-129">groupId</span></span> | <span data-ttu-id="9db1e-130">Uma ID de cadeia de caracteres para um calendário de grupo a ser usado em vez do calendário do usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="9db1e-130">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="9db1e-131">evento-consulta</span><span class="sxs-lookup"><span data-stu-id="9db1e-131">event-query</span></span> | <span data-ttu-id="9db1e-132">eventQuery</span><span class="sxs-lookup"><span data-stu-id="9db1e-132">eventQuery</span></span> | <span data-ttu-id="9db1e-133">Uma cadeia de caracteres que representa uma consulta alternativa a ser usada ao buscar eventos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9db1e-133">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="9db1e-134">Opcionalmente, adicione o escopo delegado no final da cadeia de caracteres, delimitadondo-o com `|` ( `/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all` ).</span><span class="sxs-lookup"><span data-stu-id="9db1e-134">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="9db1e-135">events</span><span class="sxs-lookup"><span data-stu-id="9db1e-135">events</span></span> | <span data-ttu-id="9db1e-136">events</span><span class="sxs-lookup"><span data-stu-id="9db1e-136">events</span></span> | <span data-ttu-id="9db1e-137">Uma matriz de eventos para obter ou definir a lista de eventos renderizados pelo componente-Use essa propriedade para acessar os eventos carregados pelo componente.</span><span class="sxs-lookup"><span data-stu-id="9db1e-137">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="9db1e-138">Defina esse valor para carregar seus próprios eventos, se o valor for definido por desenvolvedor, `date` os `days` atributos, ou `event-query` não terão efeito.</span><span class="sxs-lookup"><span data-stu-id="9db1e-138">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="9db1e-139">grupo por dia</span><span class="sxs-lookup"><span data-stu-id="9db1e-139">group-by-day</span></span> | <span data-ttu-id="9db1e-140">groupByDay</span><span class="sxs-lookup"><span data-stu-id="9db1e-140">groupByDay</span></span> | <span data-ttu-id="9db1e-141">Um valor Boolean para agrupar eventos por dia-por eventos padrão não são agrupados.</span><span class="sxs-lookup"><span data-stu-id="9db1e-141">A Boolean value to group events by day - by default events are not grouped.</span></span> |
| <span data-ttu-id="9db1e-142">fuso horário preferido</span><span class="sxs-lookup"><span data-stu-id="9db1e-142">preferred-timezone</span></span> | <span data-ttu-id="9db1e-143">preferredTimezone</span><span class="sxs-lookup"><span data-stu-id="9db1e-143">preferredTimezone</span></span> | <span data-ttu-id="9db1e-144">Nome do fuso horário preferencial a ser usado ao recuperar eventos do Microsoft Graph; por exemplo, `Pacific Standard Time` .</span><span class="sxs-lookup"><span data-stu-id="9db1e-144">Name of the preferred time zone to use when retrieving events from Microsoft Graph; for example, `Pacific Standard Time`.</span></span> <span data-ttu-id="9db1e-145">Por padrão, esse atributo usa o fuso horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9db1e-145">By default, this attribute uses the UTC time zone.</span></span> <span data-ttu-id="9db1e-146">O fuso horário preferencial para o usuário atual pode ser recuperado chamando-se o `me/mailboxSettings` ponto de extremidade e lendo o valor da propriedade **timeZone** .</span><span class="sxs-lookup"><span data-stu-id="9db1e-146">The preferred time zone for the current user can be retrieved by calling the `me/mailboxSettings` endpoint and reading the value of the **timeZone** property.</span></span> |

<span data-ttu-id="9db1e-147">O exemplo a seguir altera o comportamento do componente para buscar dados de uma data específica e até três dias.</span><span class="sxs-lookup"><span data-stu-id="9db1e-147">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="9db1e-148">O exemplo a seguir altera o comportamento do componente para buscar dados de uma consulta específica.</span><span class="sxs-lookup"><span data-stu-id="9db1e-148">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="methods"></a><span data-ttu-id="9db1e-149">Métodos</span><span class="sxs-lookup"><span data-stu-id="9db1e-149">Methods</span></span>
| <span data-ttu-id="9db1e-150">Método</span><span class="sxs-lookup"><span data-stu-id="9db1e-150">Method</span></span> | <span data-ttu-id="9db1e-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="9db1e-151">Description</span></span> |
| --- | --- |
| <span data-ttu-id="9db1e-152">reload ()</span><span class="sxs-lookup"><span data-stu-id="9db1e-152">reload()</span></span> | <span data-ttu-id="9db1e-153">Chame o método para recarregar o componente com possíveis novos dados com base em suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="9db1e-153">Call the method to reload the component with potential new data based on its properties.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="9db1e-154">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="9db1e-154">CSS custom properties</span></span>

<span data-ttu-id="9db1e-155">O `mgt-agenda` componente define essas propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="9db1e-155">The `mgt-agenda` component defines these CSS custom properties</span></span>

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

<span data-ttu-id="9db1e-156">Para saber mais, confira [estilos de componentes](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="9db1e-156">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="9db1e-157">Modelos</span><span class="sxs-lookup"><span data-stu-id="9db1e-157">Templates</span></span>

<span data-ttu-id="9db1e-158">O `mgt-agenda` componente oferece suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="9db1e-158">The `mgt-agenda` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="9db1e-159">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="9db1e-159">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="9db1e-160">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="9db1e-160">Data type</span></span> | <span data-ttu-id="9db1e-161">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="9db1e-161">Data context</span></span> | <span data-ttu-id="9db1e-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="9db1e-162">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="9db1e-163">`events`: lista de objetos Event</span><span class="sxs-lookup"><span data-stu-id="9db1e-163">`events`: list of event objects</span></span> | <span data-ttu-id="9db1e-164">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="9db1e-164">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="9db1e-165">`event`: objeto Event</span><span class="sxs-lookup"><span data-stu-id="9db1e-165">`event`: event object</span></span> | <span data-ttu-id="9db1e-166">O modelo usado para renderizar cada evento.</span><span class="sxs-lookup"><span data-stu-id="9db1e-166">The template used to render each event.</span></span> |
| `event-other` | <span data-ttu-id="9db1e-167">`event`: objeto Event</span><span class="sxs-lookup"><span data-stu-id="9db1e-167">`event`: event object</span></span> | <span data-ttu-id="9db1e-168">O modelo usado para renderizar o conteúdo adicional de cada evento.</span><span class="sxs-lookup"><span data-stu-id="9db1e-168">The template used to render additional content for each event.</span></span> |
| `header` | <span data-ttu-id="9db1e-169">`header`: String</span><span class="sxs-lookup"><span data-stu-id="9db1e-169">`header`: string</span></span> | <span data-ttu-id="9db1e-170">O modelo usado para renderizar o cabeçalho de cada dia.</span><span class="sxs-lookup"><span data-stu-id="9db1e-170">The template used to render the header for each day.</span></span> |
| `loading` | <span data-ttu-id="9db1e-171">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="9db1e-171">No data context is passed</span></span> | <span data-ttu-id="9db1e-172">O modelo usado quando os dados estão sendo carregados.</span><span class="sxs-lookup"><span data-stu-id="9db1e-172">The template used when data is loading.</span></span> |
| `no-data` | <span data-ttu-id="9db1e-173">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="9db1e-173">No data context is passed</span></span> | <span data-ttu-id="9db1e-174">O modelo usado quando não há eventos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="9db1e-174">The template used when no events are available.</span></span> |

<span data-ttu-id="9db1e-175">Os exemplos a seguir ilustram como usar o `event` modelo:</span><span class="sxs-lookup"><span data-stu-id="9db1e-175">The following examples illustrates how to use the `event` template:</span></span>

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

<span data-ttu-id="9db1e-176">Para saber mais, confira [modelos](../customize-components/templates.md).</span><span class="sxs-lookup"><span data-stu-id="9db1e-176">To learn more, see [templates](../customize-components/templates.md).</span></span>

## <a name="events"></a><span data-ttu-id="9db1e-177">Eventos</span><span class="sxs-lookup"><span data-stu-id="9db1e-177">Events</span></span>

<span data-ttu-id="9db1e-178">Os eventos a seguir são acionados do controle.</span><span class="sxs-lookup"><span data-stu-id="9db1e-178">The following events are fired from the control.</span></span>

| <span data-ttu-id="9db1e-179">Evento</span><span class="sxs-lookup"><span data-stu-id="9db1e-179">Event</span></span> | <span data-ttu-id="9db1e-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="9db1e-180">Description</span></span> |
| --- | --- |
| <span data-ttu-id="9db1e-181">eventClick</span><span class="sxs-lookup"><span data-stu-id="9db1e-181">eventClick</span></span> | <span data-ttu-id="9db1e-182">O usuário clica ou toca em um evento.</span><span class="sxs-lookup"><span data-stu-id="9db1e-182">The user clicks or taps an event.</span></span>|

## <a name="permissions"></a><span data-ttu-id="9db1e-183">Permissões</span><span class="sxs-lookup"><span data-stu-id="9db1e-183">Permissions</span></span>

<span data-ttu-id="9db1e-184">Este componente usa as seguintes APIs e permissões do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="9db1e-184">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="9db1e-185">Recurso</span><span class="sxs-lookup"><span data-stu-id="9db1e-185">Resource</span></span> | <span data-ttu-id="9db1e-186">Permissão</span><span class="sxs-lookup"><span data-stu-id="9db1e-186">Permission</span></span> |
| - | - |
| [<span data-ttu-id="9db1e-187">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="9db1e-187">/me/calendarview</span></span>](/graph/api/calendar-list-calendarview) | <span data-ttu-id="9db1e-188">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9db1e-188">Calendars.Read</span></span> |

<span data-ttu-id="9db1e-189">O componente permite que você especifique uma consulta diferente do Microsoft Graph para chamar (como `/groups/{id}/calendar/calendarView` ).</span><span class="sxs-lookup"><span data-stu-id="9db1e-189">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="9db1e-190">Nesse caso, acrescente a permissão ao final da cadeia de caracteres, delimitado por `|` .</span><span class="sxs-lookup"><span data-stu-id="9db1e-190">In this case, append the permission to the end of the string, delimited by `|`.</span></span>

<span data-ttu-id="9db1e-191">Ao usar o modelo padrão e o `renderAttendees` modelo padrão, são necessárias APIs e permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="9db1e-191">When using the default template and default `renderAttendees` template, additional APIs and permissions are required.</span></span> <span data-ttu-id="9db1e-192">O modelo padrão para esse componente usa um componente de [Gerenciamento de pessoas](people.md) para eventos que têm participantes, o que requer o seguinte.</span><span class="sxs-lookup"><span data-stu-id="9db1e-192">The default template for this component uses a [mgt-people](people.md) component for events that have attendees, which requires the following.</span></span>

| <span data-ttu-id="9db1e-193">Recurso</span><span class="sxs-lookup"><span data-stu-id="9db1e-193">Resource</span></span> | <span data-ttu-id="9db1e-194">Permissão</span><span class="sxs-lookup"><span data-stu-id="9db1e-194">Permission</span></span> |
| - | - |
| [<span data-ttu-id="9db1e-195">/Users</span><span class="sxs-lookup"><span data-stu-id="9db1e-195">/users</span></span>](/graph/api/user-list) | <span data-ttu-id="9db1e-196">Users. ReadBasic. All</span><span class="sxs-lookup"><span data-stu-id="9db1e-196">Users.ReadBasic.All</span></span> |
| [<span data-ttu-id="9db1e-197">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="9db1e-197">/me/calendarview</span></span>](/graph/api/user-list-people) | <span data-ttu-id="9db1e-198">People.Read</span><span class="sxs-lookup"><span data-stu-id="9db1e-198">People.Read</span></span> |
| [<span data-ttu-id="9db1e-199">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="9db1e-199">/me/calendarview</span></span>](/graph/api/user-list-contacts) | <span data-ttu-id="9db1e-200">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9db1e-200">Contacts.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="9db1e-201">Autenticação</span><span class="sxs-lookup"><span data-stu-id="9db1e-201">Authentication</span></span>

<span data-ttu-id="9db1e-202">O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="9db1e-202">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="9db1e-203">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="9db1e-203">Extend for more control</span></span>

<span data-ttu-id="9db1e-204">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected` métodos render \* para substituição em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="9db1e-204">For more complex scenarios or a truly custom UX, this component exposes several `protected` render\* methods for override in component extensions.</span></span>

| <span data-ttu-id="9db1e-205">Método</span><span class="sxs-lookup"><span data-stu-id="9db1e-205">Method</span></span> | <span data-ttu-id="9db1e-206">Descrição</span><span class="sxs-lookup"><span data-stu-id="9db1e-206">Description</span></span> |
| - | - |
| <span data-ttu-id="9db1e-207">renderLoading</span><span class="sxs-lookup"><span data-stu-id="9db1e-207">renderLoading</span></span> | <span data-ttu-id="9db1e-208">Renderiza um estado de carregamento enquanto o componente é carregado.</span><span class="sxs-lookup"><span data-stu-id="9db1e-208">Renders a loading state while the component loads.</span></span> |
| <span data-ttu-id="9db1e-209">renderNoData</span><span class="sxs-lookup"><span data-stu-id="9db1e-209">renderNoData</span></span> | <span data-ttu-id="9db1e-210">Renderiza um estado de dados vazio.</span><span class="sxs-lookup"><span data-stu-id="9db1e-210">Renders an empty data state.</span></span> |
| <span data-ttu-id="9db1e-211">renderGroups</span><span class="sxs-lookup"><span data-stu-id="9db1e-211">renderGroups</span></span> | <span data-ttu-id="9db1e-212">Classifica dados de eventos em grupos e os renderiza com cabeçalhos de grupo.</span><span class="sxs-lookup"><span data-stu-id="9db1e-212">Sorts event data into groups and renders them with group headers.</span></span> |
| <span data-ttu-id="9db1e-213">renderHeader</span><span class="sxs-lookup"><span data-stu-id="9db1e-213">renderHeader</span></span> | <span data-ttu-id="9db1e-214">Renderiza um cabeçalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="9db1e-214">Renders a group header.</span></span> |
| <span data-ttu-id="9db1e-215">renderEvents</span><span class="sxs-lookup"><span data-stu-id="9db1e-215">renderEvents</span></span> | <span data-ttu-id="9db1e-216">Renderiza uma lista de objetos Event.</span><span class="sxs-lookup"><span data-stu-id="9db1e-216">Renders a list of event objects.</span></span> |
| <span data-ttu-id="9db1e-217">renderEvent</span><span class="sxs-lookup"><span data-stu-id="9db1e-217">renderEvent</span></span> | <span data-ttu-id="9db1e-218">Renderiza um evento singular e todas as suas partes.</span><span class="sxs-lookup"><span data-stu-id="9db1e-218">Renders a singular event and all of its parts.</span></span>
| <span data-ttu-id="9db1e-219">renderTitle</span><span class="sxs-lookup"><span data-stu-id="9db1e-219">renderTitle</span></span> | <span data-ttu-id="9db1e-220">Renderiza a parte do título do evento.</span><span class="sxs-lookup"><span data-stu-id="9db1e-220">Renders the event title part.</span></span> |
| <span data-ttu-id="9db1e-221">renderLocation</span><span class="sxs-lookup"><span data-stu-id="9db1e-221">renderLocation</span></span> | <span data-ttu-id="9db1e-222">Renderiza a parte do local do evento.</span><span class="sxs-lookup"><span data-stu-id="9db1e-222">Renders the event location part.</span></span> |
| <span data-ttu-id="9db1e-223">renderAttendees</span><span class="sxs-lookup"><span data-stu-id="9db1e-223">renderAttendees</span></span> | <span data-ttu-id="9db1e-224">Renderiza a parte dos participantes do evento.</span><span class="sxs-lookup"><span data-stu-id="9db1e-224">Renders the event attendees part.</span></span> |
| <span data-ttu-id="9db1e-225">renderOther</span><span class="sxs-lookup"><span data-stu-id="9db1e-225">renderOther</span></span> | <span data-ttu-id="9db1e-226">Renderiza o conteúdo do evento adicional.</span><span class="sxs-lookup"><span data-stu-id="9db1e-226">Renders additional event content.</span></span> |
