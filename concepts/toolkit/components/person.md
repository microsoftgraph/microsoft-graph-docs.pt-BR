---
title: Componente person no microsoft graph Toolkit
description: O componente de pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 5250919404ecccea1f01042d93aaf2b9fa4fc3b3
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266840"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="a9c32-103">Componente person no microsoft graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="a9c32-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="a9c32-104">O componente de pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome, endereço de email ou qualquer outro detalhe de pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="a9c32-105">O componente de pessoa também usa [o mgt-person-card](./person-card.md) para exibir um cartão de sub-sub-uso com informações adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="a9c32-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="a9c32-106">Para obter detalhes, consulte a [seção Cartão de](#person-card) Pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="a9c32-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9c32-107">Example</span></span>

<span data-ttu-id="a9c32-108">O exemplo a seguir exibe uma pessoa usando o `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="a9c32-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="a9c32-109">Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="a9c32-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="a9c32-110">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="a9c32-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="a9c32-111">Definindo os detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="a9c32-111">Setting the person details</span></span>

<span data-ttu-id="a9c32-112">Você pode usar três propriedades para definir os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="a9c32-113">Use apenas uma das seguintes propriedades por instância:</span><span class="sxs-lookup"><span data-stu-id="a9c32-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="a9c32-114">De definir `user-id` o atributo ou a propriedade para buscar o usuário do Microsoft Graph usando sua `userId` ID.</span><span class="sxs-lookup"><span data-stu-id="a9c32-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="a9c32-115">De definir `person-query` o atributo ou a propriedade para pesquisar o Microsoft Graph por uma determinada `personQuery` pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="a9c32-116">Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="a9c32-117">Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.</span><span class="sxs-lookup"><span data-stu-id="a9c32-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="a9c32-118">De definir `person-presence` o atributo ou a propriedade para adicionar um selo de presença ao avatar da pessoa `personPresence` manualmente.</span><span class="sxs-lookup"><span data-stu-id="a9c32-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="a9c32-119">De definir `avatar-size` o atributo ou a propriedade como ou para determinar o tamanho do `avatarSize` `small` `large` avatar.</span><span class="sxs-lookup"><span data-stu-id="a9c32-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="a9c32-120">Isso ajuda a adicionar [o selo de presença correto](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) ao avatar.</span><span class="sxs-lookup"><span data-stu-id="a9c32-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="a9c32-121">Você precisará escolher as propriedades personalizadas css correspondentes corretas mostradas abaixo para personalizar ainda mais o tamanho do avatar.</span><span class="sxs-lookup"><span data-stu-id="a9c32-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="a9c32-122">Por padrão, o valor é definido para o qual decidirá automaticamente como renderizar a `auto` presença com base na `view` propriedade.</span><span class="sxs-lookup"><span data-stu-id="a9c32-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="a9c32-123">Recomendamos usar `small` se seu avatar for menor que 32px por 32px.</span><span class="sxs-lookup"><span data-stu-id="a9c32-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="a9c32-124">Use o atributo ou a propriedade para definir manualmente os detalhes da `person-details` `personDetails` pessoa, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="a9c32-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="a9c32-125">Se nenhuma imagem for fornecida, uma será buscada (se disponível).</span><span class="sxs-lookup"><span data-stu-id="a9c32-125">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="a9c32-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9c32-126">Properties</span></span>

<span data-ttu-id="a9c32-127">Você pode usar várias propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="a9c32-127">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="a9c32-128">Atributo</span><span class="sxs-lookup"><span data-stu-id="a9c32-128">Attribute</span></span>       | <span data-ttu-id="a9c32-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9c32-129">Property</span></span>       | <span data-ttu-id="a9c32-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c32-130">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="a9c32-131">user-id</span><span class="sxs-lookup"><span data-stu-id="a9c32-131">user-id</span></span>         | <span data-ttu-id="a9c32-132">userId</span><span class="sxs-lookup"><span data-stu-id="a9c32-132">userId</span></span>         | <span data-ttu-id="a9c32-133">De acordo com uma id do usuário para buscar os detalhes e a imagem desse usuário do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a9c32-133">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="a9c32-134">person-query</span><span class="sxs-lookup"><span data-stu-id="a9c32-134">person-query</span></span>    | <span data-ttu-id="a9c32-135">personQuery</span><span class="sxs-lookup"><span data-stu-id="a9c32-135">personQuery</span></span>    | <span data-ttu-id="a9c32-136">De definida como um nome ou email de uma pessoa para pesquisar uma pessoa no Microsoft Graph e buscar os detalhes e a imagem da primeira pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-136">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="a9c32-137">person-details</span><span class="sxs-lookup"><span data-stu-id="a9c32-137">person-details</span></span>  | <span data-ttu-id="a9c32-138">personDetails</span><span class="sxs-lookup"><span data-stu-id="a9c32-138">personDetails</span></span>  | <span data-ttu-id="a9c32-139">De acordo com um objeto que representa uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-139">Set to an object representing a person.</span></span> <span data-ttu-id="a9c32-140">Funciona com o objeto de pessoas, usuários, contatos ou grupos, recursos.</span><span class="sxs-lookup"><span data-stu-id="a9c32-140">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="a9c32-141">fallback-details</span><span class="sxs-lookup"><span data-stu-id="a9c32-141">fallback-details</span></span>| <span data-ttu-id="a9c32-142">fallbackDetails</span><span class="sxs-lookup"><span data-stu-id="a9c32-142">fallbackDetails</span></span>| <span data-ttu-id="a9c32-143">De acordo com um objeto que representa uma pessoa quando nenhum usuário/pessoa/contato é encontrado no gráfico.</span><span class="sxs-lookup"><span data-stu-id="a9c32-143">Set to an object representing a person when no user/person/contact is found in the graph.</span></span>
| <span data-ttu-id="a9c32-144">person-image</span><span class="sxs-lookup"><span data-stu-id="a9c32-144">person-image</span></span>    | <span data-ttu-id="a9c32-145">personImage</span><span class="sxs-lookup"><span data-stu-id="a9c32-145">personImage</span></span>    | <span data-ttu-id="a9c32-146">De definir a imagem para mostrar para a pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-146">Set the image to show for the person.</span></span> |
| <span data-ttu-id="a9c32-147">presença de pessoa</span><span class="sxs-lookup"><span data-stu-id="a9c32-147">person-presence</span></span> | <span data-ttu-id="a9c32-148">personPresence</span><span class="sxs-lookup"><span data-stu-id="a9c32-148">personPresence</span></span> | <span data-ttu-id="a9c32-149">Desmarcar a presença da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-149">Set the presence for the person.</span></span> |
| <span data-ttu-id="a9c32-150">fetch-image</span><span class="sxs-lookup"><span data-stu-id="a9c32-150">fetch-image</span></span>     | <span data-ttu-id="a9c32-151">fetchImage</span><span class="sxs-lookup"><span data-stu-id="a9c32-151">fetchImage</span></span>     | <span data-ttu-id="a9c32-152">De definir o sinalizador `personImage` para buscar automaticamente do Microsoft Graph com base `personDetails` no objeto fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="a9c32-152">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="a9c32-153">tipo avatar</span><span class="sxs-lookup"><span data-stu-id="a9c32-153">avatar-type</span></span>     | <span data-ttu-id="a9c32-154">avatarType</span><span class="sxs-lookup"><span data-stu-id="a9c32-154">avatarType</span></span>     | <span data-ttu-id="a9c32-155">Definir ou `initials` `photo` renderizar o estado de exibição - o padrão é foto.</span><span class="sxs-lookup"><span data-stu-id="a9c32-155">Set to `initials` or `photo` to render either display state - default is photo.</span></span> |
| <span data-ttu-id="a9c32-156">modo de exibição</span><span class="sxs-lookup"><span data-stu-id="a9c32-156">view</span></span>            | <span data-ttu-id="a9c32-157">modo de exibição</span><span class="sxs-lookup"><span data-stu-id="a9c32-157">view</span></span>           | <span data-ttu-id="a9c32-158">Definir para controlar como a pessoa é renderizada.</span><span class="sxs-lookup"><span data-stu-id="a9c32-158">Set to control how the person is rendered.</span></span> <span data-ttu-id="a9c32-159">O padrão é `avatar`</span><span class="sxs-lookup"><span data-stu-id="a9c32-159">Default is `avatar`</span></span> <br /> <span data-ttu-id="a9c32-160">`avatar` - mostrar somente o avatar</span><span class="sxs-lookup"><span data-stu-id="a9c32-160">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="a9c32-161">`oneline` - mostrar avatar e primeira linha ( `displayName` por padrão)</span><span class="sxs-lookup"><span data-stu-id="a9c32-161">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="a9c32-162">`twolines` - mostrar avatar e duas linhas de texto ( `displayName` `mail` e por padrão)</span><span class="sxs-lookup"><span data-stu-id="a9c32-162">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="a9c32-163">line1-property</span><span class="sxs-lookup"><span data-stu-id="a9c32-163">line1-property</span></span>  | <span data-ttu-id="a9c32-164">line1Property</span><span class="sxs-lookup"><span data-stu-id="a9c32-164">line1Property</span></span>  | <span data-ttu-id="a9c32-165">Define a propriedade da personDetails a ser usada para a primeira linha de texto.</span><span class="sxs-lookup"><span data-stu-id="a9c32-165">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="a9c32-166">O padrão é `displayName`.</span><span class="sxs-lookup"><span data-stu-id="a9c32-166">Default is `displayName`.</span></span>|
| <span data-ttu-id="a9c32-167">line2-property</span><span class="sxs-lookup"><span data-stu-id="a9c32-167">line2-property</span></span>  | <span data-ttu-id="a9c32-168">line2Property</span><span class="sxs-lookup"><span data-stu-id="a9c32-168">line2Property</span></span>  | <span data-ttu-id="a9c32-169">Define a propriedade da personDetails a ser usada para a segunda linha de texto.</span><span class="sxs-lookup"><span data-stu-id="a9c32-169">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="a9c32-170">O padrão é `mail`.</span><span class="sxs-lookup"><span data-stu-id="a9c32-170">Default is `mail`.</span></span>|
| <span data-ttu-id="a9c32-171">line3-property</span><span class="sxs-lookup"><span data-stu-id="a9c32-171">line3-property</span></span>  | <span data-ttu-id="a9c32-172">line3Property</span><span class="sxs-lookup"><span data-stu-id="a9c32-172">line3Property</span></span>  | <span data-ttu-id="a9c32-173">Define a propriedade da personDetails a ser usada para a terceira linha de texto.</span><span class="sxs-lookup"><span data-stu-id="a9c32-173">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="a9c32-174">O padrão é `jobTitle`.</span><span class="sxs-lookup"><span data-stu-id="a9c32-174">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="a9c32-175">show-presence</span><span class="sxs-lookup"><span data-stu-id="a9c32-175">show-presence</span></span>   | <span data-ttu-id="a9c32-176">showPresence</span><span class="sxs-lookup"><span data-stu-id="a9c32-176">showPresence</span></span>   | <span data-ttu-id="a9c32-177">Definir sinalizador para exibir a presença da pessoa - o padrão é `false` .</span><span class="sxs-lookup"><span data-stu-id="a9c32-177">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="a9c32-178">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="a9c32-178">CSS custom properties</span></span>

<span data-ttu-id="a9c32-179">O `mgt-person` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="a9c32-179">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="a9c32-180">Para saber mais, confira [componentes de estilo](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="a9c32-180">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="a9c32-181">Eventos</span><span class="sxs-lookup"><span data-stu-id="a9c32-181">Events</span></span>

<span data-ttu-id="a9c32-182">Os eventos a seguir são disparados do componente.</span><span class="sxs-lookup"><span data-stu-id="a9c32-182">The following events are fired from the component.</span></span>

| <span data-ttu-id="a9c32-183">Evento</span><span class="sxs-lookup"><span data-stu-id="a9c32-183">Event</span></span> | <span data-ttu-id="a9c32-184">Detalhe</span><span class="sxs-lookup"><span data-stu-id="a9c32-184">Detail</span></span> | <span data-ttu-id="a9c32-185">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c32-185">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="a9c32-186">line1clicked</span><span class="sxs-lookup"><span data-stu-id="a9c32-186">line1clicked</span></span> | <span data-ttu-id="a9c32-187">O detalhe contém o objeto `person` respectivo</span><span class="sxs-lookup"><span data-stu-id="a9c32-187">The detail contains the respective `person` object</span></span> | <span data-ttu-id="a9c32-188">Acionado quando a linha1 é clicada.</span><span class="sxs-lookup"><span data-stu-id="a9c32-188">Fired when line1 is clicked.</span></span> |
| <span data-ttu-id="a9c32-189">line2clicked</span><span class="sxs-lookup"><span data-stu-id="a9c32-189">line2clicked</span></span> | <span data-ttu-id="a9c32-190">O detalhe contém o objeto `person` respectivo</span><span class="sxs-lookup"><span data-stu-id="a9c32-190">The detail contains the respective `person` object</span></span> | <span data-ttu-id="a9c32-191">Disparado quando a linha2 é clicada.</span><span class="sxs-lookup"><span data-stu-id="a9c32-191">Fired when line2 is clicked.</span></span> |
| <span data-ttu-id="a9c32-192">line3clicked</span><span class="sxs-lookup"><span data-stu-id="a9c32-192">line3clicked</span></span> | <span data-ttu-id="a9c32-193">O detalhe contém o objeto `person` respectivo</span><span class="sxs-lookup"><span data-stu-id="a9c32-193">The detail contains the respective `person` object</span></span> | <span data-ttu-id="a9c32-194">Acionado quando a linha3 é clicada.</span><span class="sxs-lookup"><span data-stu-id="a9c32-194">Fired when line3 is clicked.</span></span> |

## <a name="templates"></a><span data-ttu-id="a9c32-195">Modelos</span><span class="sxs-lookup"><span data-stu-id="a9c32-195">Templates</span></span>

<span data-ttu-id="a9c32-196">O `mgt-person` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="a9c32-196">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="a9c32-197">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes:</span><span class="sxs-lookup"><span data-stu-id="a9c32-197">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="a9c32-198">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="a9c32-198">Data type</span></span> | <span data-ttu-id="a9c32-199">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="a9c32-199">Data context</span></span> | <span data-ttu-id="a9c32-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c32-200">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="a9c32-201">loading</span><span class="sxs-lookup"><span data-stu-id="a9c32-201">loading</span></span> | <span data-ttu-id="a9c32-202">nenhuma</span><span class="sxs-lookup"><span data-stu-id="a9c32-202">none</span></span> | <span data-ttu-id="a9c32-203">O modelo a ser render enquanto o componente está em um estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="a9c32-203">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="a9c32-204">no-data</span><span class="sxs-lookup"><span data-stu-id="a9c32-204">no-data</span></span> | <span data-ttu-id="a9c32-205">nenhuma</span><span class="sxs-lookup"><span data-stu-id="a9c32-205">none</span></span> | <span data-ttu-id="a9c32-206">O modelo a ser renderizar quando nenhuma imagem ou dados de pessoa estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="a9c32-206">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="a9c32-207">Padrão.</span><span class="sxs-lookup"><span data-stu-id="a9c32-207">default</span></span> | <span data-ttu-id="a9c32-208">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="a9c32-208">person: The person details object</span></span> <br> <span data-ttu-id="a9c32-209">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="a9c32-209">`personImage`: The URL of the image</span></span> | <span data-ttu-id="a9c32-210">O modelo padrão substitui todo o componente por seu próprio.</span><span class="sxs-lookup"><span data-stu-id="a9c32-210">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="a9c32-211">person-card</span><span class="sxs-lookup"><span data-stu-id="a9c32-211">person-card</span></span> | <span data-ttu-id="a9c32-212">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="a9c32-212">person: The person details object</span></span> <br> <span data-ttu-id="a9c32-213">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="a9c32-213">`personImage`: The URL of the image</span></span> | <span data-ttu-id="a9c32-214">O modelo para atualizar o mgt-person-card exibido em foco ou clique.</span><span class="sxs-lookup"><span data-stu-id="a9c32-214">The template to update the mgt-person-card displayed on hover or click.</span></span> |
| <span data-ttu-id="a9c32-215">line1</span><span class="sxs-lookup"><span data-stu-id="a9c32-215">line1</span></span> | <span data-ttu-id="a9c32-216">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="a9c32-216">person: The person details object</span></span> | <span data-ttu-id="a9c32-217">O modelo para a primeira linha de metadados de pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-217">The template for the first line of person metadata.</span></span> |
| <span data-ttu-id="a9c32-218">line2</span><span class="sxs-lookup"><span data-stu-id="a9c32-218">line2</span></span> | <span data-ttu-id="a9c32-219">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="a9c32-219">person: The person details object</span></span> | <span data-ttu-id="a9c32-220">O modelo para a segunda linha de metadados de pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-220">The template for the second line of person metadata.</span></span> |
| <span data-ttu-id="a9c32-221">line3</span><span class="sxs-lookup"><span data-stu-id="a9c32-221">line3</span></span> | <span data-ttu-id="a9c32-222">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="a9c32-222">person: The person details object</span></span> | <span data-ttu-id="a9c32-223">O modelo para a terceira linha de metadados de pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-223">The template for the third line of person metadata.</span></span> |

<span data-ttu-id="a9c32-224">O exemplo a seguir define um modelo para o componente da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-224">The following example defines a template for the person component.</span></span>

```html
<!-- Retemplate the entire person component -->
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

<!-- Retemplate the line properties -->
<mgt-person view="threeLines">
  <template data-type="line1">
    <div>
      Hello, my name is: {{person.displayName}}
    </div>
  </template>
  <template data-type="line2">
    <div>
      Super cool
    </div>
  </template>
  <template data-type="line3">
    <div>
      Loves MGT
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a><span data-ttu-id="a9c32-225">Cartão pessoal</span><span class="sxs-lookup"><span data-stu-id="a9c32-225">Person card</span></span>

<span data-ttu-id="a9c32-226">O `mgt-person` componente pode mostrar um ao passar o mouse ou `mgt-person-card` clicar.</span><span class="sxs-lookup"><span data-stu-id="a9c32-226">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="a9c32-227">Adicionar o controle à página HTML</span><span class="sxs-lookup"><span data-stu-id="a9c32-227">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="a9c32-228">Atributo</span><span class="sxs-lookup"><span data-stu-id="a9c32-228">Attribute</span></span>    |  <span data-ttu-id="a9c32-229">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9c32-229">Property</span></span>     | <span data-ttu-id="a9c32-230">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c32-230">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="a9c32-231">person-card</span><span class="sxs-lookup"><span data-stu-id="a9c32-231">person-card</span></span> | <span data-ttu-id="a9c32-232">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="a9c32-232">personCardInteraction</span></span> | <span data-ttu-id="a9c32-233">Uma enumeração para determinar a ação do usuário necessária para ativar o painel do sub-sub-plano - `hover` ou `click` .</span><span class="sxs-lookup"><span data-stu-id="a9c32-233">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="a9c32-234">O valor padrão é `none`</span><span class="sxs-lookup"><span data-stu-id="a9c32-234">Default value is `none`</span></span> |


<span data-ttu-id="a9c32-235">Para obter mais informações sobre a templating, o estilo e os atributos, consulte [Person Card component](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="a9c32-235">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="a9c32-236">Configuração de componente global</span><span class="sxs-lookup"><span data-stu-id="a9c32-236">Global component configuration</span></span>

<span data-ttu-id="a9c32-237">A `MgtPerson` classe expõe um objeto `config` estático que configura todos os componentes da pessoa no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a9c32-237">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="a9c32-238">O exemplo a seguir mostra como usar o objeto config.</span><span class="sxs-lookup"><span data-stu-id="a9c32-238">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="a9c32-239">As propriedades a seguir estão disponíveis no objeto config.</span><span class="sxs-lookup"><span data-stu-id="a9c32-239">The following properties are available on the config object.</span></span>

| <span data-ttu-id="a9c32-240">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9c32-240">Property</span></span> | <span data-ttu-id="a9c32-241">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c32-241">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="a9c32-242">useContactApis</span><span class="sxs-lookup"><span data-stu-id="a9c32-242">useContactApis</span></span> | <span data-ttu-id="a9c32-243">`boolean` - Indica se o componente da pessoa pode usar a API de contatos pessoais do Microsoft Graph para pesquisar detalhes de contato e fotos.</span><span class="sxs-lookup"><span data-stu-id="a9c32-243">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="a9c32-244">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="a9c32-244">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="a9c32-245">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a9c32-245">Microsoft Graph permissions</span></span>

<span data-ttu-id="a9c32-246">Esse controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a9c32-246">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="a9c32-247">Recurso</span><span class="sxs-lookup"><span data-stu-id="a9c32-247">Resource</span></span> | <span data-ttu-id="a9c32-248">Permissão</span><span class="sxs-lookup"><span data-stu-id="a9c32-248">Permission</span></span>     |
| -| - |
| [<span data-ttu-id="a9c32-249">/me</span><span class="sxs-lookup"><span data-stu-id="a9c32-249">/me</span></span>](/graph/api/user-get)                              | <span data-ttu-id="a9c32-250">User.Read</span><span class="sxs-lookup"><span data-stu-id="a9c32-250">User.Read</span></span>          |
| [<span data-ttu-id="a9c32-251">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="a9c32-251">/me/photo/$value</span></span>](/graph/api/profilephoto-get)        | <span data-ttu-id="a9c32-252">User.Read</span><span class="sxs-lookup"><span data-stu-id="a9c32-252">User.Read</span></span>          |
| [<span data-ttu-id="a9c32-253">/me/people/?$search=</span><span class="sxs-lookup"><span data-stu-id="a9c32-253">/me/people/?$search=</span></span>](/graph/api/user-list-people)     | <span data-ttu-id="a9c32-254">People.Read</span><span class="sxs-lookup"><span data-stu-id="a9c32-254">People.Read</span></span>        |
| [<span data-ttu-id="a9c32-255">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="a9c32-255">/me/contacts/\*</span></span>](/graph/api/user-list-contacts&tabs=cs) | <span data-ttu-id="a9c32-256">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a9c32-256">Contacts.Read</span></span>      |
| [<span data-ttu-id="a9c32-257">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="a9c32-257">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people) | <span data-ttu-id="a9c32-258">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="a9c32-258">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="a9c32-259">/me/presence</span><span class="sxs-lookup"><span data-stu-id="a9c32-259">/me/presence</span></span>](/graph/api/presence-get)                | <span data-ttu-id="a9c32-260">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="a9c32-260">Presence.Read</span></span> |
| [<span data-ttu-id="a9c32-261">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="a9c32-261">/users/{id}/presence</span></span>](/graph/api/presence-get)        | <span data-ttu-id="a9c32-262">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9c32-262">Presence.Read.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="a9c32-263">Autenticação</span><span class="sxs-lookup"><span data-stu-id="a9c32-263">Authentication</span></span>

<span data-ttu-id="a9c32-264">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.</span><span class="sxs-lookup"><span data-stu-id="a9c32-264">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="a9c32-265">Cache</span><span class="sxs-lookup"><span data-stu-id="a9c32-265">Cache</span></span>

|<span data-ttu-id="a9c32-266">Armazenamento de objetos</span><span class="sxs-lookup"><span data-stu-id="a9c32-266">Object store</span></span>|<span data-ttu-id="a9c32-267">Dados armazenados em cache</span><span class="sxs-lookup"><span data-stu-id="a9c32-267">Cached data</span></span>|<span data-ttu-id="a9c32-268">Comentários</span><span class="sxs-lookup"><span data-stu-id="a9c32-268">Remarks</span></span>|
|---------|-----------|-------|
|`photos`|<span data-ttu-id="a9c32-269">Foto da pessoa</span><span class="sxs-lookup"><span data-stu-id="a9c32-269">Person's photo</span></span>|<span data-ttu-id="a9c32-270">Usado, quando `avatarType` é definido como e é definido `photo` `fetchImage` como `true`</span><span class="sxs-lookup"><span data-stu-id="a9c32-270">Used, when `avatarType` is set to `photo` and `fetchImage` is set to `true`</span></span>|
|`presence`|<span data-ttu-id="a9c32-271">Presença da pessoa</span><span class="sxs-lookup"><span data-stu-id="a9c32-271">Person's presence</span></span>|<span data-ttu-id="a9c32-272">Usado, quando `showPresence` está definido como `true`</span><span class="sxs-lookup"><span data-stu-id="a9c32-272">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="a9c32-273">Informações do usuário da pessoa</span><span class="sxs-lookup"><span data-stu-id="a9c32-273">Person's user information</span></span>|

<span data-ttu-id="a9c32-274">Consulte [Cache para](../customize-components/cache.md) obter mais detalhes sobre como configurar o cache.</span><span class="sxs-lookup"><span data-stu-id="a9c32-274">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="a9c32-275">Estender para obter mais controle</span><span class="sxs-lookup"><span data-stu-id="a9c32-275">Extend for more control</span></span>

<span data-ttu-id="a9c32-276">Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes.</span><span class="sxs-lookup"><span data-stu-id="a9c32-276">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="a9c32-277">Método</span><span class="sxs-lookup"><span data-stu-id="a9c32-277">Method</span></span> | <span data-ttu-id="a9c32-278">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c32-278">Description</span></span> |
| - | - |
| <span data-ttu-id="a9c32-279">renderLoading</span><span class="sxs-lookup"><span data-stu-id="a9c32-279">renderLoading</span></span> | <span data-ttu-id="a9c32-280">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="a9c32-280">Renders the loading state.</span></span> |
| <span data-ttu-id="a9c32-281">renderNoData</span><span class="sxs-lookup"><span data-stu-id="a9c32-281">renderNoData</span></span> | <span data-ttu-id="a9c32-282">Renderiza quando nenhum dado de imagem ou pessoa está disponível.</span><span class="sxs-lookup"><span data-stu-id="a9c32-282">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="a9c32-283">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="a9c32-283">renderAvatar</span></span> | <span data-ttu-id="a9c32-284">Renderiza o avatar.</span><span class="sxs-lookup"><span data-stu-id="a9c32-284">Renders the avatar.</span></span> |
| <span data-ttu-id="a9c32-285">renderDetails</span><span class="sxs-lookup"><span data-stu-id="a9c32-285">renderDetails</span></span> | <span data-ttu-id="a9c32-286">Renderiza a parte de detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="a9c32-286">Renders the person details part.</span></span> |
