---
title: Modelos no Microsoft Graph Toolkit
description: Use modelos personalizados para modificar o conteúdo de um componente.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 59dbda5b18e1c8cb0c858c073a25f4a76b121fe6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955747"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Modelos no Microsoft Graph Toolkit

Use modelos personalizados para modificar o conteúdo de um componente.

Todos os componentes Web oferecem suporte a `<template>` modelos baseados no elemento. Por exemplo, para substituir o modelo de um componente, adicione um `<template>` elemento dentro de um componente.

```html
<mgt-agenda>
  <template data-type="event">
      <div>{{event.subject}}</div>
      <div data-for='attendee in event.attendees'>
          <mgt-person person-query="{{attendee.emailAddress.name}}">
            <template>
              <div data-if="person.image">
                <img src="{{person.image}}" />
              </div>
              <div data-else>
                {{person.displayName}}
              </div>
            </template>
          </mgt-person>
      </div>
  </template>
</mgt-agenda>
```

## <a name="data-type"></a>Tipo de dados

Cada componente pode ter várias partes que podem ser modeladas. Por exemplo, no `mgt-agenda` componente, você pode modelar eventos individuais, cabeçalhos de seção individuais, modo de exibição de carregamento, sem exibição de dados e muito mais. Para indicar o modelo, use o `data-type` atributo em um modelo. Por exemplo, para modelar cada evento `mgt-agenda`no, use `event` o tipo de dados, conforme mostrado.

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

Se não `data-type` for especificado, o componente inteiro será substituído pelo modelo. Você também pode usar `data-type="default"` para o mesmo objetivo.

## <a name="binding-data"></a>Dados de vinculação

Muitos modelos permitem a associação de dados que são passados para o modelo como contexto de dados. Por exemplo, o `event` modelo no `mgt-agenda` componente passa um `{event}` objeto que pode ser usado diretamente no modelo. Para expandir uma expressão, como `event.subject`, use as chaves duplas.

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

Este formato também pode ser usado dentro de atributos:

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> **Observação:** Você também pode expandir objetos como `{{event}}` e eles serão renderizados como cadeias de caracteres JSON. Isso pode ser útil quando você está desenvolvendo os modelos.

## <a name="data-context-helper-properties"></a>Propriedades do auxiliar de contexto de dados

As propriedades a seguir também podem ser usadas com o objeto de contexto de dados em seus modelos.

| Propriedade |  Descrição |
| --- | --- | --- |
| $index | Índice numérico do item que está sendo processado durante o loop `data-for`. |
| $parent | Se um modelo é renderizado dentro de outro modelo, essa propriedade permite que você acesse o contexto de dados pai. |

O exemplo a seguir mostra como usar a `$index` Propriedade em um loop data-para.

```html
<mgt-person>
  <mgt-person-card>
    <template data-type="additional-details">
      <span data-for="language in languages">
        {{ language.displayName }}<span data-if="$index < languages.length - 1">, </span>
      </span>
    </template>
  </mgt-person-card>
</mgt-person>
```

## <a name="conditional-rendering"></a>Renderização condicional

Você só pode querer renderizar elementos quando uma condição for true ou false com base no contexto de dados. Os `data-if` atributos `data-else` e podem avaliar uma expressão e renderizar somente se true ou false.

```html
<mgt-person person-query="john doe">
  <template>
    <div data-if="person.image">
      <img src="{{ person.image }}" />
    </div>
    <div data-else>
      {{ person.displayName }}
    </div>
  </template>
</mgt-person>
```

## <a name="looping"></a>Loop

Haverá casos em que o objeto de contexto de dados contém loop e você precisará fazer um loop sobre os dados. Neste cenário, use o `data-for` atributo.

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="converters"></a>Conversores

Em muitos casos, talvez você queira transformar os dados antes de apresentá-los no modelo. Por exemplo, você pode querer formatar corretamente uma data antes de ela ser renderizada. Nesses casos, talvez você queira usar um conversor de modelos.

Para usar um conversor de modelos, primeiro é necessário definir uma função que fará a conversão. Por exemplo, você pode definir uma função para formatar uma data.

```ts
getTimeRange(event) {
  // TODO: format a string from the event object as you wish
  // timeRange = ...

  return timeRange;
}
```

Em seguida, defina um novo conversor no elemento e nomeie-o conforme você vir ajustar.

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.templateConverters["myConverter"] = getTimeRange;
```

Para usar o conversor no seu modelo, use as chaves triplas.

```html
<template data-type="event">
  <div>{{{ myConverter(event) }}}</div>
</template>
```

Você também pode usar funções internas sem definir o conversor de modelos.

```html
<template data-type="event">
  <div>{{{ event.subject.toUpperCase() }}}</div>
</template>
```

## <a name="template-rendered-event"></a>Evento de modelo renderizado

Em certos casos, talvez você queira obter uma referência para o elemento renderizado. Isso pode ser útil para adicionar ouvintes de eventos a elementos no modelo. Neste cenário, você pode usar o `templateRendered` evento.

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

Os detalhes do evento conterão a referência ao elemento que está sendo renderizado, o objeto de contexto de dados e o tipo de modelo.

```ts
agenda.addEventListener('templateRendered', (e) => { 
  let templateType = e.detail.templateType;
  let dataContext = e.detail.context;
  let element = e.detail.element;

  if (type === 'event') {
    element.querySelector('.some-button').addEventListener('click', () => {});
  }
});
```

## <a name="styling"></a>Estilo

Os modelos podem ser estilizados normalmente por meio de CSS, pois eles são renderizados fora do dom de sombra.
