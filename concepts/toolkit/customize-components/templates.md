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
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="8fe93-103">Modelos no microsoft graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="8fe93-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8fe93-104">A maioria dos Toolkit do Microsoft Graph suporta o uso de modelos personalizados para modificar o conteúdo de um componente.</span><span class="sxs-lookup"><span data-stu-id="8fe93-104">Most Microsoft Graph Toolkit components support the use of custom templates to modify the content of a component.</span></span>

<span data-ttu-id="8fe93-105">Todos os componentes da Web suportam modelos com base no `<template>` elemento.</span><span class="sxs-lookup"><span data-stu-id="8fe93-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="8fe93-106">Por exemplo, para substituir o modelo de um componente, adicione um `<template>` elemento dentro de um componente.</span><span class="sxs-lookup"><span data-stu-id="8fe93-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

<span data-ttu-id="8fe93-107">Se você estiver usando os componentes do Microsoft Graph Toolkit React, poderá usar o React para modelos de autoria.</span><span class="sxs-lookup"><span data-stu-id="8fe93-107">If you're using the Microsoft Graph Toolkit React components, you can use React for authoring templates.</span></span> <span data-ttu-id="8fe93-108">Para obter detalhes, [consulte Use the toolkit with React](../get-started/mgt-react.md).</span><span class="sxs-lookup"><span data-stu-id="8fe93-108">For details, see [Use the toolkit with React](../get-started/mgt-react.md).</span></span>

## <a name="data-type"></a><span data-ttu-id="8fe93-109">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="8fe93-109">Data-type</span></span>

<span data-ttu-id="8fe93-110">Cada componente pode ter várias partes que podem ser modelos.</span><span class="sxs-lookup"><span data-stu-id="8fe93-110">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="8fe93-111">Por exemplo, no componente, você pode modelo eventos individuais, headers de seção `mgt-agenda` individuais, exibição de carregamento, sem exibição de dados e muito mais.</span><span class="sxs-lookup"><span data-stu-id="8fe93-111">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="8fe93-112">Para indicar o modelo, use o `data-type` atributo em um modelo.</span><span class="sxs-lookup"><span data-stu-id="8fe93-112">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="8fe93-113">Por exemplo, para modelo de cada evento no `mgt-agenda` , use o tipo de `event` dados, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="8fe93-113">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="8fe93-114">Se não `data-type` for especificado, todo o componente será substituído pelo modelo.</span><span class="sxs-lookup"><span data-stu-id="8fe93-114">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="8fe93-115">Você também pode `data-type="default"` usar para a mesma finalidade.</span><span class="sxs-lookup"><span data-stu-id="8fe93-115">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="8fe93-116">Dados de associação</span><span class="sxs-lookup"><span data-stu-id="8fe93-116">Binding data</span></span>

<span data-ttu-id="8fe93-117">Muitos modelos permitem a associação de dados que são passados para o modelo como contexto de dados.</span><span class="sxs-lookup"><span data-stu-id="8fe93-117">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="8fe93-118">Por exemplo, o `event` modelo no componente passa um objeto que pode ser usado diretamente no `mgt-agenda` `{event}` modelo.</span><span class="sxs-lookup"><span data-stu-id="8fe93-118">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="8fe93-119">Para expandir uma expressão, como `event.subject` , use os colchetes curvados duplos.</span><span class="sxs-lookup"><span data-stu-id="8fe93-119">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="8fe93-120">Esse formato também pode ser usado dentro de atributos:</span><span class="sxs-lookup"><span data-stu-id="8fe93-120">This format can also be used inside attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="8fe93-121">**Observação:** Você também pode expandir objetos como `{{event}}` ou `{{this}}` e eles renderizarão como cadeias de caracteres JSON.</span><span class="sxs-lookup"><span data-stu-id="8fe93-121">**Note:** You can also expand objects such as `{{event}}` or `{{this}}` and they will render as JSON strings.</span></span> <span data-ttu-id="8fe93-122">Isso pode ser útil quando você estiver desenvolvendo os modelos.</span><span class="sxs-lookup"><span data-stu-id="8fe93-122">This can be useful when you're developing the templates.</span></span>

### <a name="change-binding-syntax"></a><span data-ttu-id="8fe93-123">Alterar sintaxe de associação</span><span class="sxs-lookup"><span data-stu-id="8fe93-123">Change binding syntax</span></span>

<span data-ttu-id="8fe93-124">Por padrão, para expandir uma expressão, você usa colchetes curvados duplos ( `{{expression}}` ).</span><span class="sxs-lookup"><span data-stu-id="8fe93-124">By default, to expand an expression, you use double curly brackets ( `{{expression}}` ).</span></span> <span data-ttu-id="8fe93-125">No entanto, você pode alterar essa sintaxe para ambientes em que a sintaxe de colchete dupla curva já é usada.</span><span class="sxs-lookup"><span data-stu-id="8fe93-125">However, you can change this syntax for environments where the double curly bracket syntax is already used.</span></span> <span data-ttu-id="8fe93-126">Por exemplo, o exemplo a seguir usa colchetes duplos ( `[[expression]]` ).</span><span class="sxs-lookup"><span data-stu-id="8fe93-126">For example, the following example uses double square brackets ( `[[expression]]` ).</span></span>

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a><span data-ttu-id="8fe93-127">Propriedades auxiliares de contexto de dados</span><span class="sxs-lookup"><span data-stu-id="8fe93-127">Data context helper properties</span></span>

<span data-ttu-id="8fe93-128">As propriedades a seguir também podem ser usadas com o objeto de contexto de dados em seus modelos.</span><span class="sxs-lookup"><span data-stu-id="8fe93-128">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="8fe93-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fe93-129">Property</span></span> | <span data-ttu-id="8fe93-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fe93-130">Description</span></span>                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8fe93-131">$index</span><span class="sxs-lookup"><span data-stu-id="8fe93-131">$index</span></span>   | <span data-ttu-id="8fe93-132">Índice numérico do item que está sendo renderizado durante o loop com `data-for` .</span><span class="sxs-lookup"><span data-stu-id="8fe93-132">Numerical index of item being rendered while being looped with `data-for`.</span></span>                                     |
| <span data-ttu-id="8fe93-133">$parent</span><span class="sxs-lookup"><span data-stu-id="8fe93-133">$parent</span></span>  | <span data-ttu-id="8fe93-134">Se um modelo for renderizado dentro de outro modelo, essa propriedade permitirá que você acesse o contexto de dados pai.</span><span class="sxs-lookup"><span data-stu-id="8fe93-134">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="8fe93-135">O exemplo a seguir mostra como usar `$index` a propriedade em um loop data-for.</span><span class="sxs-lookup"><span data-stu-id="8fe93-135">The following example shows how to use the `$index` property in a data-for loop.</span></span>

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

### <a name="this"></a><span data-ttu-id="8fe93-136">{{this}}</span><span class="sxs-lookup"><span data-stu-id="8fe93-136">{{this}}</span></span>

<span data-ttu-id="8fe93-137">Para ajudar a depurar o contexto de dados, você pode usar `this` em suas expressões de associação.</span><span class="sxs-lookup"><span data-stu-id="8fe93-137">To help debug the data context, you can use `this` in your binding expressions.</span></span> <span data-ttu-id="8fe93-138">O formulário mais simples é adicionar em `{{this}}` qualquer lugar do seu modelo.</span><span class="sxs-lookup"><span data-stu-id="8fe93-138">The simplest form is to add `{{this}}` anywhere in your template.</span></span>

```html
<template data-type="event">
  <div>
    {{this}}
  </div>
</template>
```

<span data-ttu-id="8fe93-139">Como você pode usar JavaScript em suas expressões de associação, você também tem acesso ao objeto que permite que você use (ou qualquer outra [`console`](https://developer.mozilla.org/docs/Web/API/Console) `console.log(this)` `console` API) em seus modelos.</span><span class="sxs-lookup"><span data-stu-id="8fe93-139">Because you can use JavaScript in your binding expressions, you also have access to the [`console`](https://developer.mozilla.org/docs/Web/API/Console) object which allows you to use `console.log(this)` (or any other `console` API) in your templates.</span></span>

```html
<template data-type="event">
  <div>
    {{console.log(this)}}
  </div>
</template>
```

## <a name="conditional-rendering"></a><span data-ttu-id="8fe93-140">Renderização condicional</span><span class="sxs-lookup"><span data-stu-id="8fe93-140">Conditional rendering</span></span>

<span data-ttu-id="8fe93-141">Você só pode querer renderizar elementos quando uma condição for verdadeira ou false com base no contexto de dados.</span><span class="sxs-lookup"><span data-stu-id="8fe93-141">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="8fe93-142">Os `data-if` atributos e podem avaliar uma expressão e `data-else` renderizar somente se for verdadeiro ou falso.</span><span class="sxs-lookup"><span data-stu-id="8fe93-142">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="8fe93-143">Looping</span><span class="sxs-lookup"><span data-stu-id="8fe93-143">Looping</span></span>

<span data-ttu-id="8fe93-144">Haverá casos em que o objeto de contexto de dados contém loop e você precisará fazer um loop sobre os dados.</span><span class="sxs-lookup"><span data-stu-id="8fe93-144">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="8fe93-145">Para esse cenário, use o `data-for` atributo.</span><span class="sxs-lookup"><span data-stu-id="8fe93-145">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="template-context"></a><span data-ttu-id="8fe93-146">Contexto do modelo</span><span class="sxs-lookup"><span data-stu-id="8fe93-146">Template context</span></span>

<span data-ttu-id="8fe93-147">Em cenários em que você precisa converter dados em suas vinculações, vincular a eventos ou apenas usar dados externos em suas vinculações de modelos, os modelos suportam a associação ao contexto de dados externos.</span><span class="sxs-lookup"><span data-stu-id="8fe93-147">In scenarios where you need to convert data in your bindings, bind to events, or just use external data in your templates bindings, the templates support binding to external data context.</span></span> <span data-ttu-id="8fe93-148">Você pode adicionar contexto de modelo adicional de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="8fe93-148">You can add additional template context in two ways:</span></span>

1. <span data-ttu-id="8fe93-149">Diretamente no componente.</span><span class="sxs-lookup"><span data-stu-id="8fe93-149">Directly on the component.</span></span>

    <span data-ttu-id="8fe93-150">Cada componente define a `templateContext` propriedade, que você pode usar para passar dados adicionais para qualquer modelo no componente.</span><span class="sxs-lookup"><span data-stu-id="8fe93-150">Each component defines the `templateContext` property, which you can use to pass additional data to any template in the component.</span></span>

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    <span data-ttu-id="8fe93-151">As propriedades no objeto agora estarão disponíveis para serem `templateContext` usadas nas expressões de associação no modelo.</span><span class="sxs-lookup"><span data-stu-id="8fe93-151">The properties in the `templateContext` object will now be available to be used in the binding expressions in the template.</span></span>

2. <span data-ttu-id="8fe93-152">Globalmente para todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="8fe93-152">Globally for all components.</span></span>

    <span data-ttu-id="8fe93-153">A classe expõe o objeto para adicionar dados ou funções que `TemplateHelper` `globalContext` devem estar disponíveis globalmente para todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="8fe93-153">The `TemplateHelper` class exposes the `globalContext` object to add data or functions that should be globally available for all components.</span></span>

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a><span data-ttu-id="8fe93-154">Conversores</span><span class="sxs-lookup"><span data-stu-id="8fe93-154">Converters</span></span>

<span data-ttu-id="8fe93-155">Em muitos casos, talvez você queira transformar os dados antes de apresentá-los no modelo.</span><span class="sxs-lookup"><span data-stu-id="8fe93-155">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="8fe93-156">Por exemplo, talvez você queira formatar corretamente uma data antes de ser renderizada.</span><span class="sxs-lookup"><span data-stu-id="8fe93-156">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="8fe93-157">Nesses casos, talvez você queira usar um conversor de modelo.</span><span class="sxs-lookup"><span data-stu-id="8fe93-157">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="8fe93-158">Para usar um conversor de modelo, primeiro você precisa definir uma função que fará a conversão.</span><span class="sxs-lookup"><span data-stu-id="8fe93-158">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="8fe93-159">Por exemplo, você pode definir uma função para converter um objeto de evento em um intervalo de tempo formatado.</span><span class="sxs-lookup"><span data-stu-id="8fe93-159">For example, you might define a function to convert an event object to a formatted time range.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

<span data-ttu-id="8fe93-160">Para usar o conversor em seu modelo, use-o como se você usaria uma função em code behind.</span><span class="sxs-lookup"><span data-stu-id="8fe93-160">To use the converter in your template, use it as if you would use a function in code behind.</span></span>

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a><span data-ttu-id="8fe93-161">Associação de eventos ou propriedades</span><span class="sxs-lookup"><span data-stu-id="8fe93-161">Event or property binding</span></span>

<span data-ttu-id="8fe93-162">O atributo permite adicionar um ouvinte de eventos ou definir um valor `data-props` de propriedade diretamente em seus modelos.</span><span class="sxs-lookup"><span data-stu-id="8fe93-162">The `data-props` attribute allows you to add an event listener or set a property value directly in your templates.</span></span>

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

<span data-ttu-id="8fe93-163">Os data-props aceitam uma cadeia de caracteres delimitada por vírgula para cada propriedade ou manipulador de eventos que você talvez queira definir.</span><span class="sxs-lookup"><span data-stu-id="8fe93-163">The data-props accepts a comma delimited string for each property or event handler you might want to set.</span></span>

<span data-ttu-id="8fe93-164">Para adicionar um manipulador de eventos, prefixe o nome do evento com `@` .</span><span class="sxs-lookup"><span data-stu-id="8fe93-164">To add an event handler, prefix the name of the event with `@`.</span></span> <span data-ttu-id="8fe93-165">O manipulador de eventos precisará estar disponível no `templateContext` elemento.</span><span class="sxs-lookup"><span data-stu-id="8fe93-165">The event handler will need to be available in the `templateContext` of the element.</span></span>

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

<span data-ttu-id="8fe93-166">Os args de evento, o contexto de dados e o elemento raiz do modelo são passados para o manipulador de eventos como parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8fe93-166">The event args, data context, and the root element of the template are passed to the event handler as parameters.</span></span>


## <a name="template-rendered-event"></a><span data-ttu-id="8fe93-167">Evento renderizado de modelo</span><span class="sxs-lookup"><span data-stu-id="8fe93-167">Template rendered event</span></span>

<span data-ttu-id="8fe93-168">Em determinados casos, talvez você queira obter uma referência ao elemento renderizado.</span><span class="sxs-lookup"><span data-stu-id="8fe93-168">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="8fe93-169">Isso pode ser útil se você quiser manipular a renderização do conteúdo por conta própria ou se quiser modificar o elemento renderizado.</span><span class="sxs-lookup"><span data-stu-id="8fe93-169">This can be useful if you want to handle the rendering of the content yourself, or you want to modify the rendered element.</span></span>

<span data-ttu-id="8fe93-170">Nesse cenário, você pode usar o `templateRendered` evento, que é a disparar depois que o modelo é renderizado.</span><span class="sxs-lookup"><span data-stu-id="8fe93-170">In this scenario, you can use the `templateRendered` event, which fires after the template has been rendered.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="8fe93-171">Os detalhes do evento conterão uma referência ao elemento que está sendo renderizado, ao objeto de contexto de dados e ao tipo do modelo.</span><span class="sxs-lookup"><span data-stu-id="8fe93-171">The event details will contain a reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

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

## <a name="styling"></a><span data-ttu-id="8fe93-172">Estilo</span><span class="sxs-lookup"><span data-stu-id="8fe93-172">Styling</span></span>

<span data-ttu-id="8fe93-173">Os modelos podem ser estilizados normalmente via CSS à medida que são renderizados fora do dom de sombra.</span><span class="sxs-lookup"><span data-stu-id="8fe93-173">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
