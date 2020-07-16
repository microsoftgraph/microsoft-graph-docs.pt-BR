---
title: Componente Person no Microsoft Graph Toolkit
description: O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: d944fa470b8d0f6baffb56d5cd997fe2a0bd7c91
ms.sourcegitcommit: 9f1e02ab486a2c3e0a128e5d36f46cebe4961581
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2020
ms.locfileid: "45024415"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d5637-103">Componente Person no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="d5637-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d5637-104">O componente pessoa é usado para exibir uma pessoa ou contato usando a foto, o nome, o endereço de email ou qualquer outro detalhe de pessoa.</span><span class="sxs-lookup"><span data-stu-id="d5637-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="d5637-105">O componente pessoa também usa a [pessoa de gerenciamento de pessoas](./person-card.md) para exibir um cartão de submenu com informações adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="d5637-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="d5637-106">Para obter detalhes, consulte a seção [cartão de pessoa](#person-card) .</span><span class="sxs-lookup"><span data-stu-id="d5637-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="d5637-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5637-107">Example</span></span>

<span data-ttu-id="d5637-108">O exemplo a seguir exibe uma pessoa usando o `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="d5637-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="d5637-109">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="d5637-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="d5637-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="d5637-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="d5637-111">Configurando os detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="d5637-111">Setting the person details</span></span>

<span data-ttu-id="d5637-112">Você pode usar três propriedades para definir os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="d5637-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="d5637-113">Use apenas uma das seguintes propriedades por instância:</span><span class="sxs-lookup"><span data-stu-id="d5637-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="d5637-114">Defina o `user-id` atributo ou a `userId` propriedade para buscar o usuário do Microsoft Graph usando sua ID.</span><span class="sxs-lookup"><span data-stu-id="d5637-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="d5637-115">Definir o `person-query` atributo ou a `personQuery` propriedade para pesquisar o Microsoft Graph em uma determinada pessoa.</span><span class="sxs-lookup"><span data-stu-id="d5637-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="d5637-116">Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="d5637-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="d5637-117">Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.</span><span class="sxs-lookup"><span data-stu-id="d5637-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="d5637-118">Defina o `person-presence` atributo ou a `personPresence` propriedade para adicionar um emblema de presença ao avatar manualmente.</span><span class="sxs-lookup"><span data-stu-id="d5637-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="d5637-119">Defina o `avatar-size` atributo ou a `avatarSize` propriedade como `small` ou `large` para determinar o tamanho do Avatar.</span><span class="sxs-lookup"><span data-stu-id="d5637-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="d5637-120">Isso ajuda a adicionar o [emblema de presença correto](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) ao avatar.</span><span class="sxs-lookup"><span data-stu-id="d5637-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="d5637-121">Você precisará escolher as propriedades personalizadas de CSS correspondentes indicadas abaixo para personalizar ainda mais o tamanho do Avatar.</span><span class="sxs-lookup"><span data-stu-id="d5637-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="d5637-122">Por padrão, o valor é definido como o `auto` qual decidirá automaticamente como renderizar a presença com base na `view` propriedade.</span><span class="sxs-lookup"><span data-stu-id="d5637-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="d5637-123">Recomendamos usar `small` o se o seu avatar for menor do que o medianiz 32px por medianiz 32px.</span><span class="sxs-lookup"><span data-stu-id="d5637-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="d5637-124">Use o `person-details` atributo ou `personDetails` propriedade para definir manualmente os detalhes da pessoa, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="d5637-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="d5637-125">Se nenhuma imagem for fornecida, uma será buscada (se disponível).</span><span class="sxs-lookup"><span data-stu-id="d5637-125">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="d5637-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5637-126">Properties</span></span>

<span data-ttu-id="d5637-127">Você pode usar várias propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="d5637-127">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="d5637-128">Atributo</span><span class="sxs-lookup"><span data-stu-id="d5637-128">Attribute</span></span>       | <span data-ttu-id="d5637-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5637-129">Property</span></span>       | <span data-ttu-id="d5637-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5637-130">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="d5637-131">ID de usuário</span><span class="sxs-lookup"><span data-stu-id="d5637-131">user-id</span></span>         | <span data-ttu-id="d5637-132">userId</span><span class="sxs-lookup"><span data-stu-id="d5637-132">userId</span></span>         | <span data-ttu-id="d5637-133">Defina como uma ID de usuário para buscar os detalhes e a imagem do usuário do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d5637-133">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="d5637-134">pessoa – consulta</span><span class="sxs-lookup"><span data-stu-id="d5637-134">person-query</span></span>    | <span data-ttu-id="d5637-135">personQuery</span><span class="sxs-lookup"><span data-stu-id="d5637-135">personQuery</span></span>    | <span data-ttu-id="d5637-136">Defina como um nome ou email de uma pessoa para pesquisar uma pessoa no Microsoft Graph e busque os detalhes e a imagem da primeira pessoa.</span><span class="sxs-lookup"><span data-stu-id="d5637-136">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="d5637-137">pessoa-detalhes</span><span class="sxs-lookup"><span data-stu-id="d5637-137">person-details</span></span>  | <span data-ttu-id="d5637-138">personDetails</span><span class="sxs-lookup"><span data-stu-id="d5637-138">personDetails</span></span>  | <span data-ttu-id="d5637-139">Defina como um objeto que represente uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="d5637-139">Set to an object representing a person.</span></span> <span data-ttu-id="d5637-140">Funciona com o objeto dos recursos pessoas, usuários, contatos ou grupos.</span><span class="sxs-lookup"><span data-stu-id="d5637-140">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="d5637-141">pessoa-imagem</span><span class="sxs-lookup"><span data-stu-id="d5637-141">person-image</span></span>    | <span data-ttu-id="d5637-142">personImage</span><span class="sxs-lookup"><span data-stu-id="d5637-142">personImage</span></span>    | <span data-ttu-id="d5637-143">Defina a imagem a ser mostrada para a pessoa.</span><span class="sxs-lookup"><span data-stu-id="d5637-143">Set the image to show for the person.</span></span> |
| <span data-ttu-id="d5637-144">presença de pessoa</span><span class="sxs-lookup"><span data-stu-id="d5637-144">person-presence</span></span> | <span data-ttu-id="d5637-145">personPresence</span><span class="sxs-lookup"><span data-stu-id="d5637-145">personPresence</span></span> | <span data-ttu-id="d5637-146">Definir a presença para a pessoa.</span><span class="sxs-lookup"><span data-stu-id="d5637-146">Set the presence for the person.</span></span> |
| <span data-ttu-id="d5637-147">FETCH-Image</span><span class="sxs-lookup"><span data-stu-id="d5637-147">fetch-image</span></span>     | <span data-ttu-id="d5637-148">fetchImage</span><span class="sxs-lookup"><span data-stu-id="d5637-148">fetchImage</span></span>     | <span data-ttu-id="d5637-149">Defina o sinalizador para buscar `personImage` automaticamente a partir do Microsoft Graph com base no `personDetails` objeto fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="d5637-149">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="d5637-150">modo de exibição</span><span class="sxs-lookup"><span data-stu-id="d5637-150">view</span></span>            | <span data-ttu-id="d5637-151">modo de exibição</span><span class="sxs-lookup"><span data-stu-id="d5637-151">view</span></span>           | <span data-ttu-id="d5637-152">Definido para controlar como a pessoa é renderizada.</span><span class="sxs-lookup"><span data-stu-id="d5637-152">Set to control how the person is rendered.</span></span> <span data-ttu-id="d5637-153">O padrão é`avatar`</span><span class="sxs-lookup"><span data-stu-id="d5637-153">Default is `avatar`</span></span> <br /> <span data-ttu-id="d5637-154">`avatar`-Mostrar somente avatar</span><span class="sxs-lookup"><span data-stu-id="d5637-154">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="d5637-155">`oneline`-Mostrar avatar e primeira linha ( `displayName` por padrão)</span><span class="sxs-lookup"><span data-stu-id="d5637-155">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="d5637-156">`twolines`-Mostrar avatar e duas linhas de texto ( `displayName` e `mail` por padrão)</span><span class="sxs-lookup"><span data-stu-id="d5637-156">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="d5637-157">linha1-Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5637-157">line1-property</span></span>  | <span data-ttu-id="d5637-158">line1Property</span><span class="sxs-lookup"><span data-stu-id="d5637-158">line1Property</span></span>  | <span data-ttu-id="d5637-159">Define a propriedade do personDetails a ser usado para a primeira linha do texto.</span><span class="sxs-lookup"><span data-stu-id="d5637-159">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="d5637-160">O padrão é `displayName`.</span><span class="sxs-lookup"><span data-stu-id="d5637-160">Default is `displayName`.</span></span>|
| <span data-ttu-id="d5637-161">Linha2-Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5637-161">line2-property</span></span>  | <span data-ttu-id="d5637-162">line2Property</span><span class="sxs-lookup"><span data-stu-id="d5637-162">line2Property</span></span>  | <span data-ttu-id="d5637-163">Define a propriedade do personDetails a ser usado para a segunda linha de texto.</span><span class="sxs-lookup"><span data-stu-id="d5637-163">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="d5637-164">O padrão é `mail`.</span><span class="sxs-lookup"><span data-stu-id="d5637-164">Default is `mail`.</span></span>|
| <span data-ttu-id="d5637-165">show-Presence</span><span class="sxs-lookup"><span data-stu-id="d5637-165">show-presence</span></span>   | <span data-ttu-id="d5637-166">a presença</span><span class="sxs-lookup"><span data-stu-id="d5637-166">showPresence</span></span>   | <span data-ttu-id="d5637-167">Definir sinalizador para exibir a presença de pessoa-o padrão é `false` .</span><span class="sxs-lookup"><span data-stu-id="d5637-167">Set flag to display person presence - default is `false`.</span></span>|
| <span data-ttu-id="d5637-168">show-Name</span><span class="sxs-lookup"><span data-stu-id="d5637-168">show-name</span></span>       | <span data-ttu-id="d5637-169">Nome do mesmo</span><span class="sxs-lookup"><span data-stu-id="d5637-169">showName</span></span>       | <span data-ttu-id="d5637-170">**Preterido-uso `view` .**</span><span class="sxs-lookup"><span data-stu-id="d5637-170">**DEPRECATED - use `view`.**</span></span>  <span data-ttu-id="d5637-171">Definir sinalizador para exibir o nome de exibição da pessoa-o padrão é `false` .</span><span class="sxs-lookup"><span data-stu-id="d5637-171">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="d5637-172">Mostrar-email</span><span class="sxs-lookup"><span data-stu-id="d5637-172">show-email</span></span>      | <span data-ttu-id="d5637-173">Enviar email</span><span class="sxs-lookup"><span data-stu-id="d5637-173">showEmail</span></span>      | <span data-ttu-id="d5637-174">**Preterido-uso `view` .**</span><span class="sxs-lookup"><span data-stu-id="d5637-174">**DEPRECATED - use `view`.**</span></span> <span data-ttu-id="d5637-175">Definir sinalizador para exibir o email da pessoa-o padrão é `false` .</span><span class="sxs-lookup"><span data-stu-id="d5637-175">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="d5637-176">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="d5637-176">CSS custom properties</span></span>

<span data-ttu-id="d5637-177">O `mgt-person` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="d5637-177">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 500;
  --color: black;
  --presence-background-color: #ffffff;
  --text-transform: none;
  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: black;
  --line2-text-transform: none;
  --details-spacing: 12px;
}
```

<span data-ttu-id="d5637-178">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="d5637-178">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="d5637-179">Modelos</span><span class="sxs-lookup"><span data-stu-id="d5637-179">Templates</span></span>

<span data-ttu-id="d5637-180">O `mgt-person` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="d5637-180">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="d5637-181">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="d5637-181">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="d5637-182">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="d5637-182">Data type</span></span> | <span data-ttu-id="d5637-183">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="d5637-183">Data context</span></span> | <span data-ttu-id="d5637-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5637-184">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="d5637-185">carregando</span><span class="sxs-lookup"><span data-stu-id="d5637-185">loading</span></span> | <span data-ttu-id="d5637-186">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d5637-186">none</span></span> | <span data-ttu-id="d5637-187">O modelo a ser renderizado enquanto o componente está em um estado laoding.</span><span class="sxs-lookup"><span data-stu-id="d5637-187">The template to render while the component is in a laoding state.</span></span> |
| <span data-ttu-id="d5637-188">sem dados</span><span class="sxs-lookup"><span data-stu-id="d5637-188">no-data</span></span> | <span data-ttu-id="d5637-189">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d5637-189">none</span></span> | <span data-ttu-id="d5637-190">O modelo a ser renderizado quando nenhuma imagem de pessoa ou dados estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="d5637-190">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="d5637-191">Padrão.</span><span class="sxs-lookup"><span data-stu-id="d5637-191">default</span></span> | <span data-ttu-id="d5637-192">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="d5637-192">person: The person details object</span></span> <br> <span data-ttu-id="d5637-193">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="d5637-193">`personImage`: The URL of the image</span></span> | <span data-ttu-id="d5637-194">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="d5637-194">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="d5637-195">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="d5637-195">person-card</span></span> | <span data-ttu-id="d5637-196">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="d5637-196">person: The person details object</span></span> <br> <span data-ttu-id="d5637-197">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="d5637-197">`personImage`: The URL of the image</span></span> | <span data-ttu-id="d5637-198">O modelo para atualizar o item de gerenciamento de pessoa que é exibido ao focalizar ou clique.</span><span class="sxs-lookup"><span data-stu-id="d5637-198">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="d5637-199">O exemplo a seguir define um modelo para o componente Person.</span><span class="sxs-lookup"><span data-stu-id="d5637-199">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="d5637-200">Cartão Pessoal</span><span class="sxs-lookup"><span data-stu-id="d5637-200">Person Card</span></span>

<span data-ttu-id="d5637-201">O `mgt-person` componente pode mostrar um `mgt-person-card` em foco ou clique.</span><span class="sxs-lookup"><span data-stu-id="d5637-201">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="d5637-202">Adicionar o controle à página HTML</span><span class="sxs-lookup"><span data-stu-id="d5637-202">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="d5637-203">Atributo</span><span class="sxs-lookup"><span data-stu-id="d5637-203">Attribute</span></span>    |  <span data-ttu-id="d5637-204">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5637-204">Property</span></span>     | <span data-ttu-id="d5637-205">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5637-205">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="d5637-206">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="d5637-206">person-card</span></span> | <span data-ttu-id="d5637-207">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="d5637-207">personCardInteraction</span></span> | <span data-ttu-id="d5637-208">Uma enumeração para determinar a ação do usuário necessária para ativar o painel ou o menu suspenso `hover` `click` .</span><span class="sxs-lookup"><span data-stu-id="d5637-208">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="d5637-209">O valor padrão é`none`</span><span class="sxs-lookup"><span data-stu-id="d5637-209">Default value is `none`</span></span> |


<span data-ttu-id="d5637-210">Para obter mais informações sobre modelos, estilos e atributos, consulte [componente de cartão de pessoa](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="d5637-210">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="d5637-211">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d5637-211">Microsoft Graph permissions</span></span>

<span data-ttu-id="d5637-212">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d5637-212">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="d5637-213">Recurso</span><span class="sxs-lookup"><span data-stu-id="d5637-213">Resource</span></span>                                                                                                    | <span data-ttu-id="d5637-214">Permission</span><span class="sxs-lookup"><span data-stu-id="d5637-214">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="d5637-215">/me</span><span class="sxs-lookup"><span data-stu-id="d5637-215">/me</span></span>](/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="d5637-216">User.Read</span><span class="sxs-lookup"><span data-stu-id="d5637-216">User.Read</span></span>          |
| [<span data-ttu-id="d5637-217">$value/me/Photo/</span><span class="sxs-lookup"><span data-stu-id="d5637-217">/me/photo/$value</span></span>](/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="d5637-218">User.Read</span><span class="sxs-lookup"><span data-stu-id="d5637-218">User.Read</span></span>          |
| [<span data-ttu-id="d5637-219">/me/People/? $search =</span><span class="sxs-lookup"><span data-stu-id="d5637-219">/me/people/?$search=</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="d5637-220">People.Read</span><span class="sxs-lookup"><span data-stu-id="d5637-220">People.Read</span></span>        |
| [<span data-ttu-id="d5637-221">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="d5637-221">/me/contacts/\*</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="d5637-222">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d5637-222">Contacts.Read</span></span>      |
| [<span data-ttu-id="d5637-223">$value/Users/{ID}/Photo/</span><span class="sxs-lookup"><span data-stu-id="d5637-223">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="d5637-224">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="d5637-224">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="d5637-225">/me/presence</span><span class="sxs-lookup"><span data-stu-id="d5637-225">/me/presence</span></span>](/graph/api/presence-get?view=graph-rest-beta)                | <span data-ttu-id="d5637-226">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="d5637-226">Presence.Read</span></span> |
| [<span data-ttu-id="d5637-227">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="d5637-227">/users/{id}/presence</span></span>](/graph/api/presence-get?view=graph-rest-beta)        | <span data-ttu-id="d5637-228">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5637-228">Presence.Read.All</span></span> |

> <span data-ttu-id="d5637-229">**Observação:** para acessar os `*/photo/$value` recursos para contas pessoais da Microsoft, use o ponto de extremidade beta do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d5637-229">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="d5637-230">Autenticação</span><span class="sxs-lookup"><span data-stu-id="d5637-230">Authentication</span></span>

<span data-ttu-id="d5637-231">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md) para buscar os dados necessários.</span><span class="sxs-lookup"><span data-stu-id="d5637-231">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="d5637-232">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="d5637-232">Extend for more control</span></span>

<span data-ttu-id="d5637-233">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="d5637-233">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="d5637-234">Método</span><span class="sxs-lookup"><span data-stu-id="d5637-234">Method</span></span> | <span data-ttu-id="d5637-235">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5637-235">Description</span></span> |
| - | - |
| <span data-ttu-id="d5637-236">renderLoading</span><span class="sxs-lookup"><span data-stu-id="d5637-236">renderLoading</span></span> | <span data-ttu-id="d5637-237">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="d5637-237">Renders the loading state.</span></span> |
| <span data-ttu-id="d5637-238">renderNoData</span><span class="sxs-lookup"><span data-stu-id="d5637-238">renderNoData</span></span> | <span data-ttu-id="d5637-239">Renderiza quando nenhum dado de imagem ou pessoa está disponível.</span><span class="sxs-lookup"><span data-stu-id="d5637-239">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="d5637-240">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="d5637-240">renderAvatar</span></span> | <span data-ttu-id="d5637-241">Renderiza o Avatar.</span><span class="sxs-lookup"><span data-stu-id="d5637-241">Renders the avatar.</span></span> |
| <span data-ttu-id="d5637-242">renderDetails</span><span class="sxs-lookup"><span data-stu-id="d5637-242">renderDetails</span></span> | <span data-ttu-id="d5637-243">Renderiza a parte de detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="d5637-243">Renders the person details part.</span></span> |
