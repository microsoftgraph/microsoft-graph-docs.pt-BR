---
title: Componente de agenda no kit de ferramentas do Microsoft Graph
description: O componente de gerenciamento de agenda da Web é usado para representar eventos em um calendário de usuário ou grupo.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 8a91b20a48c1646fafd8cd7a287f037615024a73
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242946"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="8e23a-103">Componente de agenda no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8e23a-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8e23a-104">O `mgt-agenda` componente da Web representa eventos em um calendário de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="8e23a-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="8e23a-105">Por padrão, o calendário exibe o atual eventos de usuário conectado para o dia atual.</span><span class="sxs-lookup"><span data-stu-id="8e23a-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="8e23a-106">O componente também pode usar qualquer ponto de extremidade que retorne eventos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8e23a-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span> 

## <a name="example"></a><span data-ttu-id="8e23a-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e23a-107">Example</span></span>

[<span data-ttu-id="8e23a-108">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="8e23a-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/ojt2c7vp/)

```html
<mgt-agenda group-by-day></mgt-agenda>
```

![gerenciamento-agenda](./images/mgt-agenda.png)

## <a name="properties"></a><span data-ttu-id="8e23a-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e23a-110">Properties</span></span>

<span data-ttu-id="8e23a-111">Por padrão, o `mgt-agenda` componente busca eventos do `/me/calendarview` ponto de extremidade e exibe eventos para o dia atual.</span><span class="sxs-lookup"><span data-stu-id="8e23a-111">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="8e23a-112">Há várias propriedades que você pode usar para alterar esse comportamento.</span><span class="sxs-lookup"><span data-stu-id="8e23a-112">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="8e23a-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e23a-113">Property</span></span> | <span data-ttu-id="8e23a-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="8e23a-114">Attribute</span></span> | <span data-ttu-id="8e23a-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e23a-115">Description</span></span> |
| --- | --- | --- |
| `groupByDay` | `group-by-day` | <span data-ttu-id="8e23a-116">Um valor Boolean para agrupar eventos por dia-por eventos padrão não são agrupados.</span><span class="sxs-lookup"><span data-stu-id="8e23a-116">A Boolean value to group events by day - by default events are not grouped.</span></span> |
| `date` | `date` | <span data-ttu-id="8e23a-117">Uma cadeia de caracteres que representa a data de início dos eventos a serem buscados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8e23a-117">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="8e23a-118">O valor deve estar em um formato que pode ser analisado pelo [Construtor de data](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) -o valor não tem `event-query` efeito se o atributo for definido.</span><span class="sxs-lookup"><span data-stu-id="8e23a-118">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| `days` | `days` | <span data-ttu-id="8e23a-119">Um número de dias para buscar do Microsoft Graph-padrão é de 3 valores não tem efeito se `event-query` o atributo for definido.</span><span class="sxs-lookup"><span data-stu-id="8e23a-119">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| `eventQuery` | `event-query` | <span data-ttu-id="8e23a-120">Uma cadeia de caracteres que representa uma consulta alternativa a ser usada ao buscar eventos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8e23a-120">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="8e23a-121">Opcionalmente, adicione o escopo delegado no final da cadeia de caracteres, delimitadondo-o com `|` (`"/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all"`).</span><span class="sxs-lookup"><span data-stu-id="8e23a-121">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`"/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all"`).</span></span> |
| `events` | `events` | <span data-ttu-id="8e23a-122">Uma matriz de eventos para obter ou definir a lista de eventos renderizados pelo componente-Use essa propriedade para acessar os eventos carregados pelo componente.</span><span class="sxs-lookup"><span data-stu-id="8e23a-122">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="8e23a-123">Defina esse valor para carregar seus próprios eventos, se o valor for definido por desenvolvedor, `date`os `days`atributos, `event-query` ou não terão efeito.</span><span class="sxs-lookup"><span data-stu-id="8e23a-123">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |

<span data-ttu-id="8e23a-124">O exemplo a seguir altera o comportamento do componente para buscar dados para uma data específica e até 3 dias.</span><span class="sxs-lookup"><span data-stu-id="8e23a-124">The following example changes the behavior of the component to fetch data for a specific date and up to 3 days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="8e23a-125">O exemplo a seguir altera o comportamento do componente para buscar dados de uma consulta específica.</span><span class="sxs-lookup"><span data-stu-id="8e23a-125">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a><span data-ttu-id="8e23a-126">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="8e23a-126">CSS Custom properties</span></span>

<span data-ttu-id="8e23a-127">O `mgt-agenda` componente define essas propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="8e23a-127">The `mgt-agenda` component defines these CSS custom properties</span></span>

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

<span data-ttu-id="8e23a-128">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="8e23a-128">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="8e23a-129">Modelos</span><span class="sxs-lookup"><span data-stu-id="8e23a-129">Templates</span></span>

<span data-ttu-id="8e23a-130">O `mgt-agenda` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="8e23a-130">The `mgt-agenda` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="8e23a-131">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="8e23a-131">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="8e23a-132">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="8e23a-132">Data type</span></span> | <span data-ttu-id="8e23a-133">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="8e23a-133">Data context</span></span> | <span data-ttu-id="8e23a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e23a-134">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="8e23a-135">`events`: lista de objetos Event</span><span class="sxs-lookup"><span data-stu-id="8e23a-135">`events`: list of event objects</span></span> | <span data-ttu-id="8e23a-136">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="8e23a-136">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="8e23a-137">`event`: objeto Event</span><span class="sxs-lookup"><span data-stu-id="8e23a-137">`event`: event object</span></span> | <span data-ttu-id="8e23a-138">O modelo usado para renderizar cada evento.</span><span class="sxs-lookup"><span data-stu-id="8e23a-138">The template used to render each event.</span></span> |
| `header` | <span data-ttu-id="8e23a-139">`header`: String</span><span class="sxs-lookup"><span data-stu-id="8e23a-139">`header`: string</span></span> | <span data-ttu-id="8e23a-140">O modelo usado para renderizar o cabeçalho de cada dia.</span><span class="sxs-lookup"><span data-stu-id="8e23a-140">The template used to render the header for each day.</span></span> |
| `other` | <span data-ttu-id="8e23a-141">`event`: objeto Event</span><span class="sxs-lookup"><span data-stu-id="8e23a-141">`event`: event object</span></span> | <span data-ttu-id="8e23a-142">O modelo usado para renderizar o conteúdo adicional de cada evento.</span><span class="sxs-lookup"><span data-stu-id="8e23a-142">The template used to render additional content for each event.</span></span> |
| `no-data` | <span data-ttu-id="8e23a-143">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="8e23a-143">No data context is passed</span></span> | <span data-ttu-id="8e23a-144">O modelo usado quando não há eventos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="8e23a-144">The template used when no events are available.</span></span> |
| `loading` | <span data-ttu-id="8e23a-145">Nenhum contexto de dados é passado</span><span class="sxs-lookup"><span data-stu-id="8e23a-145">No data context is passed</span></span> | <span data-ttu-id="8e23a-146">O modelo usado quando os dados estão sendo carregados.</span><span class="sxs-lookup"><span data-stu-id="8e23a-146">The template used when data is loading.</span></span> |

<span data-ttu-id="8e23a-147">Os exemplos a seguir ilustram como usar `event` o modelo:</span><span class="sxs-lookup"><span data-stu-id="8e23a-147">The following examples illustrates how to use the `event` template:</span></span>

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

<span data-ttu-id="8e23a-148">Para saber mais, confira [modelos](../templates.md).</span><span class="sxs-lookup"><span data-stu-id="8e23a-148">To learn more, see [templates](../templates.md).</span></span>

## <a name="graph-scopes"></a><span data-ttu-id="8e23a-149">Escopos de gráfico</span><span class="sxs-lookup"><span data-stu-id="8e23a-149">Graph scopes</span></span>

<span data-ttu-id="8e23a-150">Este componente usa as seguintes APIs e permissões do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="8e23a-150">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="8e23a-151">recurso</span><span class="sxs-lookup"><span data-stu-id="8e23a-151">resource</span></span> | <span data-ttu-id="8e23a-152">permissão/escopo</span><span class="sxs-lookup"><span data-stu-id="8e23a-152">permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="8e23a-153">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="8e23a-153">/me/calendarview</span></span>](https://docs.microsoft.com/en-us/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | `Calendars.Read` |

<span data-ttu-id="8e23a-154">O componente permite que você especifique uma consulta diferente do Microsoft Graph para chamar (como `/groups/{id}/calendar/calendarView`).</span><span class="sxs-lookup"><span data-stu-id="8e23a-154">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="8e23a-155">Nesse caso, acrescente o escopo no final da cadeia de caracteres, delimitado por`|`</span><span class="sxs-lookup"><span data-stu-id="8e23a-155">In this case, append the scope at the end of the string, delimited by `|`</span></span>

## <a name="authentication"></a><span data-ttu-id="8e23a-156">Autenticação</span><span class="sxs-lookup"><span data-stu-id="8e23a-156">Authentication</span></span>

<span data-ttu-id="8e23a-157">O controle de logon aproveita o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="8e23a-157">The login control leverages the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

