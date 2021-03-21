---
title: Modelos no microsoft graph Toolkit
description: Use modelos personalizados para modificar o conteúdo de um componente.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 1db3f315cd89932481a0a2325eecae19592d9276
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963278"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Modelos no microsoft graph Toolkit

A maioria dos Toolkit do Microsoft Graph suporta o uso de modelos personalizados para modificar o conteúdo de um componente.

Todos os componentes da Web suportam modelos com base no `<template>` elemento. Por exemplo, para substituir o modelo de um componente, adicione um `<template>` elemento dentro de um componente.

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

Se você estiver usando os componentes do Microsoft Graph Toolkit React, poderá usar o React para modelos de autoria. Para obter detalhes, [consulte Use the toolkit with React](../get-started/mgt-react.md).

## <a name="data-type"></a>Tipo de dados

Cada componente pode ter várias partes que podem ser modelos. Por exemplo, no componente, você pode modelo eventos individuais, headers de seção `mgt-agenda` individuais, exibição de carregamento, sem exibição de dados e muito mais. Para indicar o modelo, use o `data-type` atributo em um modelo. Por exemplo, para modelo de cada evento no `mgt-agenda` , use o tipo de `event` dados, conforme mostrado.

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

Se não `data-type` for especificado, todo o componente será substituído pelo modelo. Você também pode `data-type="default"` usar para a mesma finalidade.

## <a name="binding-data"></a>Dados de associação

Muitos modelos permitem a associação de dados que são passados para o modelo como contexto de dados. Por exemplo, o `event` modelo no componente passa um objeto que pode ser usado diretamente no `mgt-agenda` `{event}` modelo. Para expandir uma expressão, como `event.subject` , use os colchetes curvados duplos.

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

Esse formato também pode ser usado dentro de atributos:

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> **Observação:** Você também pode expandir objetos como `{{event}}` ou `{{this}}` e eles renderizarão como cadeias de caracteres JSON. Isso pode ser útil quando você estiver desenvolvendo os modelos.

### <a name="change-binding-syntax"></a>Alterar sintaxe de associação

Por padrão, para expandir uma expressão, você usa colchetes curvados duplos ( `{{expression}}` ). No entanto, você pode alterar essa sintaxe para ambientes em que a sintaxe de colchete dupla curva já é usada. Por exemplo, o exemplo a seguir usa colchetes duplos ( `[[expression]]` ).

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a>Propriedades auxiliares de contexto de dados

As propriedades a seguir também podem ser usadas com o objeto de contexto de dados em seus modelos.

| Propriedade | Descrição                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| $index   | Índice numérico do item que está sendo renderizado durante o loop com `data-for` .                                     |
| $parent  | Se um modelo for renderizado dentro de outro modelo, essa propriedade permitirá que você acesse o contexto de dados pai. |

O exemplo a seguir mostra como usar `$index` a propriedade em um loop data-for.

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

### <a name="this"></a>{{this}}

Para ajudar a depurar o contexto de dados, você pode usar `this` em suas expressões de associação. O formulário mais simples é adicionar em `{{this}}` qualquer lugar do seu modelo.

```html
<template data-type="event">
  <div>
    {{this}}
  </div>
</template>
```

Como você pode usar JavaScript em suas expressões de associação, você também tem acesso ao objeto que permite que você use (ou qualquer outra [`console`](https://developer.mozilla.org/docs/Web/API/Console) `console.log(this)` `console` API) em seus modelos.

```html
<template data-type="event">
  <div>
    {{console.log(this)}}
  </div>
</template>
```

## <a name="conditional-rendering"></a>Renderização condicional

Você só pode querer renderizar elementos quando uma condição for verdadeira ou false com base no contexto de dados. Os `data-if` atributos e podem avaliar uma expressão e `data-else` renderizar somente se for verdadeiro ou falso.

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

## <a name="looping"></a>Looping

Haverá casos em que o objeto de contexto de dados contém loop e você precisará fazer um loop sobre os dados. Para esse cenário, use o `data-for` atributo.

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="template-context"></a>Contexto do modelo

Em cenários em que você precisa converter dados em suas vinculações, vincular a eventos ou apenas usar dados externos em suas vinculações de modelos, os modelos suportam a associação ao contexto de dados externos. Você pode adicionar contexto de modelo adicional de duas maneiras:

1. Diretamente no componente.

    Cada componente define a `templateContext` propriedade, que você pode usar para passar dados adicionais para qualquer modelo no componente.

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    As propriedades no objeto agora estarão disponíveis para serem `templateContext` usadas nas expressões de associação no modelo.

2. Globalmente para todos os componentes.

    A classe expõe o objeto para adicionar dados ou funções que `TemplateHelper` `globalContext` devem estar disponíveis globalmente para todos os componentes.

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a>Conversores

Em muitos casos, talvez você queira transformar os dados antes de apresentá-los no modelo. Por exemplo, talvez você queira formatar corretamente uma data antes de ser renderizada. Nesses casos, talvez você queira usar um conversor de modelo.

Para usar um conversor de modelo, primeiro você precisa definir uma função que fará a conversão. Por exemplo, você pode definir uma função para converter um objeto de evento em um intervalo de tempo formatado.

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

Para usar o conversor em seu modelo, use-o como se você usaria uma função em code behind.

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a>Associação de eventos ou propriedades

O atributo permite adicionar um ouvinte de eventos ou definir um valor `data-props` de propriedade diretamente em seus modelos.

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

Os data-props aceitam uma cadeia de caracteres delimitada por vírgula para cada propriedade ou manipulador de eventos que você talvez queira definir.

Para adicionar um manipulador de eventos, prefixe o nome do evento com `@` . O manipulador de eventos precisará estar disponível no `templateContext` elemento.

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

Os args de evento, o contexto de dados e o elemento raiz do modelo são passados para o manipulador de eventos como parâmetros.


## <a name="template-rendered-event"></a>Evento renderizado de modelo

Em determinados casos, talvez você queira obter uma referência ao elemento renderizado. Isso pode ser útil se você quiser manipular a renderização do conteúdo por conta própria ou se quiser modificar o elemento renderizado.

Nesse cenário, você pode usar o `templateRendered` evento, que é a disparar depois que o modelo é renderizado.

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

Os detalhes do evento conterão uma referência ao elemento que está sendo renderizado, ao objeto de contexto de dados e ao tipo do modelo.

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

Os modelos podem ser estilizados normalmente via CSS à medida que são renderizados fora do dom de sombra.
