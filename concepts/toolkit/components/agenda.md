---
title: Componente agenda no microsoft Graph Toolkit
description: O componente web mgt-agenda é usado para representar eventos em um calendário de usuário ou grupo.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 6787f7d5ce8804b4f24306b0b17ad47024d227b5
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589046"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a>Componente agenda no microsoft Graph Toolkit

O `mgt-agenda` componente Web representa eventos em um calendário de usuário ou grupo. Por padrão, o calendário exibe os eventos de usuário atuais assinados no dia atual. O componente também pode usar qualquer ponto de extremidade que retorne eventos do Microsoft Graph.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra os eventos de calendário do usuário assinado exibidos usando o `mgt-agenda` componente. Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a>Propriedades

Por padrão, o `mgt-agenda` componente busca eventos do `/me/calendarview` ponto de extremidade e exibe eventos para o dia atual. Há várias propriedades que você pode usar para alterar esse comportamento.

| Atributo | Propriedade | Descrição |
| --- | --- | --- |
| data | data | Uma cadeia de caracteres que representa a data de início dos eventos a buscar da Microsoft Graph. O valor deve estar em um formato que pode ser analisado pelo construtor [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - o valor não terá efeito se `event-query` o atributo for definido. |
| days | days | Um número de dias para buscar do Microsoft Graph - o padrão é 3 - o valor não terá efeito se `event-query` o atributo for definido. |
| show-max | showMax | Um número para indicar o número máximo de eventos a mostrar. O valor padrão não está definido (nenhum máximo). |
| group-id | groupId | Uma ID de cadeia de caracteres para um calendário de grupo a ser usado em vez do calendário atual do usuário. |
| event-query | eventQuery | Uma cadeia de caracteres que representa uma consulta alternativa a ser usada ao buscar eventos da Microsoft Graph. Opcionalmente, adicione o escopo delegado no final da cadeia de caracteres delimitando-o com `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`). |
| events | events | Uma matriz de eventos para obter ou definir a lista de eventos renderizados pelo componente - use essa propriedade para acessar os eventos carregados pelo componente. De definir esse valor para carregar seus próprios eventos - se o valor for definido pelo desenvolvedor, `date`os atributos , ou não `days``event-query` terão efeito. |
| group-by-day | groupByDay | Um valor Boolean para agrupar eventos por dia - por padrão, os eventos não são agrupados. |
| preferred-timezone | preferredTimezone | Nome do fuso horário preferencial a ser usado ao recuperar eventos do Microsoft Graph; por exemplo, `Pacific Standard Time`. Por padrão, esse atributo usa o fuso horário UTC. O fuso horário preferencial para o usuário atual `me/mailboxSettings` pode ser recuperado chamando o ponto de extremidade e lendo o valor da **propriedade timeZone** . |

O exemplo a seguir altera o comportamento do componente para buscar dados para uma data específica e até três dias.

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

## <a name="methods"></a>Métodos
| Método | Descrição |
| --- | --- |
| reload() | Chame o método para recarregar o componente com novos dados potenciais com base em suas propriedades. |

## <a name="css-custom-properties"></a>Propriedades personalizadas CSS

O `mgt-agenda` componente define essas propriedades personalizadas CSS

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

Para saber mais, confira [componentes de estilo](../customize-components/style.md).

## <a name="templates"></a>Modelos

O `mgt-agenda` componente dá suporte a [vários modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e de `data-type` definir o valor como um dos seguintes:

| Tipo de dados | Contexto de dados | Descrição |
| --- | --- | --- |
| `default` | `events`: lista de objetos de evento | O modelo padrão substitui todo o componente por seu próprio. |
| `event` | `event`: objeto event | O modelo usado para renderizar cada evento. |
| `event-other` | `event`: objeto event | O modelo usado para renderizar conteúdo adicional para cada evento. |
| `header` | `header`: string | O modelo usado para renderizar o header para cada dia. |
| `loading` | Nenhum contexto de dados é passado | O modelo usado quando os dados estão sendo carregados. |
| `no-data` | Nenhum contexto de dados é passado | O modelo usado quando nenhum evento está disponível. |

Os exemplos a seguir ilustram como usar o `event` modelo:

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

Para saber mais, confira [modelos](../customize-components/templates.md).

## <a name="events"></a>Eventos

Os eventos a seguir são disparados do controle.

Evento | Quando é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`eventClick` | O usuário clica ou toca em um evento. | Evento [selecionado](/graph/api/resources/event) | Não | Não | Sim, com modelo **de evento** personalizado

Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este componente usa as seguintes APIs Graph Microsoft e permissões:

| Configuração | Permissão | API
| - | - | - |
| Padrão. | Calendars.Read | [/me/calendarview](/graph/api/calendar-list-calendarview) |

O componente permite que você especifique uma consulta Graph Microsoft para chamar (como `/groups/{id}/calendar/calendarView`). Nesse caso, anexar a permissão ao final da cadeia de caracteres, delimitada por `|`.

Ao usar o modelo padrão e o modelo `renderAttendees` padrão, APIs e permissões adicionais são necessárias. O modelo padrão para esse componente usa um [componente mgt-people](people.md) para eventos que têm participantes e herda todas as permissões.

## <a name="authentication"></a>Autenticação

O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).

## <a name="cache"></a>Cache

O `mgt-agenda` componente não armazena dados em cache.

## <a name="extend-for-more-control"></a>Estender para obter mais controle

Para cenários mais complexos ou um UX realmente personalizado, `protected` esse componente expõe vários métodos render* para substituição em extensões de componentes.

| Método | Descrição |
| - | - |
| renderLoading | Renderiza um estado de carregamento enquanto o componente é carregado. |
| renderNoData | Renderiza um estado de dados vazio. |
| renderGroups | Classifica os dados de eventos em grupos e os renderiza com os headers de grupo. |
| renderHeader | Renderiza um header de grupo. |
| renderEvents | Renderiza uma lista de objetos de evento. |
| renderEvent | Renderiza um evento singular e todas as suas partes.
| renderTitle | Renderiza a parte do título do evento. |
| renderLocation | Renderiza a parte do local do evento. |
| renderAttendees | Renderiza a parte dos participantes do evento. |
| renderOther | Renderiza conteúdo de evento adicional. |
