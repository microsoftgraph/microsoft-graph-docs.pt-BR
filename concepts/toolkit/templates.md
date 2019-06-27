---
title: Modelos no Microsoft Graph Toolkit
description: Use modelos personalizados para modificar o conteúdo de um componente.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: f0648d0ac1348fbadad6cebe8a022f9445fcf1e3
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242929"
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

Há suporte para os seguintes recursos de modelo:

- Use as chaves duplas (`{{expression}}`) para expandir uma expressão. No exemplo anterior, o `<mgt-person>` passa um `person` objeto que você pode usar no modelo.
- Use os `data-if` atributos `data-else` e para a renderização condicional. Expressões condicionais como `event.attendees.length > 2` são suportadas.
- Use o `data-for` para repetir um elemento.
- Use o `data-type` para especificar de que parte do componente será o modelo. Não especificar o tipo aplicará o modelo a todo o componente.

Cada componente documenta os valores `data-type` com suporte e qual contexto de dados é passado para cada modelo.

Os modelos podem ser estilizados normalmente, já que são renderizados fora do dom de sombra.
