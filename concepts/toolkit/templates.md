---
title: Modelos no Microsoft Graph Toolkit
description: Use modelos personalizados para modificar o conteúdo de um componente.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 00be58b006fd4442154f547603cf1f2c5dbeb5a5
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682240"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="19709-103">Modelos no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="19709-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="19709-104">Use modelos personalizados para modificar o conteúdo de um componente.</span><span class="sxs-lookup"><span data-stu-id="19709-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="19709-105">Todos os componentes Web oferecem suporte a modelos baseados no `<template>` elemento.</span><span class="sxs-lookup"><span data-stu-id="19709-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="19709-106">Por exemplo, para substituir o modelo de um componente, adicione um `<template>` elemento dentro de um componente.</span><span class="sxs-lookup"><span data-stu-id="19709-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

## <a name="data-type"></a><span data-ttu-id="19709-107">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="19709-107">Data-type</span></span>

<span data-ttu-id="19709-108">Cada componente pode ter várias partes que podem ser modeladas.</span><span class="sxs-lookup"><span data-stu-id="19709-108">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="19709-109">Por exemplo, no `mgt-agenda` componente, você pode modelar eventos individuais, cabeçalhos de seção individuais, modo de exibição de carregamento, sem exibição de dados e muito mais.</span><span class="sxs-lookup"><span data-stu-id="19709-109">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="19709-110">Para indicar o modelo, use o `data-type` atributo em um modelo.</span><span class="sxs-lookup"><span data-stu-id="19709-110">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="19709-111">Por exemplo, para modelar cada evento no `mgt-agenda` , use o `event` tipo de dados, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="19709-111">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="19709-112">Se não `data-type` for especificado, o componente inteiro será substituído pelo modelo.</span><span class="sxs-lookup"><span data-stu-id="19709-112">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="19709-113">Você também pode usar `data-type="default"` para o mesmo objetivo.</span><span class="sxs-lookup"><span data-stu-id="19709-113">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="19709-114">Dados de vinculação</span><span class="sxs-lookup"><span data-stu-id="19709-114">Binding data</span></span>

<span data-ttu-id="19709-115">Muitos modelos permitem a associação de dados que são passados para o modelo como contexto de dados.</span><span class="sxs-lookup"><span data-stu-id="19709-115">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="19709-116">Por exemplo, o `event` modelo no `mgt-agenda` componente passa um `{event}` objeto que pode ser usado diretamente no modelo.</span><span class="sxs-lookup"><span data-stu-id="19709-116">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="19709-117">Para expandir uma expressão, como `event.subject` , use as chaves duplas.</span><span class="sxs-lookup"><span data-stu-id="19709-117">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="19709-118">Este formato também pode ser usado dentro de atributos:</span><span class="sxs-lookup"><span data-stu-id="19709-118">This format can also be used inside attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="19709-119">**Observação:** Você também pode expandir objetos como `{{event}}` e eles serão renderizados como cadeias de caracteres JSON.</span><span class="sxs-lookup"><span data-stu-id="19709-119">**Note:** You can also expand objects such as `{{event}}` and they will render as JSON strings.</span></span> <span data-ttu-id="19709-120">Isso pode ser útil quando você está desenvolvendo os modelos.</span><span class="sxs-lookup"><span data-stu-id="19709-120">This can be useful when you're developing the templates.</span></span>

### <a name="change-binding-syntax"></a><span data-ttu-id="19709-121">Alterar sintaxe de associação</span><span class="sxs-lookup"><span data-stu-id="19709-121">Change binding syntax</span></span>

<span data-ttu-id="19709-122">Por padrão, para expandir uma expressão, você usa chaves duplas ( `{{expression}}` ).</span><span class="sxs-lookup"><span data-stu-id="19709-122">By default, to expand an expression, you use double curly brackets ( `{{expression}}` ).</span></span> <span data-ttu-id="19709-123">No entanto, você pode alterar essa sintaxe para ambientes onde a sintaxe de chave dupla já é usada.</span><span class="sxs-lookup"><span data-stu-id="19709-123">However, you can change this syntax for environments where the double curly bracket syntax is already used.</span></span> <span data-ttu-id="19709-124">Por exemplo, o exemplo a seguir usa colchetes duplos ( `[[expression]]` ).</span><span class="sxs-lookup"><span data-stu-id="19709-124">For example, the following example uses double square brackets ( `[[expression]]` ).</span></span>

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a><span data-ttu-id="19709-125">Propriedades do auxiliar de contexto de dados</span><span class="sxs-lookup"><span data-stu-id="19709-125">Data context helper properties</span></span>

<span data-ttu-id="19709-126">As propriedades a seguir também podem ser usadas com o objeto de contexto de dados em seus modelos.</span><span class="sxs-lookup"><span data-stu-id="19709-126">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="19709-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19709-127">Property</span></span> |  <span data-ttu-id="19709-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="19709-128">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="19709-129">$index</span><span class="sxs-lookup"><span data-stu-id="19709-129">$index</span></span> | <span data-ttu-id="19709-130">Índice numérico do item que está sendo processado durante o loop `data-for` .</span><span class="sxs-lookup"><span data-stu-id="19709-130">Numerical index of item being rendered while being looped with `data-for`.</span></span> |
| <span data-ttu-id="19709-131">$parent</span><span class="sxs-lookup"><span data-stu-id="19709-131">$parent</span></span> | <span data-ttu-id="19709-132">Se um modelo é renderizado dentro de outro modelo, essa propriedade permite que você acesse o contexto de dados pai.</span><span class="sxs-lookup"><span data-stu-id="19709-132">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="19709-133">O exemplo a seguir mostra como usar a `$index` propriedade em um loop data-para.</span><span class="sxs-lookup"><span data-stu-id="19709-133">The following example shows how to use the `$index` property in a data-for loop.</span></span>

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

## <a name="conditional-rendering"></a><span data-ttu-id="19709-134">Renderização condicional</span><span class="sxs-lookup"><span data-stu-id="19709-134">Conditional rendering</span></span>

<span data-ttu-id="19709-135">Você só pode querer renderizar elementos quando uma condição for true ou false com base no contexto de dados.</span><span class="sxs-lookup"><span data-stu-id="19709-135">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="19709-136">Os `data-if` `data-else` atributos e podem avaliar uma expressão e renderizar somente se true ou false.</span><span class="sxs-lookup"><span data-stu-id="19709-136">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="19709-137">Loop</span><span class="sxs-lookup"><span data-stu-id="19709-137">Looping</span></span>

<span data-ttu-id="19709-138">Haverá casos em que o objeto de contexto de dados contém loop e você precisará fazer um loop sobre os dados.</span><span class="sxs-lookup"><span data-stu-id="19709-138">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="19709-139">Neste cenário, use o `data-for` atributo.</span><span class="sxs-lookup"><span data-stu-id="19709-139">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="template-context"></a><span data-ttu-id="19709-140">Contexto de modelo</span><span class="sxs-lookup"><span data-stu-id="19709-140">Template context</span></span>

<span data-ttu-id="19709-141">Em cenários em que você precisa converter dados em suas associações, vincular a eventos ou apenas usar dados externos em associações de modelos, os modelos dão suporte à associação a contexto de dados externos.</span><span class="sxs-lookup"><span data-stu-id="19709-141">In scenarios where you need to convert data in your bindings, bind to events, or just use external data in your templates bindings, the templates support binding to external data context.</span></span> <span data-ttu-id="19709-142">Você pode adicionar contexto de modelo adicional de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="19709-142">You can add additional template context in two ways:</span></span>

1. <span data-ttu-id="19709-143">Diretamente no componente.</span><span class="sxs-lookup"><span data-stu-id="19709-143">Directly on the component.</span></span>

    <span data-ttu-id="19709-144">Cada componente define a `templateContext` propriedade, que você pode usar para passar dados adicionais para qualquer modelo no componente.</span><span class="sxs-lookup"><span data-stu-id="19709-144">Each component defines the `templateContext` property, which you can use to pass additional data to any template in the component.</span></span> 

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    <span data-ttu-id="19709-145">Agora, as propriedades no `templateContext` objeto estarão disponíveis para serem usadas nas expressões de associação no modelo.</span><span class="sxs-lookup"><span data-stu-id="19709-145">The properties in the `templateContext` object will now be available to be used in the binding expressions in the template.</span></span>

2. <span data-ttu-id="19709-146">Globalmente para todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="19709-146">Globally for all components.</span></span>

    <span data-ttu-id="19709-147">A `TemplateHelper` classe expõe o `globalContext` objeto para adicionar dados ou funções que devem estar disponíveis globalmente para todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="19709-147">The `TemplateHelper` class exposes the `globalContext` object to add data or functions that should be globally available for all components.</span></span>

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a><span data-ttu-id="19709-148">Conversores</span><span class="sxs-lookup"><span data-stu-id="19709-148">Converters</span></span>

<span data-ttu-id="19709-149">Em muitos casos, talvez você queira transformar os dados antes de apresentá-los no modelo.</span><span class="sxs-lookup"><span data-stu-id="19709-149">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="19709-150">Por exemplo, você pode querer formatar corretamente uma data antes de ela ser renderizada.</span><span class="sxs-lookup"><span data-stu-id="19709-150">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="19709-151">Nesses casos, talvez você queira usar um conversor de modelos.</span><span class="sxs-lookup"><span data-stu-id="19709-151">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="19709-152">Para usar um conversor de modelos, primeiro é necessário definir uma função que fará a conversão.</span><span class="sxs-lookup"><span data-stu-id="19709-152">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="19709-153">Por exemplo, você pode definir uma função para converter um objeto de evento em um intervalo de tempo formatado.</span><span class="sxs-lookup"><span data-stu-id="19709-153">For example, you might define a function to convert an event object to a formatted time range.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

<span data-ttu-id="19709-154">Para usar o conversor no seu modelo, use-o como se você tivesse usado uma função no code-behind.</span><span class="sxs-lookup"><span data-stu-id="19709-154">To use the converter in your template, use it as if you would use a function in code behind.</span></span>

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a><span data-ttu-id="19709-155">Associação de evento ou propriedade</span><span class="sxs-lookup"><span data-stu-id="19709-155">Event or property binding</span></span>

<span data-ttu-id="19709-156">O `data-props` atributo permite adicionar um ouvinte de eventos ou definir um valor de propriedade diretamente em seus modelos.</span><span class="sxs-lookup"><span data-stu-id="19709-156">The `data-props` attribute allows you to add an event listener or set a property value directly in your templates.</span></span> 

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

<span data-ttu-id="19709-157">Os dados-props aceitam uma cadeia de caracteres delimitada por vírgulas para cada propriedade ou manipulador de eventos que você queira definir.</span><span class="sxs-lookup"><span data-stu-id="19709-157">The data-props accepts a comma delimited string for each property or event handler you might want to set.</span></span> 

<span data-ttu-id="19709-158">Para adicionar um manipulador de eventos, Prefixe o nome do evento com `@` .</span><span class="sxs-lookup"><span data-stu-id="19709-158">To add an event handler, prefix the name of the event with `@`.</span></span> <span data-ttu-id="19709-159">O manipulador de eventos deverá estar disponível no `templateContext` do elemento.</span><span class="sxs-lookup"><span data-stu-id="19709-159">The event handler will need to be available in the `templateContext` of the element.</span></span>

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

<span data-ttu-id="19709-160">Os argumentos de evento, o contexto de dados e o elemento raiz do modelo são passados para o manipulador de eventos como parâmetros.</span><span class="sxs-lookup"><span data-stu-id="19709-160">The event args, data context, and the root element of the template are passed to the event handler as parameters.</span></span>


## <a name="template-rendered-event"></a><span data-ttu-id="19709-161">Evento de modelo renderizado</span><span class="sxs-lookup"><span data-stu-id="19709-161">Template rendered event</span></span>

<span data-ttu-id="19709-162">Em certos casos, talvez você queira obter uma referência para o elemento renderizado.</span><span class="sxs-lookup"><span data-stu-id="19709-162">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="19709-163">Isso pode ser útil se você quiser manipular a renderização do conteúdo sozinho ou se quiser modificar o elemento renderizado.</span><span class="sxs-lookup"><span data-stu-id="19709-163">This can be useful if you want to handle the rendering of the content yourself, or you want to modify the rendered element.</span></span>

<span data-ttu-id="19709-164">Neste cenário, você pode usar o `templateRendered` evento, que é acionado depois que o modelo é renderizado.</span><span class="sxs-lookup"><span data-stu-id="19709-164">In this scenario, you can use the `templateRendered` event, which fires after the template has been rendered.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="19709-165">Os detalhes do evento conterão uma referência ao elemento que está sendo renderizado, o objeto de contexto de dados e o tipo de modelo.</span><span class="sxs-lookup"><span data-stu-id="19709-165">The event details will contain a reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

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

## <a name="styling"></a><span data-ttu-id="19709-166">Estilo</span><span class="sxs-lookup"><span data-stu-id="19709-166">Styling</span></span>

<span data-ttu-id="19709-167">Os modelos podem ser estilizados normalmente por meio de CSS, pois eles são renderizados fora do dom de sombra.</span><span class="sxs-lookup"><span data-stu-id="19709-167">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
