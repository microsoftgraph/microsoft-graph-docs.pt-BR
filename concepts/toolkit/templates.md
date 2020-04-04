---
title: Modelos no Microsoft Graph Toolkit
description: Use modelos personalizados para modificar o conteúdo de um componente.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 46a1f9b771f358de6099bf1266c10c4c1ebe0cb0
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144258"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="0bf77-103">Modelos no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="0bf77-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="0bf77-104">Use modelos personalizados para modificar o conteúdo de um componente.</span><span class="sxs-lookup"><span data-stu-id="0bf77-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="0bf77-105">Todos os componentes Web oferecem suporte a `<template>` modelos baseados no elemento.</span><span class="sxs-lookup"><span data-stu-id="0bf77-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="0bf77-106">Por exemplo, para substituir o modelo de um componente, adicione um `<template>` elemento dentro de um componente.</span><span class="sxs-lookup"><span data-stu-id="0bf77-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

## <a name="data-type"></a><span data-ttu-id="0bf77-107">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="0bf77-107">Data-type</span></span>

<span data-ttu-id="0bf77-108">Cada componente pode ter várias partes que podem ser modeladas.</span><span class="sxs-lookup"><span data-stu-id="0bf77-108">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="0bf77-109">Por exemplo, no `mgt-agenda` componente, você pode modelar eventos individuais, cabeçalhos de seção individuais, modo de exibição de carregamento, sem exibição de dados e muito mais.</span><span class="sxs-lookup"><span data-stu-id="0bf77-109">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="0bf77-110">Para indicar o modelo, use o `data-type` atributo em um modelo.</span><span class="sxs-lookup"><span data-stu-id="0bf77-110">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="0bf77-111">Por exemplo, para modelar cada evento `mgt-agenda`no, use `event` o tipo de dados, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="0bf77-111">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="0bf77-112">Se não `data-type` for especificado, o componente inteiro será substituído pelo modelo.</span><span class="sxs-lookup"><span data-stu-id="0bf77-112">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="0bf77-113">Você também pode usar `data-type="default"` para o mesmo objetivo.</span><span class="sxs-lookup"><span data-stu-id="0bf77-113">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="0bf77-114">Dados de vinculação</span><span class="sxs-lookup"><span data-stu-id="0bf77-114">Binding data</span></span>

<span data-ttu-id="0bf77-115">Muitos modelos permitem a associação de dados que são passados para o modelo como contexto de dados.</span><span class="sxs-lookup"><span data-stu-id="0bf77-115">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="0bf77-116">Por exemplo, o `event` modelo no `mgt-agenda` componente passa um `{event}` objeto que pode ser usado diretamente no modelo.</span><span class="sxs-lookup"><span data-stu-id="0bf77-116">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="0bf77-117">Para expandir uma expressão, como `event.subject`, use as chaves duplas.</span><span class="sxs-lookup"><span data-stu-id="0bf77-117">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="0bf77-118">Este formato também pode ser usado dentro de atributos:</span><span class="sxs-lookup"><span data-stu-id="0bf77-118">This format can also be used inside of attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="0bf77-119">**Observação:** Você também pode expandir objetos como `{{event}}` e eles serão renderizados como cadeias de caracteres JSON.</span><span class="sxs-lookup"><span data-stu-id="0bf77-119">**Note:** You can also expand objects such as `{{event}}` and they will render as JSON strings.</span></span> <span data-ttu-id="0bf77-120">Isso pode ser útil quando você está desenvolvendo os modelos.</span><span class="sxs-lookup"><span data-stu-id="0bf77-120">This can be useful when you're developing the templates.</span></span>

## <a name="data-context-helper-properties"></a><span data-ttu-id="0bf77-121">Propriedades do auxiliar de contexto de dados</span><span class="sxs-lookup"><span data-stu-id="0bf77-121">Data context helper properties</span></span>

<span data-ttu-id="0bf77-122">As propriedades a seguir também podem ser usadas com o objeto de contexto de dados em seus modelos.</span><span class="sxs-lookup"><span data-stu-id="0bf77-122">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="0bf77-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bf77-123">Property</span></span> |  <span data-ttu-id="0bf77-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bf77-124">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="0bf77-125">$index</span><span class="sxs-lookup"><span data-stu-id="0bf77-125">$index</span></span> | <span data-ttu-id="0bf77-126">Índice numérico do item que está sendo processado durante o loop `data-for`.</span><span class="sxs-lookup"><span data-stu-id="0bf77-126">Numerical index of item being rendered while being looped with `data-for`.</span></span> |
| <span data-ttu-id="0bf77-127">$parent</span><span class="sxs-lookup"><span data-stu-id="0bf77-127">$parent</span></span> | <span data-ttu-id="0bf77-128">Se um modelo é renderizado dentro de outro modelo, essa propriedade permite que você acesse o contexto de dados pai.</span><span class="sxs-lookup"><span data-stu-id="0bf77-128">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="0bf77-129">O exemplo a seguir mostra como usar a `$index` Propriedade em um loop data-para.</span><span class="sxs-lookup"><span data-stu-id="0bf77-129">The following example shows how to use the `$index` property in a data-for loop.</span></span>

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

## <a name="conditional-rendering"></a><span data-ttu-id="0bf77-130">Renderização condicional</span><span class="sxs-lookup"><span data-stu-id="0bf77-130">Conditional rendering</span></span>

<span data-ttu-id="0bf77-131">Você só pode querer renderizar elementos quando uma condição for true ou false com base no contexto de dados.</span><span class="sxs-lookup"><span data-stu-id="0bf77-131">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="0bf77-132">Os `data-if` atributos `data-else` e podem avaliar uma expressão e renderizar somente se true ou false.</span><span class="sxs-lookup"><span data-stu-id="0bf77-132">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="0bf77-133">Loop</span><span class="sxs-lookup"><span data-stu-id="0bf77-133">Looping</span></span>

<span data-ttu-id="0bf77-134">Haverá casos em que o objeto de contexto de dados contém loop e você precisará fazer um loop sobre os dados.</span><span class="sxs-lookup"><span data-stu-id="0bf77-134">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="0bf77-135">Neste cenário, use o `data-for` atributo.</span><span class="sxs-lookup"><span data-stu-id="0bf77-135">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="templatecontext"></a><span data-ttu-id="0bf77-136">TemplateContext</span><span class="sxs-lookup"><span data-stu-id="0bf77-136">TemplateContext</span></span>

<span data-ttu-id="0bf77-137">Cada componente no Microsoft Graph Toolkit define a `templateContext` Propriedade, que você pode usar para passar dados adicionais para qualquer modelo no componente.</span><span class="sxs-lookup"><span data-stu-id="0bf77-137">Each component in the Microsoft Graph Toolkit defines the `templateContext` property, which you can use to pass additional data to any template in the component.</span></span> 

```ts
document.querySelector('mgt-agenda').templateContext = {

  someObject: {},
  formatDate: (date: Date) => { /* format date and return */ },
  someEventHandler: (e) => { /* handleEvent */  }

}
```

<span data-ttu-id="0bf77-138">Agora, as propriedades `templateContext` no objeto estarão disponíveis para serem usadas nas expressões de associação no modelo.</span><span class="sxs-lookup"><span data-stu-id="0bf77-138">The properties in the `templateContext` object will now be available to be used in the binding expressions in the template.</span></span>

<span data-ttu-id="0bf77-139">Isso pode ser útil em muitos cenários, como converter dados em suas associações ou vincular a eventos.</span><span class="sxs-lookup"><span data-stu-id="0bf77-139">This can be useful in many scenarios, such as converting data in your bindings, or binding to events.</span></span> 

### <a name="converters"></a><span data-ttu-id="0bf77-140">Conversores</span><span class="sxs-lookup"><span data-stu-id="0bf77-140">Converters</span></span>

<span data-ttu-id="0bf77-141">Em muitos casos, talvez você queira transformar os dados antes de apresentá-los no modelo.</span><span class="sxs-lookup"><span data-stu-id="0bf77-141">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="0bf77-142">Por exemplo, você pode querer formatar corretamente uma data antes de ela ser renderizada.</span><span class="sxs-lookup"><span data-stu-id="0bf77-142">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="0bf77-143">Nesses casos, talvez você queira usar um conversor de modelos.</span><span class="sxs-lookup"><span data-stu-id="0bf77-143">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="0bf77-144">Para usar um conversor de modelos, primeiro é necessário definir uma função que fará a conversão.</span><span class="sxs-lookup"><span data-stu-id="0bf77-144">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="0bf77-145">Por exemplo, você pode definir uma função para converter um objeto de evento em um intervalo de tempo formatado.</span><span class="sxs-lookup"><span data-stu-id="0bf77-145">For example, you might define a function to convert an event object to a formatted time range.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

<span data-ttu-id="0bf77-146">Para usar o conversor no seu modelo, use-o como se você tivesse usado uma função no code-behind.</span><span class="sxs-lookup"><span data-stu-id="0bf77-146">To use the converter in your template, use it as if you would use a function in code behind.</span></span>

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a><span data-ttu-id="0bf77-147">Associação de evento ou propriedade</span><span class="sxs-lookup"><span data-stu-id="0bf77-147">Event or property binding</span></span>

<span data-ttu-id="0bf77-148">O `data-props` atributo permite adicionar um ouvinte de eventos ou definir um valor de propriedade diretamente em seus modelos.</span><span class="sxs-lookup"><span data-stu-id="0bf77-148">The `data-props` attribute allows you to add an event listener or set a property value directly in your templates.</span></span> 

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

<span data-ttu-id="0bf77-149">Os dados-props aceitam uma cadeia de caracteres delimitada por vírgulas para cada propriedade ou manipulador de eventos que você queira definir.</span><span class="sxs-lookup"><span data-stu-id="0bf77-149">The data-props accepts a comma delimited string for each property or event handler you might want to set.</span></span> 

<span data-ttu-id="0bf77-150">Para adicionar um manipulador de eventos, Prefixe o nome do evento `@`com.</span><span class="sxs-lookup"><span data-stu-id="0bf77-150">To add an event handler, prefix the name of the event with `@`.</span></span> <span data-ttu-id="0bf77-151">O manipulador de eventos deverá estar disponível no `templateContext` do elemento.</span><span class="sxs-lookup"><span data-stu-id="0bf77-151">The event handler will need to be available in the `templateContext` of the element.</span></span>

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

<span data-ttu-id="0bf77-152">Os argumentos de evento, o contexto de dados e o elemento raiz do modelo são passados para o manipulador de eventos como parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0bf77-152">The event args, data context, and the root element of the template are passed to the event handler as parameters.</span></span>


## <a name="template-rendered-event"></a><span data-ttu-id="0bf77-153">Evento de modelo renderizado</span><span class="sxs-lookup"><span data-stu-id="0bf77-153">Template rendered event</span></span>

<span data-ttu-id="0bf77-154">Em certos casos, talvez você queira obter uma referência para o elemento renderizado.</span><span class="sxs-lookup"><span data-stu-id="0bf77-154">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="0bf77-155">Isso pode ser útil se você quiser manipular a renderização do conteúdo sozinho ou se quiser modificar o elemento renderizado.</span><span class="sxs-lookup"><span data-stu-id="0bf77-155">This can be useful if you want to handle the rendering of the content yourself, or you want to modify the rendered element.</span></span>

<span data-ttu-id="0bf77-156">Neste cenário, você pode usar o `templateRendered` evento, que é acionado depois que o modelo é renderizado.</span><span class="sxs-lookup"><span data-stu-id="0bf77-156">In this scenario, you can use the `templateRendered` event, which fires after the template has been rendered.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="0bf77-157">Os detalhes do evento conterão uma referência ao elemento que está sendo renderizado, o objeto de contexto de dados e o tipo de modelo.</span><span class="sxs-lookup"><span data-stu-id="0bf77-157">The event details will contain a reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

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

## <a name="styling"></a><span data-ttu-id="0bf77-158">Estilo</span><span class="sxs-lookup"><span data-stu-id="0bf77-158">Styling</span></span>

<span data-ttu-id="0bf77-159">Os modelos podem ser estilizados normalmente por meio de CSS, pois eles são renderizados fora do dom de sombra.</span><span class="sxs-lookup"><span data-stu-id="0bf77-159">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
