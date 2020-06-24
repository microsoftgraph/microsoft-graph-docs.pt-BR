---
title: Modelos no Microsoft Graph Toolkit
description: Use modelos personalizados para modificar o conteúdo de um componente.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 4f855558b8b1ee5d0f84b9998b62c2f770a4dc6b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845950"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Modelos no Microsoft Graph Toolkit

Use modelos personalizados para modificar o conteúdo de um componente.

Todos os componentes Web oferecem suporte a modelos baseados no `<template>` elemento. Por exemplo, para substituir o modelo de um componente, adicione um `<template>` elemento dentro de um componente.

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

Cada componente pode ter várias partes que podem ser modeladas. Por exemplo, no `mgt-agenda` componente, você pode modelar eventos individuais, cabeçalhos de seção individuais, modo de exibição de carregamento, sem exibição de dados e muito mais. Para indicar o modelo, use o `data-type` atributo em um modelo. Por exemplo, para modelar cada evento no `mgt-agenda` , use o `event` tipo de dados, conforme mostrado.

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

Se não `data-type` for especificado, o componente inteiro será substituído pelo modelo. Você também pode usar `data-type="default"` para o mesmo objetivo.

## <a name="binding-data"></a>Dados de vinculação

Muitos modelos permitem a associação de dados que são passados para o modelo como contexto de dados. Por exemplo, o `event` modelo no `mgt-agenda` componente passa um `{event}` objeto que pode ser usado diretamente no modelo. Para expandir uma expressão, como `event.subject` , use as chaves duplas.

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

### <a name="change-binding-syntax"></a>Alterar sintaxe de associação

Por padrão, para expandir uma expressão, você usa chaves duplas ( `{{expression}}` ). No entanto, você pode alterar essa sintaxe para ambientes onde a sintaxe de chave dupla já é usada. Por exemplo, o exemplo a seguir usa colchetes duplos ( `[[expression]]` ).

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a>Propriedades do auxiliar de contexto de dados

As propriedades a seguir também podem ser usadas com o objeto de contexto de dados em seus modelos.

| Propriedade | Descrição                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| $index   | Índice numérico do item que está sendo processado durante o loop `data-for` .                                     |
| $parent  | Se um modelo é renderizado dentro de outro modelo, essa propriedade permite que você acesse o contexto de dados pai. |

O exemplo a seguir mostra como usar a `$index` propriedade em um loop data-para.

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

Você só pode querer renderizar elementos quando uma condição for true ou false com base no contexto de dados. Os `data-if` `data-else` atributos e podem avaliar uma expressão e renderizar somente se true ou false.

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

## <a name="template-context"></a>Contexto de modelo

Em cenários em que você precisa converter dados em suas associações, vincular a eventos ou apenas usar dados externos em associações de modelos, os modelos dão suporte à associação a contexto de dados externos. Você pode adicionar contexto de modelo adicional de duas maneiras:

1. Diretamente no componente.

    Cada componente define a `templateContext` propriedade, que você pode usar para passar dados adicionais para qualquer modelo no componente.

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    Agora, as propriedades no `templateContext` objeto estarão disponíveis para serem usadas nas expressões de associação no modelo.

2. Globalmente para todos os componentes.

    A `TemplateHelper` classe expõe o `globalContext` objeto para adicionar dados ou funções que devem estar disponíveis globalmente para todos os componentes.

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a>Conversores

Em muitos casos, talvez você queira transformar os dados antes de apresentá-los no modelo. Por exemplo, você pode querer formatar corretamente uma data antes de ela ser renderizada. Nesses casos, talvez você queira usar um conversor de modelos.

Para usar um conversor de modelos, primeiro é necessário definir uma função que fará a conversão. Por exemplo, você pode definir uma função para converter um objeto de evento em um intervalo de tempo formatado.

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

Para usar o conversor no seu modelo, use-o como se você tivesse usado uma função no code-behind.

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a>Associação de evento ou propriedade

O `data-props` atributo permite adicionar um ouvinte de eventos ou definir um valor de propriedade diretamente em seus modelos.

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

Os dados-props aceitam uma cadeia de caracteres delimitada por vírgulas para cada propriedade ou manipulador de eventos que você queira definir.

Para adicionar um manipulador de eventos, Prefixe o nome do evento com `@` . O manipulador de eventos deverá estar disponível no `templateContext` do elemento.

```ts
document.querySelector('mgt-agenda').templateContext = {

  someEventHandler: (e, context, root) => { /* handleEvent */  }

}
```

```html
<template>
    <button data-props="{{@click: someEventHandler}}"></button>
</template>
```

Os argumentos de evento, o contexto de dados e o elemento raiz do modelo são passados para o manipulador de eventos como parâmetros.


## <a name="template-rendered-event"></a>Evento de modelo renderizado

Em certos casos, talvez você queira obter uma referência para o elemento renderizado. Isso pode ser útil se você quiser manipular a renderização do conteúdo sozinho ou se quiser modificar o elemento renderizado.

Neste cenário, você pode usar o `templateRendered` evento, que é acionado depois que o modelo é renderizado.

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

Os detalhes do evento conterão uma referência ao elemento que está sendo renderizado, o objeto de contexto de dados e o tipo de modelo.

```ts
agenda.addEventListener('templateRendered', (e) => {
  let templateType = e.detail.templateType;
  let dataContext = e.detail.context;
  let element = e.detail.element;

  if (templateType === 'event') {
    element.querySelector('.some-button').addEventListener('click', () => {});
  }
});
```

## <a name="styling"></a>Estilo

Os modelos podem ser estilizados normalmente por meio de CSS, pois eles são renderizados fora do dom de sombra.
