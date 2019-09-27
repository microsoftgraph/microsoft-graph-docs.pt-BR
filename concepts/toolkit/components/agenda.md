---
title: Componente de agenda no kit de ferramentas do Microsoft Graph
description: O componente de gerenciamento de agenda da Web é usado para representar eventos em um calendário de usuário ou grupo.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0afe3546541e38349404b80abac48073b90f7eb4
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275729"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d429d-103">Componente de agenda no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d429d-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d429d-104">O `mgt-agenda` componente da Web representa eventos em um calendário de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="d429d-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="d429d-105">Por padrão, o calendário exibe o atual eventos de usuário conectado para o dia atual.</span><span class="sxs-lookup"><span data-stu-id="d429d-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="d429d-106">O componente também pode usar qualquer ponto de extremidade que retorne eventos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d429d-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span> 

## <a name="example"></a><span data-ttu-id="d429d-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d429d-107">Example</span></span>

[<span data-ttu-id="d429d-108">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="d429d-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/ojt2c7vp/)

```html
<mgt-agenda group-by-day></mgt-agenda>
```

![gerenciamento-agenda](./images/mgt-agenda.png)

## <a name="properties"></a><span data-ttu-id="d429d-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d429d-110">Properties</span></span>

<span data-ttu-id="d429d-111">Por padrão, o `mgt-agenda` componente busca eventos do `/me/calendarview` ponto de extremidade e exibe eventos para o dia atual.</span><span class="sxs-lookup"><span data-stu-id="d429d-111">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="d429d-112">Há várias propriedades que você pode usar para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="d429d-112">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="d429d-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d429d-113">Property</span></span> | <span data-ttu-id="d429d-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="d429d-114">Attribute</span></span> | <span data-ttu-id="d429d-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="d429d-115">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="d429d-116">data</span><span class="sxs-lookup"><span data-stu-id="d429d-116">date</span></span> | <span data-ttu-id="d429d-117">data</span><span class="sxs-lookup"><span data-stu-id="d429d-117">date</span></span> | <span data-ttu-id="d429d-118">Uma cadeia de caracteres que representa a data de início dos eventos a serem buscados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d429d-118">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="d429d-119">O valor deve estar em um formato que pode ser analisado pelo [Construtor de data](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) -o valor não tem `event-query` efeito se o atributo for definido.</span><span class="sxs-lookup"><span data-stu-id="d429d-119">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="d429d-120">durante</span><span class="sxs-lookup"><span data-stu-id="d429d-120">days</span></span> | <span data-ttu-id="d429d-121">durante</span><span class="sxs-lookup"><span data-stu-id="d429d-121">days</span></span> | <span data-ttu-id="d429d-122">Um número de dias para buscar do Microsoft Graph-padrão é de 3 valores não tem efeito se `event-query` o atributo for definido.</span><span class="sxs-lookup"><span data-stu-id="d429d-122">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="d429d-123">showMax</span><span class="sxs-lookup"><span data-stu-id="d429d-123">showMax</span></span> | <span data-ttu-id="d429d-124">show-Max</span><span class="sxs-lookup"><span data-stu-id="d429d-124">show-max</span></span> | <span data-ttu-id="d429d-125">Um número para indicar o número máximo de eventos a serem exibidos.</span><span class="sxs-lookup"><span data-stu-id="d429d-125">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="d429d-126">O valor padrão não é definido (sem máximo).</span><span class="sxs-lookup"><span data-stu-id="d429d-126">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="d429d-127">groupId</span><span class="sxs-lookup"><span data-stu-id="d429d-127">groupId</span></span> | <span data-ttu-id="d429d-128">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="d429d-128">group-id</span></span> | <span data-ttu-id="d429d-129">Uma ID de cadeia de caracteres para um calendário de grupo a ser usado em vez do calendário do usuário conectado no momento.</span><span class="sxs-lookup"><span data-stu-id="d429d-129">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="d429d-130">eventQuery</span><span class="sxs-lookup"><span data-stu-id="d429d-130">eventQuery</span></span> | <span data-ttu-id="d429d-131">evento-consulta</span><span class="sxs-lookup"><span data-stu-id="d429d-131">event-query</span></span> | <span data-ttu-id="d429d-132">Uma cadeia de caracteres que representa uma consulta alternativa a ser usada ao buscar eventos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d429d-132">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="d429d-133">Opcionalmente, adicione o escopo delegado no final da cadeia de caracteres, delimitadondo-o com `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span><span class="sxs-lookup"><span data-stu-id="d429d-133">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="d429d-134">eventos</span><span class="sxs-lookup"><span data-stu-id="d429d-134">events</span></span> | <span data-ttu-id="d429d-135">eventos</span><span class="sxs-lookup"><span data-stu-id="d429d-135">events</span></span> | <span data-ttu-id="d429d-136">Uma matriz de eventos para obter ou definir a lista de eventos renderizados pelo componente-Use essa propriedade para acessar os eventos carregados pelo componente.</span><span class="sxs-lookup"><span data-stu-id="d429d-136">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="d429d-137">Defina esse valor para carregar seus próprios eventos, se o valor for definido por desenvolvedor, `date`os `days`atributos, `event-query` ou não terão efeito.</span><span class="sxs-lookup"><span data-stu-id="d429d-137">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="d429d-138">groupByDay</span><span class="sxs-lookup"><span data-stu-id="d429d-138">groupByDay</span></span> | <span data-ttu-id="d429d-139">grupo por dia</span><span class="sxs-lookup"><span data-stu-id="d429d-139">group-by-day</span></span> | <span data-ttu-id="d429d-140">Um valor Boolean para agrupar eventos por dia-por eventos padrão não são agrupados.</span><span class="sxs-lookup"><span data-stu-id="d429d-140">A Boolean value to group events by day - by default events are not grouped.</span></span> |

<span data-ttu-id="d429d-141">O exemplo a seguir altera o comportamento do componente para buscar dados de uma data específica e até três dias.</span><span class="sxs-lookup"><span data-stu-id="d429d-141">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="d429d-142">O exemplo a seguir altera o comportamento do componente para buscar dados de uma consulta específica.</span><span class="sxs-lookup"><span data-stu-id="d429d-142">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a><span data-ttu-id="d429d-143">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="d429d-143">CSS custom properties</span></span>

<span data-ttu-id="d429d-144">O `mgt-agenda` componente define essas propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="d429d-144">The `mgt-agenda` component defines these CSS custom properties</span></span>

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

<span data-ttu-id="d429d-145">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="d429d-145">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="d429d-146">Modelos</span><span class="sxs-lookup"><span data-stu-id="d429d-146">Templates</span></span>

<span data-ttu-id="d429d-147">O `mgt-agenda` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="d429d-147">The `mgt-agenda` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="d429d-148">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="d429d-148">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="d429d-149">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="d429d-149">Data type</span></span> | <span data-ttu-id="d429d-150">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="d429d-150">Data context</span></span> | <span data-ttu-id="d429d-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="d429d-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="d429d-152">`events`: lista de objetos Event</span><span class="sxs-lookup"><span data-stu-id="d429d-152">`events`: list of event objects</span></span> | <span data-ttu-id="d429d-153">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="d429d-153">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="d429d-154">`event`: objeto Event</span><span class="sxs-lookup"><span data-stu-id="d429d-154">`event`: event object</span></span> | <span data-ttu-id="d429d-155">O modelo usado para renderizar cada evento.</span><span class="sxs-lookup"><span data-stu-id="d429d-155">The template used to render each event.</span></span> |
| `header` | <span data-ttu-id="d429d-156">`header`: String</span><span class="sxs-lookup"><span data-stu-id="d429d-156">`header`: string</span></span> | <span data-ttu-id="d429d-157">O modelo usado para renderizar o cabeçalho de cada dia.</span><span class="sxs-lookup"><span data-stu-id="d429d-157">The template used to render the header for each day.</span></span> |
| `other` | <span data-ttu-id="d429d-158">`event`: objeto Event</span><span class="sxs-lookup"><span data-stu-id="d429d-158">`event`: event object</span></span> | <span data-ttu-id="d429d-159">O modelo usado para renderizar o conteúdo adicional de cada evento.</span><span class="sxs-lookup"><span data-stu-id="d429d-159">The template used to render additional content for each event.</span></span> |
| `no-data` | <span data-ttu-id="d429d-160">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="d429d-160">No data context is passed</span></span> | <span data-ttu-id="d429d-161">O modelo usado quando não há eventos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="d429d-161">The template used when no events are available.</span></span> |
| `loading` | <span data-ttu-id="d429d-162">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="d429d-162">No data context is passed</span></span> | <span data-ttu-id="d429d-163">O modelo usado quando os dados estão sendo carregados.</span><span class="sxs-lookup"><span data-stu-id="d429d-163">The template used when data is loading.</span></span> |

<span data-ttu-id="d429d-164">Os exemplos a seguir ilustram como usar `event` o modelo:</span><span class="sxs-lookup"><span data-stu-id="d429d-164">The following examples illustrates how to use the `event` template:</span></span>

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

<span data-ttu-id="d429d-165">Para saber mais, confira [modelos](../templates.md).</span><span class="sxs-lookup"><span data-stu-id="d429d-165">To learn more, see [templates](../templates.md).</span></span>

## <a name="graph-scopes"></a><span data-ttu-id="d429d-166">Escopos de gráfico</span><span class="sxs-lookup"><span data-stu-id="d429d-166">Graph scopes</span></span>

<span data-ttu-id="d429d-167">Este componente usa as seguintes APIs e permissões do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="d429d-167">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="d429d-168">recurso</span><span class="sxs-lookup"><span data-stu-id="d429d-168">resource</span></span> | <span data-ttu-id="d429d-169">permissão/escopo</span><span class="sxs-lookup"><span data-stu-id="d429d-169">permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="d429d-170">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="d429d-170">/me/calendarview</span></span>](https://docs.microsoft.com/en-us/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | `Calendars.Read` |

<span data-ttu-id="d429d-171">O componente permite que você especifique uma consulta diferente do Microsoft Graph para chamar (como `/groups/{id}/calendar/calendarView`).</span><span class="sxs-lookup"><span data-stu-id="d429d-171">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="d429d-172">Nesse caso, acrescente o escopo no final da cadeia de caracteres, delimitado por`|`</span><span class="sxs-lookup"><span data-stu-id="d429d-172">In this case, append the scope at the end of the string, delimited by `|`</span></span>

## <a name="authentication"></a><span data-ttu-id="d429d-173">Autenticação</span><span class="sxs-lookup"><span data-stu-id="d429d-173">Authentication</span></span>

<span data-ttu-id="d429d-174">O controle de logon aproveita o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="d429d-174">The login control leverages the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

