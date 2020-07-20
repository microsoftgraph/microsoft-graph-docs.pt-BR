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
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a>Componente de agenda no kit de ferramentas do Microsoft Graph

O `mgt-agenda` componente da Web representa eventos em um calendário de usuário ou grupo. Por padrão, o calendário exibe o atual eventos de usuário conectado para o dia atual. O componente também pode usar qualquer ponto de extremidade que retorne eventos do Microsoft Graph.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra os eventos de calendário do usuário conectado exibidos usando o `mgt-agenda` componente. Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-agenda` componente busca eventos do ponto de `/me/calendarview` extremidade e exibe eventos para o dia atual. Há várias propriedades que você pode usar para alterar esse comportamento.

| Atributo | Propriedade | Descrição |
| --- | --- | --- |
| data | data | Uma cadeia de caracteres que representa a data de início dos eventos a serem buscados do Microsoft Graph. O valor deve estar em um formato que pode ser analisado pelo [Construtor de data](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) -o valor não tem efeito se o `event-query` atributo for definido. |
| durante | durante | Um número de dias para buscar do Microsoft Graph-padrão é de 3 valores não tem efeito se o `event-query` atributo for definido. |
| show-Max | showMax | Um número para indicar o número máximo de eventos a serem exibidos. O valor padrão não é definido (sem máximo). |
| ID de grupo | groupId | Uma ID de cadeia de caracteres para um calendário de grupo a ser usado em vez do calendário do usuário conectado no momento. |
| evento-consulta | eventQuery | Uma cadeia de caracteres que representa uma consulta alternativa a ser usada ao buscar eventos do Microsoft Graph. Opcionalmente, adicione o escopo delegado no final da cadeia de caracteres, delimitadondo-o com `|` ( `/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all` ). |
| eventos | eventos | Uma matriz de eventos para obter ou definir a lista de eventos renderizados pelo componente-Use essa propriedade para acessar os eventos carregados pelo componente. Defina esse valor para carregar seus próprios eventos, se o valor for definido por desenvolvedor, `date` os `days` atributos, ou `event-query` não terão efeito. |
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
| `event-other` | `event`: objeto Event | O modelo usado para renderizar o conteúdo adicional de cada evento. |
| `header` | `header`: String | O modelo usado para renderizar o cabeçalho de cada dia. |
| `loading` | Nenhum contexto de dados é passado | O modelo usado quando os dados estão sendo carregados. |
| `no-data` | Nenhum contexto de dados é passado | O modelo usado quando não há eventos disponíveis. |

Os exemplos a seguir ilustram como usar o `event` modelo:

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

## <a name="permissions"></a>Permissões

Este componente usa as seguintes APIs e permissões do Microsoft Graph:

| Recurso | Permissão |
| - | - |
| [/me/calendarview](/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | Calendars.Read |

O componente permite que você especifique uma consulta diferente do Microsoft Graph para chamar (como `/groups/{id}/calendar/calendarView` ). Nesse caso, acrescente a permissão ao final da cadeia de caracteres, delimitado por `|` .

Ao usar o modelo padrão e o `renderAttendees` modelo padrão, são necessárias APIs e permissões adicionais. O modelo padrão para esse componente usa um componente de [Gerenciamento de pessoas](people.md) para eventos que têm participantes, o que requer o seguinte.

| Recurso | Permissão |
| - | - |
| [/Users](/graph/api/user-list?view=graph-rest-1.0) | Users. ReadBasic. All |
| [/me/calendarview](/graph/api/user-list-people?view=graph-rest-1.0) | People.Read |
| [/me/calendarview](/graph/api/user-list-contacts?view=graph-rest-1.0) | Contacts.Read |

## <a name="authentication"></a>Autenticação

O controle de logon aproveita o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).

## <a name="extend-for-more-control"></a>Estender para mais controle

Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected` métodos render * para substituição em extensões de componente.

| Método | Descrição |
| - | - |
| renderLoading | Renderiza um estado de carregamento enquanto o componente é carregado. |
| renderNoData | Renderiza um estado de dados vazio. |
| renderGroups | Classifica dados de eventos em grupos e os renderiza com cabeçalhos de grupo. |
| renderHeader | Renderiza um cabeçalho de grupo. |
| renderEvents | Renderiza uma lista de objetos Event. |
| renderEvent | Renderiza um evento singular e todas as suas partes.
| renderTitle | Renderiza a parte do título do evento. |
| renderLocation | Renderiza a parte do local do evento. |
| renderAttendees | Renderiza a parte dos participantes do evento. |
| renderOther | Renderiza o conteúdo do evento adicional. |
