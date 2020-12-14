---
title: Componente Person no Microsoft Graph Toolkit
description: O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: cfe5f6b97c35c2704def8c4879522268cc8cc91e
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660036"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="1d509-103">Componente Person no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="1d509-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1d509-104">O componente pessoa é usado para exibir uma pessoa ou contato usando a foto, o nome, o endereço de email ou qualquer outro detalhe de pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d509-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="1d509-105">O componente pessoa também usa a [pessoa de gerenciamento de pessoas](./person-card.md) para exibir um cartão de submenu com informações adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="1d509-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="1d509-106">Para obter detalhes, consulte a seção [cartão de pessoa](#person-card) .</span><span class="sxs-lookup"><span data-stu-id="1d509-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="1d509-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d509-107">Example</span></span>

<span data-ttu-id="1d509-108">O exemplo a seguir exibe uma pessoa usando o `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="1d509-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="1d509-109">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="1d509-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="1d509-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="1d509-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="1d509-111">Configurando os detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="1d509-111">Setting the person details</span></span>

<span data-ttu-id="1d509-112">Você pode usar três propriedades para definir os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d509-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="1d509-113">Use apenas uma das seguintes propriedades por instância:</span><span class="sxs-lookup"><span data-stu-id="1d509-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="1d509-114">Defina o `user-id` atributo ou a `userId` propriedade para buscar o usuário do Microsoft Graph usando sua ID.</span><span class="sxs-lookup"><span data-stu-id="1d509-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="1d509-115">Definir o `person-query` atributo ou a `personQuery` propriedade para pesquisar o Microsoft Graph em uma determinada pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d509-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="1d509-116">Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d509-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="1d509-117">Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.</span><span class="sxs-lookup"><span data-stu-id="1d509-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="1d509-118">Defina o `person-presence` atributo ou a `personPresence` propriedade para adicionar um emblema de presença ao avatar manualmente.</span><span class="sxs-lookup"><span data-stu-id="1d509-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="1d509-119">Defina o `avatar-size` atributo ou a `avatarSize` propriedade como `small` ou `large` para determinar o tamanho do Avatar.</span><span class="sxs-lookup"><span data-stu-id="1d509-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="1d509-120">Isso ajuda a adicionar o [emblema de presença correto](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) ao avatar.</span><span class="sxs-lookup"><span data-stu-id="1d509-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="1d509-121">Você precisará escolher as propriedades personalizadas de CSS correspondentes indicadas abaixo para personalizar ainda mais o tamanho do Avatar.</span><span class="sxs-lookup"><span data-stu-id="1d509-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="1d509-122">Por padrão, o valor é definido como o `auto` qual decidirá automaticamente como renderizar a presença com base na `view` propriedade.</span><span class="sxs-lookup"><span data-stu-id="1d509-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="1d509-123">Recomendamos usar `small` o se o seu avatar for menor do que o medianiz 32px por medianiz 32px.</span><span class="sxs-lookup"><span data-stu-id="1d509-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="1d509-124">Use o `person-details` atributo ou `personDetails` propriedade para definir manualmente os detalhes da pessoa, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="1d509-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="1d509-125">Se nenhuma imagem for fornecida, uma será buscada (se disponível).</span><span class="sxs-lookup"><span data-stu-id="1d509-125">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="1d509-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d509-126">Properties</span></span>

<span data-ttu-id="1d509-127">Você pode usar várias propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="1d509-127">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="1d509-128">Atributo</span><span class="sxs-lookup"><span data-stu-id="1d509-128">Attribute</span></span>       | <span data-ttu-id="1d509-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d509-129">Property</span></span>       | <span data-ttu-id="1d509-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d509-130">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="1d509-131">ID de usuário</span><span class="sxs-lookup"><span data-stu-id="1d509-131">user-id</span></span>         | <span data-ttu-id="1d509-132">userId</span><span class="sxs-lookup"><span data-stu-id="1d509-132">userId</span></span>         | <span data-ttu-id="1d509-133">Defina como uma ID de usuário para buscar os detalhes e a imagem do usuário do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d509-133">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="1d509-134">pessoa – consulta</span><span class="sxs-lookup"><span data-stu-id="1d509-134">person-query</span></span>    | <span data-ttu-id="1d509-135">personQuery</span><span class="sxs-lookup"><span data-stu-id="1d509-135">personQuery</span></span>    | <span data-ttu-id="1d509-136">Defina como um nome ou email de uma pessoa para pesquisar uma pessoa no Microsoft Graph e busque os detalhes e a imagem da primeira pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d509-136">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="1d509-137">pessoa-detalhes</span><span class="sxs-lookup"><span data-stu-id="1d509-137">person-details</span></span>  | <span data-ttu-id="1d509-138">personDetails</span><span class="sxs-lookup"><span data-stu-id="1d509-138">personDetails</span></span>  | <span data-ttu-id="1d509-139">Defina como um objeto que represente uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d509-139">Set to an object representing a person.</span></span> <span data-ttu-id="1d509-140">Funciona com o objeto dos recursos pessoas, usuários, contatos ou grupos.</span><span class="sxs-lookup"><span data-stu-id="1d509-140">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="1d509-141">pessoa-imagem</span><span class="sxs-lookup"><span data-stu-id="1d509-141">person-image</span></span>    | <span data-ttu-id="1d509-142">personImage</span><span class="sxs-lookup"><span data-stu-id="1d509-142">personImage</span></span>    | <span data-ttu-id="1d509-143">Defina a imagem a ser mostrada para a pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d509-143">Set the image to show for the person.</span></span> |
| <span data-ttu-id="1d509-144">presença de pessoa</span><span class="sxs-lookup"><span data-stu-id="1d509-144">person-presence</span></span> | <span data-ttu-id="1d509-145">personPresence</span><span class="sxs-lookup"><span data-stu-id="1d509-145">personPresence</span></span> | <span data-ttu-id="1d509-146">Definir a presença para a pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d509-146">Set the presence for the person.</span></span> |
| <span data-ttu-id="1d509-147">FETCH-Image</span><span class="sxs-lookup"><span data-stu-id="1d509-147">fetch-image</span></span>     | <span data-ttu-id="1d509-148">fetchImage</span><span class="sxs-lookup"><span data-stu-id="1d509-148">fetchImage</span></span>     | <span data-ttu-id="1d509-149">Defina o sinalizador para buscar `personImage` automaticamente a partir do Microsoft Graph com base no `personDetails` objeto fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1d509-149">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="1d509-150">modo de exibição</span><span class="sxs-lookup"><span data-stu-id="1d509-150">view</span></span>            | <span data-ttu-id="1d509-151">modo de exibição</span><span class="sxs-lookup"><span data-stu-id="1d509-151">view</span></span>           | <span data-ttu-id="1d509-152">Definido para controlar como a pessoa é renderizada.</span><span class="sxs-lookup"><span data-stu-id="1d509-152">Set to control how the person is rendered.</span></span> <span data-ttu-id="1d509-153">O padrão é `avatar`</span><span class="sxs-lookup"><span data-stu-id="1d509-153">Default is `avatar`</span></span> <br /> <span data-ttu-id="1d509-154">`avatar` -Mostrar somente avatar</span><span class="sxs-lookup"><span data-stu-id="1d509-154">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="1d509-155">`oneline` -Mostrar avatar e primeira linha ( `displayName` por padrão)</span><span class="sxs-lookup"><span data-stu-id="1d509-155">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="1d509-156">`twolines` -Mostrar avatar e duas linhas de texto ( `displayName` e `mail` por padrão)</span><span class="sxs-lookup"><span data-stu-id="1d509-156">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="1d509-157">linha1-Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d509-157">line1-property</span></span>  | <span data-ttu-id="1d509-158">line1Property</span><span class="sxs-lookup"><span data-stu-id="1d509-158">line1Property</span></span>  | <span data-ttu-id="1d509-159">Define a propriedade do personDetails a ser usado para a primeira linha do texto.</span><span class="sxs-lookup"><span data-stu-id="1d509-159">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="1d509-160">O padrão é `displayName`.</span><span class="sxs-lookup"><span data-stu-id="1d509-160">Default is `displayName`.</span></span>|
| <span data-ttu-id="1d509-161">Linha2-Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d509-161">line2-property</span></span>  | <span data-ttu-id="1d509-162">line2Property</span><span class="sxs-lookup"><span data-stu-id="1d509-162">line2Property</span></span>  | <span data-ttu-id="1d509-163">Define a propriedade do personDetails a ser usado para a segunda linha de texto.</span><span class="sxs-lookup"><span data-stu-id="1d509-163">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="1d509-164">O padrão é `mail`.</span><span class="sxs-lookup"><span data-stu-id="1d509-164">Default is `mail`.</span></span>|
| <span data-ttu-id="1d509-165">Line3-Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d509-165">line3-property</span></span>  | <span data-ttu-id="1d509-166">line3Property</span><span class="sxs-lookup"><span data-stu-id="1d509-166">line3Property</span></span>  | <span data-ttu-id="1d509-167">Define a propriedade do personDetails a ser usada para a terceira linha de texto.</span><span class="sxs-lookup"><span data-stu-id="1d509-167">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="1d509-168">O padrão é `jobTitle`.</span><span class="sxs-lookup"><span data-stu-id="1d509-168">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="1d509-169">show-Presence</span><span class="sxs-lookup"><span data-stu-id="1d509-169">show-presence</span></span>   | <span data-ttu-id="1d509-170">a presença</span><span class="sxs-lookup"><span data-stu-id="1d509-170">showPresence</span></span>   | <span data-ttu-id="1d509-171">Definir sinalizador para exibir a presença de pessoa-o padrão é `false` .</span><span class="sxs-lookup"><span data-stu-id="1d509-171">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="1d509-172">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="1d509-172">CSS custom properties</span></span>

<span data-ttu-id="1d509-173">O `mgt-person` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="1d509-173">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  
  --initials-color: white;
  --initials-background-color: magenta;

  --presence-background-color: #ffffff;
  --presence-icon-color: #ffffff;

  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 500;
  --color: black;
  --text-transform: none;

  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: black;
  --line2-text-transform: none;

  --line3-font-size: 12px;
  --line3-font-weight: 400;
  --line3-color: black;
  --line3-text-transform: none;

  --details-spacing: 12px;
}
```

<span data-ttu-id="1d509-174">Para saber mais, confira [estilos de componentes](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="1d509-174">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="1d509-175">Modelos</span><span class="sxs-lookup"><span data-stu-id="1d509-175">Templates</span></span>

<span data-ttu-id="1d509-176">O `mgt-person` componente oferece suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="1d509-176">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="1d509-177">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="1d509-177">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="1d509-178">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="1d509-178">Data type</span></span> | <span data-ttu-id="1d509-179">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="1d509-179">Data context</span></span> | <span data-ttu-id="1d509-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d509-180">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="1d509-181">carregando</span><span class="sxs-lookup"><span data-stu-id="1d509-181">loading</span></span> | <span data-ttu-id="1d509-182">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1d509-182">none</span></span> | <span data-ttu-id="1d509-183">O modelo a ser processado enquanto o componente estiver em um estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="1d509-183">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="1d509-184">sem dados</span><span class="sxs-lookup"><span data-stu-id="1d509-184">no-data</span></span> | <span data-ttu-id="1d509-185">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1d509-185">none</span></span> | <span data-ttu-id="1d509-186">O modelo a ser renderizado quando nenhuma imagem de pessoa ou dados estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="1d509-186">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="1d509-187">Padrão.</span><span class="sxs-lookup"><span data-stu-id="1d509-187">default</span></span> | <span data-ttu-id="1d509-188">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="1d509-188">person: The person details object</span></span> <br> <span data-ttu-id="1d509-189">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="1d509-189">`personImage`: The URL of the image</span></span> | <span data-ttu-id="1d509-190">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="1d509-190">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="1d509-191">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="1d509-191">person-card</span></span> | <span data-ttu-id="1d509-192">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="1d509-192">person: The person details object</span></span> <br> <span data-ttu-id="1d509-193">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="1d509-193">`personImage`: The URL of the image</span></span> | <span data-ttu-id="1d509-194">O modelo para atualizar o item de gerenciamento de pessoa que é exibido ao focalizar ou clique.</span><span class="sxs-lookup"><span data-stu-id="1d509-194">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="1d509-195">O exemplo a seguir define um modelo para o componente Person.</span><span class="sxs-lookup"><span data-stu-id="1d509-195">The following example defines a template for the person component.</span></span>

```html
<mgt-person>
  <template>
    <div data-if="personImage">
      <img src="{{personImage}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a><span data-ttu-id="1d509-196">Cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="1d509-196">Person card</span></span>

<span data-ttu-id="1d509-197">O `mgt-person` componente pode mostrar um `mgt-person-card` em foco ou clique.</span><span class="sxs-lookup"><span data-stu-id="1d509-197">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="1d509-198">Adicionar o controle à página HTML</span><span class="sxs-lookup"><span data-stu-id="1d509-198">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="1d509-199">Atributo</span><span class="sxs-lookup"><span data-stu-id="1d509-199">Attribute</span></span>    |  <span data-ttu-id="1d509-200">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d509-200">Property</span></span>     | <span data-ttu-id="1d509-201">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d509-201">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="1d509-202">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="1d509-202">person-card</span></span> | <span data-ttu-id="1d509-203">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="1d509-203">personCardInteraction</span></span> | <span data-ttu-id="1d509-204">Uma enumeração para determinar a ação do usuário necessária para ativar o painel ou o menu suspenso `hover` `click` .</span><span class="sxs-lookup"><span data-stu-id="1d509-204">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="1d509-205">O valor padrão é `none`</span><span class="sxs-lookup"><span data-stu-id="1d509-205">Default value is `none`</span></span> |


<span data-ttu-id="1d509-206">Para obter mais informações sobre modelos, estilos e atributos, consulte [componente de cartão de pessoa](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="1d509-206">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="1d509-207">Configuração de componente global</span><span class="sxs-lookup"><span data-stu-id="1d509-207">Global component configuration</span></span>

<span data-ttu-id="1d509-208">A `MgtPerson` classe expõe um `config` objeto estático que configura todos os componentes de pessoa no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1d509-208">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="1d509-209">O exemplo a seguir mostra como usar o objeto config.</span><span class="sxs-lookup"><span data-stu-id="1d509-209">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="1d509-210">As propriedades a seguir estão disponíveis no objeto config.</span><span class="sxs-lookup"><span data-stu-id="1d509-210">The following properties are available on the config object.</span></span>

| <span data-ttu-id="1d509-211">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d509-211">Property</span></span> | <span data-ttu-id="1d509-212">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d509-212">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="1d509-213">useContactApis</span><span class="sxs-lookup"><span data-stu-id="1d509-213">useContactApis</span></span> | <span data-ttu-id="1d509-214">`boolean` – Indica se o componente de pessoa pode usar a API de contatos pessoais do Microsoft Graph para pesquisar detalhes e fotos de contato.</span><span class="sxs-lookup"><span data-stu-id="1d509-214">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="1d509-215">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="1d509-215">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="1d509-216">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1d509-216">Microsoft Graph permissions</span></span>

<span data-ttu-id="1d509-217">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d509-217">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="1d509-218">Recurso</span><span class="sxs-lookup"><span data-stu-id="1d509-218">Resource</span></span> | <span data-ttu-id="1d509-219">Permissão</span><span class="sxs-lookup"><span data-stu-id="1d509-219">Permission</span></span>     |
| -| - |
| [<span data-ttu-id="1d509-220">/me</span><span class="sxs-lookup"><span data-stu-id="1d509-220">/me</span></span>](/graph/api/user-get)                              | <span data-ttu-id="1d509-221">User.Read</span><span class="sxs-lookup"><span data-stu-id="1d509-221">User.Read</span></span>          |
| [<span data-ttu-id="1d509-222">$value/me/Photo/</span><span class="sxs-lookup"><span data-stu-id="1d509-222">/me/photo/$value</span></span>](/graph/api/profilephoto-get)        | <span data-ttu-id="1d509-223">User.Read</span><span class="sxs-lookup"><span data-stu-id="1d509-223">User.Read</span></span>          |
| [<span data-ttu-id="1d509-224">/me/People/? $search =</span><span class="sxs-lookup"><span data-stu-id="1d509-224">/me/people/?$search=</span></span>](/graph/api/user-list-people)     | <span data-ttu-id="1d509-225">People.Read</span><span class="sxs-lookup"><span data-stu-id="1d509-225">People.Read</span></span>        |
| [<span data-ttu-id="1d509-226">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="1d509-226">/me/contacts/\*</span></span>](/graph/api/user-list-contacts&tabs=cs) | <span data-ttu-id="1d509-227">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1d509-227">Contacts.Read</span></span>      |
| [<span data-ttu-id="1d509-228">$value/Users/{ID}/Photo/</span><span class="sxs-lookup"><span data-stu-id="1d509-228">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people) | <span data-ttu-id="1d509-229">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="1d509-229">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="1d509-230">/me/presence</span><span class="sxs-lookup"><span data-stu-id="1d509-230">/me/presence</span></span>](/graph/api/presence-get)                | <span data-ttu-id="1d509-231">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="1d509-231">Presence.Read</span></span> |
| [<span data-ttu-id="1d509-232">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="1d509-232">/users/{id}/presence</span></span>](/graph/api/presence-get)        | <span data-ttu-id="1d509-233">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d509-233">Presence.Read.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="1d509-234">Autenticação</span><span class="sxs-lookup"><span data-stu-id="1d509-234">Authentication</span></span>

<span data-ttu-id="1d509-235">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.</span><span class="sxs-lookup"><span data-stu-id="1d509-235">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="1d509-236">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="1d509-236">Extend for more control</span></span>

<span data-ttu-id="1d509-237">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="1d509-237">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="1d509-238">Método</span><span class="sxs-lookup"><span data-stu-id="1d509-238">Method</span></span> | <span data-ttu-id="1d509-239">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d509-239">Description</span></span> |
| - | - |
| <span data-ttu-id="1d509-240">renderLoading</span><span class="sxs-lookup"><span data-stu-id="1d509-240">renderLoading</span></span> | <span data-ttu-id="1d509-241">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="1d509-241">Renders the loading state.</span></span> |
| <span data-ttu-id="1d509-242">renderNoData</span><span class="sxs-lookup"><span data-stu-id="1d509-242">renderNoData</span></span> | <span data-ttu-id="1d509-243">Renderiza quando nenhum dado de imagem ou pessoa está disponível.</span><span class="sxs-lookup"><span data-stu-id="1d509-243">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="1d509-244">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="1d509-244">renderAvatar</span></span> | <span data-ttu-id="1d509-245">Renderiza o Avatar.</span><span class="sxs-lookup"><span data-stu-id="1d509-245">Renders the avatar.</span></span> |
| <span data-ttu-id="1d509-246">renderDetails</span><span class="sxs-lookup"><span data-stu-id="1d509-246">renderDetails</span></span> | <span data-ttu-id="1d509-247">Renderiza a parte de detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d509-247">Renders the person details part.</span></span> |
