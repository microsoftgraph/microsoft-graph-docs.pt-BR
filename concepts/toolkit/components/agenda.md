---
title: Componente de agenda no kit de ferramentas do Microsoft Graph
description: O componente de gerenciamento de agenda da Web é usado para representar eventos em um calendário de usuário ou grupo.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 334da23db286c7243b9722cae443913219a97f7f
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639944"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a>Componente de agenda no kit de ferramentas do Microsoft Graph

O `mgt-agenda` componente da Web representa eventos em um calendário de usuário ou grupo. Por padrão, o calendário exibe o atual eventos de usuário conectado para o dia atual. O componente também pode usar qualquer ponto de extremidade que retorne eventos do Microsoft Graph.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra os eventos de calendário do usuário conectado exibidos usando o `mgt-agenda` componente. Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-agenda` componente busca eventos do `/me/calendarview` ponto de extremidade e exibe eventos para o dia atual. Há várias propriedades que você pode usar para alterar esse comportamento.

| Atributo | Propriedade | Descrição |
| --- | --- | --- |
| data | data | Uma cadeia de caracteres que representa a data de início dos eventos a serem buscados do Microsoft Graph. O valor deve estar em um formato que pode ser analisado pelo [Construtor de data](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) -o valor não tem `event-query` efeito se o atributo for definido. |
| durante | durante | Um número de dias para buscar do Microsoft Graph-padrão é de 3 valores não tem efeito se `event-query` o atributo for definido. |
| show-Max | showMax | Um número para indicar o número máximo de eventos a serem exibidos. O valor padrão não é definido (sem máximo). |
| ID de grupo | groupId | Uma ID de cadeia de caracteres para um calendário de grupo a ser usado em vez do calendário do usuário conectado no momento. |
| evento-consulta | eventQuery | Uma cadeia de caracteres que representa uma consulta alternativa a ser usada ao buscar eventos do Microsoft Graph. Opcionalmente, adicione o escopo delegado no final da cadeia de caracteres, delimitadondo-o com `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`). |
| events | events | Uma matriz de eventos para obter ou definir a lista de eventos renderizados pelo componente-Use essa propriedade para acessar os eventos carregados pelo componente. Defina esse valor para carregar seus próprios eventos, se o valor for definido por desenvolvedor, `date`os `days`atributos, `event-query` ou não terão efeito. |
| grupo por dia | groupByDay | Um valor Boolean para agrupar eventos por dia-por eventos padrão não são agrupados. |

O exemplo a seguir altera o comportamento do componente para buscar dados de uma data específica e até três dias.

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

O exemplo a seguir altera o comportamento do componente para buscar dados de uma consulta específica.

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a>Propriedades personalizadas de CSS

O `mgt-agenda` componente define essas propriedades personalizadas de CSS

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

Para saber mais, confira [estilos de componentes](../style.md).

## <a name="templates"></a>Modelos

O `mgt-agenda` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes:

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| `default` | `events`: lista de objetos Event | O modelo padrão substitui todo o componente pelo seu. |
| `event` | `event`: objeto Event | O modelo usado para renderizar cada evento. |
| `header` | `header`: String | O modelo usado para renderizar o cabeçalho de cada dia. |
| `other` | `event`: objeto Event | O modelo usado para renderizar o conteúdo adicional de cada evento. |
| `no-data` | Nenhum contexto de dados é passado | O modelo usado quando não há eventos disponíveis. |
| `loading` | Nenhum contexto de dados é passado | O modelo usado quando os dados estão sendo carregados. |

Os exemplos a seguir ilustram como usar `event` o modelo:

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

Para saber mais, confira [modelos](../templates.md).

## <a name="events"></a>Eventos

Os eventos a seguir são acionados do controle.

| Evento | Descrição |
| --- | --- |
| eventClick | O usuário clica ou toca em um evento.|


## <a name="graph-scopes"></a>Escopos de gráfico

Este componente usa as seguintes APIs e permissões do Microsoft Graph:

| recurso | permissão/escopo |
| - | - |
| [/me/calendarview](/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | `Calendars.Read` |

O componente permite que você especifique uma consulta diferente do Microsoft Graph para chamar (como `/groups/{id}/calendar/calendarView`). Nesse caso, acrescente o escopo no final da cadeia de caracteres, delimitado por`|`

## <a name="authentication"></a>Autenticação

O controle de logon aproveita o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).

