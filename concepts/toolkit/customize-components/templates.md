---
title: Modelos no Microsoft Graph Toolkit
description: Use modelos personalizados para modificar o conteúdo de um componente.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 94529f45c95dcfdd56ade2dffc7b4ac7bf48babb
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658587"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="fdc57-103">Modelos no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="fdc57-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="fdc57-104">A maioria dos componentes do kit de ferramentas do Microsoft Graph oferece suporte ao uso de modelos personalizados para modificar o conteúdo de um componente.</span><span class="sxs-lookup"><span data-stu-id="fdc57-104">Most Microsoft Graph Toolkit components support the use of custom templates to modify the content of a component.</span></span>

<span data-ttu-id="fdc57-105">Todos os componentes Web oferecem suporte a modelos baseados no `<template>` elemento.</span><span class="sxs-lookup"><span data-stu-id="fdc57-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="fdc57-106">Por exemplo, para substituir o modelo de um componente, adicione um `<template>` elemento dentro de um componente.</span><span class="sxs-lookup"><span data-stu-id="fdc57-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

<span data-ttu-id="fdc57-107">Se você estiver usando os componentes de reagir do Microsoft Graph Toolkit, você poderá usar o reagir para modelos de criação.</span><span class="sxs-lookup"><span data-stu-id="fdc57-107">If you're using the Microsoft Graph Toolkit React components, you can use React for authoring templates.</span></span> <span data-ttu-id="fdc57-108">Para obter detalhes, consulte [usar o kit de ferramentas com reagir](../get-started/mgt-react.md).</span><span class="sxs-lookup"><span data-stu-id="fdc57-108">For details, see [Use the toolkit with React](../get-started/mgt-react.md).</span></span>

## <a name="data-type"></a><span data-ttu-id="fdc57-109">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="fdc57-109">Data-type</span></span>

<span data-ttu-id="fdc57-110">Cada componente pode ter várias partes que podem ser modeladas.</span><span class="sxs-lookup"><span data-stu-id="fdc57-110">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="fdc57-111">Por exemplo, no `mgt-agenda` componente, você pode modelar eventos individuais, cabeçalhos de seção individuais, modo de exibição de carregamento, sem exibição de dados e muito mais.</span><span class="sxs-lookup"><span data-stu-id="fdc57-111">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="fdc57-112">Para indicar o modelo, use o `data-type` atributo em um modelo.</span><span class="sxs-lookup"><span data-stu-id="fdc57-112">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="fdc57-113">Por exemplo, para modelar cada evento no `mgt-agenda` , use o `event` tipo de dados, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="fdc57-113">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="fdc57-114">Se não `data-type` for especificado, o componente inteiro será substituído pelo modelo.</span><span class="sxs-lookup"><span data-stu-id="fdc57-114">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="fdc57-115">Você também pode usar `data-type="default"` para o mesmo objetivo.</span><span class="sxs-lookup"><span data-stu-id="fdc57-115">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="fdc57-116">Dados de vinculação</span><span class="sxs-lookup"><span data-stu-id="fdc57-116">Binding data</span></span>

<span data-ttu-id="fdc57-117">Muitos modelos permitem a associação de dados que são passados para o modelo como contexto de dados.</span><span class="sxs-lookup"><span data-stu-id="fdc57-117">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="fdc57-118">Por exemplo, o `event` modelo no `mgt-agenda` componente passa um `{event}` objeto que pode ser usado diretamente no modelo.</span><span class="sxs-lookup"><span data-stu-id="fdc57-118">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="fdc57-119">Para expandir uma expressão, como `event.subject` , use as chaves duplas.</span><span class="sxs-lookup"><span data-stu-id="fdc57-119">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="fdc57-120">Este formato também pode ser usado dentro de atributos:</span><span class="sxs-lookup"><span data-stu-id="fdc57-120">This format can also be used inside attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="fdc57-121">**Observação:** Você também pode expandir objetos como `{{event}}` ou `{{this}}` e eles serão renderizados como cadeias de caracteres JSON.</span><span class="sxs-lookup"><span data-stu-id="fdc57-121">**Note:** You can also expand objects such as `{{event}}` or `{{this}}` and they will render as JSON strings.</span></span> <span data-ttu-id="fdc57-122">Isso pode ser útil quando você está desenvolvendo os modelos.</span><span class="sxs-lookup"><span data-stu-id="fdc57-122">This can be useful when you're developing the templates.</span></span>

### <a name="change-binding-syntax"></a><span data-ttu-id="fdc57-123">Alterar sintaxe de associação</span><span class="sxs-lookup"><span data-stu-id="fdc57-123">Change binding syntax</span></span>

<span data-ttu-id="fdc57-124">Por padrão, para expandir uma expressão, você usa chaves duplas ( `{{expression}}` ).</span><span class="sxs-lookup"><span data-stu-id="fdc57-124">By default, to expand an expression, you use double curly brackets ( `{{expression}}` ).</span></span> <span data-ttu-id="fdc57-125">No entanto, você pode alterar essa sintaxe para ambientes onde a sintaxe de chave dupla já é usada.</span><span class="sxs-lookup"><span data-stu-id="fdc57-125">However, you can change this syntax for environments where the double curly bracket syntax is already used.</span></span> <span data-ttu-id="fdc57-126">Por exemplo, o exemplo a seguir usa colchetes duplos ( `[[expression]]` ).</span><span class="sxs-lookup"><span data-stu-id="fdc57-126">For example, the following example uses double square brackets ( `[[expression]]` ).</span></span>

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a><span data-ttu-id="fdc57-127">Propriedades do auxiliar de contexto de dados</span><span class="sxs-lookup"><span data-stu-id="fdc57-127">Data context helper properties</span></span>

<span data-ttu-id="fdc57-128">As propriedades a seguir também podem ser usadas com o objeto de contexto de dados em seus modelos.</span><span class="sxs-lookup"><span data-stu-id="fdc57-128">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="fdc57-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdc57-129">Property</span></span> | <span data-ttu-id="fdc57-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdc57-130">Description</span></span>                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fdc57-131">$index</span><span class="sxs-lookup"><span data-stu-id="fdc57-131">$index</span></span>   | <span data-ttu-id="fdc57-132">Índice numérico do item que está sendo processado durante o loop `data-for` .</span><span class="sxs-lookup"><span data-stu-id="fdc57-132">Numerical index of item being rendered while being looped with `data-for`.</span></span>                                     |
| <span data-ttu-id="fdc57-133">$parent</span><span class="sxs-lookup"><span data-stu-id="fdc57-133">$parent</span></span>  | <span data-ttu-id="fdc57-134">Se um modelo é renderizado dentro de outro modelo, essa propriedade permite que você acesse o contexto de dados pai.</span><span class="sxs-lookup"><span data-stu-id="fdc57-134">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="fdc57-135">O exemplo a seguir mostra como usar a `$index` propriedade em um loop data-para.</span><span class="sxs-lookup"><span data-stu-id="fdc57-135">The following example shows how to use the `$index` property in a data-for loop.</span></span>

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

## <a name="conditional-rendering"></a><span data-ttu-id="fdc57-136">Renderização condicional</span><span class="sxs-lookup"><span data-stu-id="fdc57-136">Conditional rendering</span></span>

<span data-ttu-id="fdc57-137">Você só pode querer renderizar elementos quando uma condição for true ou false com base no contexto de dados.</span><span class="sxs-lookup"><span data-stu-id="fdc57-137">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="fdc57-138">Os `data-if` `data-else` atributos e podem avaliar uma expressão e renderizar somente se true ou false.</span><span class="sxs-lookup"><span data-stu-id="fdc57-138">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="fdc57-139">Loop</span><span class="sxs-lookup"><span data-stu-id="fdc57-139">Looping</span></span>

<span data-ttu-id="fdc57-140">Haverá casos em que o objeto de contexto de dados contém loop e você precisará fazer um loop sobre os dados.</span><span class="sxs-lookup"><span data-stu-id="fdc57-140">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="fdc57-141">Neste cenário, use o `data-for` atributo.</span><span class="sxs-lookup"><span data-stu-id="fdc57-141">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="template-context"></a><span data-ttu-id="fdc57-142">Contexto de modelo</span><span class="sxs-lookup"><span data-stu-id="fdc57-142">Template context</span></span>

<span data-ttu-id="fdc57-143">Em cenários em que você precisa converter dados em suas associações, vincular a eventos ou apenas usar dados externos em associações de modelos, os modelos dão suporte à associação a contexto de dados externos.</span><span class="sxs-lookup"><span data-stu-id="fdc57-143">In scenarios where you need to convert data in your bindings, bind to events, or just use external data in your templates bindings, the templates support binding to external data context.</span></span> <span data-ttu-id="fdc57-144">Você pode adicionar contexto de modelo adicional de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="fdc57-144">You can add additional template context in two ways:</span></span>

1. <span data-ttu-id="fdc57-145">Diretamente no componente.</span><span class="sxs-lookup"><span data-stu-id="fdc57-145">Directly on the component.</span></span>

    <span data-ttu-id="fdc57-146">Cada componente define a `templateContext` propriedade, que você pode usar para passar dados adicionais para qualquer modelo no componente.</span><span class="sxs-lookup"><span data-stu-id="fdc57-146">Each component defines the `templateContext` property, which you can use to pass additional data to any template in the component.</span></span>

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    <span data-ttu-id="fdc57-147">Agora, as propriedades no `templateContext` objeto estarão disponíveis para serem usadas nas expressões de associação no modelo.</span><span class="sxs-lookup"><span data-stu-id="fdc57-147">The properties in the `templateContext` object will now be available to be used in the binding expressions in the template.</span></span>

2. <span data-ttu-id="fdc57-148">Globalmente para todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="fdc57-148">Globally for all components.</span></span>

    <span data-ttu-id="fdc57-149">A `TemplateHelper` classe expõe o `globalContext` objeto para adicionar dados ou funções que devem estar disponíveis globalmente para todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="fdc57-149">The `TemplateHelper` class exposes the `globalContext` object to add data or functions that should be globally available for all components.</span></span>

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a><span data-ttu-id="fdc57-150">Conversores</span><span class="sxs-lookup"><span data-stu-id="fdc57-150">Converters</span></span>

<span data-ttu-id="fdc57-151">Em muitos casos, talvez você queira transformar os dados antes de apresentá-los no modelo.</span><span class="sxs-lookup"><span data-stu-id="fdc57-151">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="fdc57-152">Por exemplo, você pode querer formatar corretamente uma data antes de ela ser renderizada.</span><span class="sxs-lookup"><span data-stu-id="fdc57-152">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="fdc57-153">Nesses casos, talvez você queira usar um conversor de modelos.</span><span class="sxs-lookup"><span data-stu-id="fdc57-153">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="fdc57-154">Para usar um conversor de modelos, primeiro é necessário definir uma função que fará a conversão.</span><span class="sxs-lookup"><span data-stu-id="fdc57-154">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="fdc57-155">Por exemplo, você pode definir uma função para converter um objeto de evento em um intervalo de tempo formatado.</span><span class="sxs-lookup"><span data-stu-id="fdc57-155">For example, you might define a function to convert an event object to a formatted time range.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

<span data-ttu-id="fdc57-156">Para usar o conversor no seu modelo, use-o como se você tivesse usado uma função no code-behind.</span><span class="sxs-lookup"><span data-stu-id="fdc57-156">To use the converter in your template, use it as if you would use a function in code behind.</span></span>

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a><span data-ttu-id="fdc57-157">Associação de evento ou propriedade</span><span class="sxs-lookup"><span data-stu-id="fdc57-157">Event or property binding</span></span>

<span data-ttu-id="fdc57-158">O `data-props` atributo permite adicionar um ouvinte de eventos ou definir um valor de propriedade diretamente em seus modelos.</span><span class="sxs-lookup"><span data-stu-id="fdc57-158">The `data-props` attribute allows you to add an event listener or set a property value directly in your templates.</span></span>

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

<span data-ttu-id="fdc57-159">Os dados-props aceitam uma cadeia de caracteres delimitada por vírgulas para cada propriedade ou manipulador de eventos que você queira definir.</span><span class="sxs-lookup"><span data-stu-id="fdc57-159">The data-props accepts a comma delimited string for each property or event handler you might want to set.</span></span>

<span data-ttu-id="fdc57-160">Para adicionar um manipulador de eventos, Prefixe o nome do evento com `@` .</span><span class="sxs-lookup"><span data-stu-id="fdc57-160">To add an event handler, prefix the name of the event with `@`.</span></span> <span data-ttu-id="fdc57-161">O manipulador de eventos deverá estar disponível no `templateContext` do elemento.</span><span class="sxs-lookup"><span data-stu-id="fdc57-161">The event handler will need to be available in the `templateContext` of the element.</span></span>

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

<span data-ttu-id="fdc57-162">Os argumentos de evento, o contexto de dados e o elemento raiz do modelo são passados para o manipulador de eventos como parâmetros.</span><span class="sxs-lookup"><span data-stu-id="fdc57-162">The event args, data context, and the root element of the template are passed to the event handler as parameters.</span></span>


## <a name="template-rendered-event"></a><span data-ttu-id="fdc57-163">Evento de modelo renderizado</span><span class="sxs-lookup"><span data-stu-id="fdc57-163">Template rendered event</span></span>

<span data-ttu-id="fdc57-164">Em certos casos, talvez você queira obter uma referência para o elemento renderizado.</span><span class="sxs-lookup"><span data-stu-id="fdc57-164">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="fdc57-165">Isso pode ser útil se você quiser manipular a renderização do conteúdo sozinho ou se quiser modificar o elemento renderizado.</span><span class="sxs-lookup"><span data-stu-id="fdc57-165">This can be useful if you want to handle the rendering of the content yourself, or you want to modify the rendered element.</span></span>

<span data-ttu-id="fdc57-166">Neste cenário, você pode usar o `templateRendered` evento, que é acionado depois que o modelo é renderizado.</span><span class="sxs-lookup"><span data-stu-id="fdc57-166">In this scenario, you can use the `templateRendered` event, which fires after the template has been rendered.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="fdc57-167">Os detalhes do evento conterão uma referência ao elemento que está sendo renderizado, o objeto de contexto de dados e o tipo de modelo.</span><span class="sxs-lookup"><span data-stu-id="fdc57-167">The event details will contain a reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

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

## <a name="styling"></a><span data-ttu-id="fdc57-168">Estilo</span><span class="sxs-lookup"><span data-stu-id="fdc57-168">Styling</span></span>

<span data-ttu-id="fdc57-169">Os modelos podem ser estilizados normalmente por meio de CSS, pois eles são renderizados fora do dom de sombra.</span><span class="sxs-lookup"><span data-stu-id="fdc57-169">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
