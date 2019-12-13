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
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="a3fa5-103">Modelos no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="a3fa5-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="a3fa5-104">Use modelos personalizados para modificar o conteúdo de um componente.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="a3fa5-105">Todos os componentes Web oferecem suporte a `<template>` modelos baseados no elemento.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="a3fa5-106">Por exemplo, para substituir o modelo de um componente, adicione um `<template>` elemento dentro de um componente.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

## <a name="data-type"></a><span data-ttu-id="a3fa5-107">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="a3fa5-107">Data-type</span></span>

<span data-ttu-id="a3fa5-108">Cada componente pode ter várias partes que podem ser modeladas.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-108">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="a3fa5-109">Por exemplo, no `mgt-agenda` componente, você pode modelar eventos individuais, cabeçalhos de seção individuais, modo de exibição de carregamento, sem exibição de dados e muito mais.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-109">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="a3fa5-110">Para indicar o modelo, use o `data-type` atributo em um modelo.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-110">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="a3fa5-111">Por exemplo, para modelar cada evento `mgt-agenda`no, use `event` o tipo de dados, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-111">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="a3fa5-112">Se não `data-type` for especificado, o componente inteiro será substituído pelo modelo.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-112">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="a3fa5-113">Você também pode usar `data-type="default"` para o mesmo objetivo.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-113">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="a3fa5-114">Dados de vinculação</span><span class="sxs-lookup"><span data-stu-id="a3fa5-114">Binding data</span></span>

<span data-ttu-id="a3fa5-115">Muitos modelos permitem a associação de dados que são passados para o modelo como contexto de dados.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-115">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="a3fa5-116">Por exemplo, o `event` modelo no `mgt-agenda` componente passa um `{event}` objeto que pode ser usado diretamente no modelo.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-116">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="a3fa5-117">Para expandir uma expressão, como `event.subject`, use as chaves duplas.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-117">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="a3fa5-118">Este formato também pode ser usado dentro de atributos:</span><span class="sxs-lookup"><span data-stu-id="a3fa5-118">This format can also be used inside of attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="a3fa5-119">**Observação:** Você também pode expandir objetos como `{{event}}` e eles serão renderizados como cadeias de caracteres JSON.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-119">**Note:** You can also expand objects such as `{{event}}` and they will render as JSON strings.</span></span> <span data-ttu-id="a3fa5-120">Isso pode ser útil quando você está desenvolvendo os modelos.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-120">This can be useful when you're developing the templates.</span></span>

## <a name="data-context-helper-properties"></a><span data-ttu-id="a3fa5-121">Propriedades do auxiliar de contexto de dados</span><span class="sxs-lookup"><span data-stu-id="a3fa5-121">Data context helper properties</span></span>

<span data-ttu-id="a3fa5-122">As propriedades a seguir também podem ser usadas com o objeto de contexto de dados em seus modelos.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-122">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="a3fa5-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3fa5-123">Property</span></span> |  <span data-ttu-id="a3fa5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3fa5-124">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="a3fa5-125">$index</span><span class="sxs-lookup"><span data-stu-id="a3fa5-125">$index</span></span> | <span data-ttu-id="a3fa5-126">Índice numérico do item que está sendo processado durante o loop `data-for`.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-126">Numerical index of item being rendered while being looped with `data-for`.</span></span> |
| <span data-ttu-id="a3fa5-127">$parent</span><span class="sxs-lookup"><span data-stu-id="a3fa5-127">$parent</span></span> | <span data-ttu-id="a3fa5-128">Se um modelo é renderizado dentro de outro modelo, essa propriedade permite que você acesse o contexto de dados pai.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-128">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="a3fa5-129">O exemplo a seguir mostra como usar a `$index` Propriedade em um loop data-para.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-129">The following example shows how to use the `$index` property in a data-for loop.</span></span>

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

## <a name="conditional-rendering"></a><span data-ttu-id="a3fa5-130">Renderização condicional</span><span class="sxs-lookup"><span data-stu-id="a3fa5-130">Conditional rendering</span></span>

<span data-ttu-id="a3fa5-131">Você só pode querer renderizar elementos quando uma condição for true ou false com base no contexto de dados.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-131">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="a3fa5-132">Os `data-if` atributos `data-else` e podem avaliar uma expressão e renderizar somente se true ou false.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-132">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="a3fa5-133">Loop</span><span class="sxs-lookup"><span data-stu-id="a3fa5-133">Looping</span></span>

<span data-ttu-id="a3fa5-134">Haverá casos em que o objeto de contexto de dados contém loop e você precisará fazer um loop sobre os dados.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-134">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="a3fa5-135">Neste cenário, use o `data-for` atributo.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-135">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="converters"></a><span data-ttu-id="a3fa5-136">Conversores</span><span class="sxs-lookup"><span data-stu-id="a3fa5-136">Converters</span></span>

<span data-ttu-id="a3fa5-137">Em muitos casos, talvez você queira transformar os dados antes de apresentá-los no modelo.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-137">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="a3fa5-138">Por exemplo, você pode querer formatar corretamente uma data antes de ela ser renderizada.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-138">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="a3fa5-139">Nesses casos, talvez você queira usar um conversor de modelos.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-139">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="a3fa5-140">Para usar um conversor de modelos, primeiro é necessário definir uma função que fará a conversão.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-140">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="a3fa5-141">Por exemplo, você pode definir uma função para formatar uma data.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-141">For example, you might define a function to format a date.</span></span>

```ts
getTimeRange(event) {
  // TODO: format a string from the event object as you wish
  // timeRange = ...

  return timeRange;
}
```

<span data-ttu-id="a3fa5-142">Em seguida, defina um novo conversor no elemento e nomeie-o conforme você vir ajustar.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-142">Then define a new converter on the element and name it as you see fit.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.templateConverters["myConverter"] = getTimeRange;
```

<span data-ttu-id="a3fa5-143">Para usar o conversor no seu modelo, use as chaves triplas.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-143">To use the converter in your template, use the triple curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{{ myConverter(event) }}}</div>
</template>
```

<span data-ttu-id="a3fa5-144">Você também pode usar funções internas sem definir o conversor de modelos.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-144">You can also use built-in functions without defining template converter.</span></span>

```html
<template data-type="event">
  <div>{{{ event.subject.toUpperCase() }}}</div>
</template>
```

## <a name="template-rendered-event"></a><span data-ttu-id="a3fa5-145">Evento de modelo renderizado</span><span class="sxs-lookup"><span data-stu-id="a3fa5-145">Template Rendered Event</span></span>

<span data-ttu-id="a3fa5-146">Em certos casos, talvez você queira obter uma referência para o elemento renderizado.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-146">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="a3fa5-147">Isso pode ser útil para adicionar ouvintes de eventos a elementos no modelo.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-147">This can be useful for adding event listeners to elements in the template.</span></span> <span data-ttu-id="a3fa5-148">Neste cenário, você pode usar o `templateRendered` evento.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-148">In this scenario, you might use the `templateRendered` event.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="a3fa5-149">Os detalhes do evento conterão a referência ao elemento que está sendo renderizado, o objeto de contexto de dados e o tipo de modelo.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-149">The event details will contain reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

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

## <a name="styling"></a><span data-ttu-id="a3fa5-150">Estilo</span><span class="sxs-lookup"><span data-stu-id="a3fa5-150">Styling</span></span>

<span data-ttu-id="a3fa5-151">Os modelos podem ser estilizados normalmente por meio de CSS, pois eles são renderizados fora do dom de sombra.</span><span class="sxs-lookup"><span data-stu-id="a3fa5-151">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
