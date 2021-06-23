---
title: Componente person no microsoft Graph Toolkit
description: O componente de pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 7f35b5c1a3ef764995d319e9e603489b50a1fe2c
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082045"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="e6a1a-103">Componente person no microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="e6a1a-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="e6a1a-104">O componente de pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome, endereço de email ou qualquer outro detalhe de pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="e6a1a-105">O componente de pessoa também usa [o mgt-person-card](./person-card.md) para exibir um cartão de sub-sub-uso com informações adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="e6a1a-106">Para obter detalhes, consulte a [seção Cartão de](#person-card) Pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="e6a1a-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6a1a-107">Example</span></span>

<span data-ttu-id="e6a1a-108">O exemplo a seguir exibe uma pessoa usando o `mgt-person` componente.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="e6a1a-109">Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="e6a1a-110">Abrir este exemplo no mgt.dev</span><span class="sxs-lookup"><span data-stu-id="e6a1a-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="e6a1a-111">Definindo os detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="e6a1a-111">Setting the person details</span></span>

<span data-ttu-id="e6a1a-112">Você pode usar três propriedades para definir os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="e6a1a-113">Use apenas uma das seguintes propriedades por instância:</span><span class="sxs-lookup"><span data-stu-id="e6a1a-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="e6a1a-114">De definir `user-id` o atributo ou a propriedade para buscar o usuário da Microsoft Graph usando sua `userId` ID.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="e6a1a-115">De definir `person-query` o atributo ou a propriedade para pesquisar o Microsoft Graph uma determinada `personQuery` pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="e6a1a-116">Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="e6a1a-117">Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="e6a1a-118">De definir `person-presence` o atributo ou a propriedade para adicionar um selo de presença ao avatar da pessoa `personPresence` manualmente.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="e6a1a-119">De definir `avatar-size` o atributo ou a propriedade como ou para determinar o tamanho do `avatarSize` `small` `large` avatar.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="e6a1a-120">Isso ajuda a adicionar [o selo de presença correto](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) ao avatar.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="e6a1a-121">Você precisará escolher as propriedades personalizadas css correspondentes corretas mostradas abaixo para personalizar ainda mais o tamanho do avatar.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="e6a1a-122">Por padrão, o valor é definido para o qual decidirá automaticamente como renderizar a `auto` presença com base na `view` propriedade.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="e6a1a-123">Recomendamos usar `small` se seu avatar for menor que 32px por 32px.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="e6a1a-124">Use o atributo ou a propriedade para definir manualmente os detalhes da `person-details` `personDetails` pessoa, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="e6a1a-125">Se nenhuma imagem for fornecida, uma será buscada (se disponível).</span><span class="sxs-lookup"><span data-stu-id="e6a1a-125">If no image is provided, one will be fetched (if available).</span></span>

* <span data-ttu-id="e6a1a-126">Por padrão, o componente de pessoa solicitará apenas o conjunto de propriedades padrão da Microsoft Graph [usuário.](/graph/api/user-get?&tabs=http#optional-query-parameters)</span><span class="sxs-lookup"><span data-stu-id="e6a1a-126">By default, the person component will only request the standard Microsoft Graph user set of [properties](/graph/api/user-get?&tabs=http#optional-query-parameters).</span></span> <span data-ttu-id="e6a1a-127">Para solicitar propriedades adicionais, declare-as como qualquer parte do `line(x)Property` .</span><span class="sxs-lookup"><span data-stu-id="e6a1a-127">In order to request additional properties, declare them as any part of the `line(x)Property`.</span></span> 


## <a name="properties"></a><span data-ttu-id="e6a1a-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6a1a-128">Properties</span></span>

<span data-ttu-id="e6a1a-129">Você pode usar várias propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-129">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="e6a1a-130">Atributo</span><span class="sxs-lookup"><span data-stu-id="e6a1a-130">Attribute</span></span>       | <span data-ttu-id="e6a1a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6a1a-131">Property</span></span>       | <span data-ttu-id="e6a1a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6a1a-132">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="e6a1a-133">user-id</span><span class="sxs-lookup"><span data-stu-id="e6a1a-133">user-id</span></span>         | <span data-ttu-id="e6a1a-134">userId</span><span class="sxs-lookup"><span data-stu-id="e6a1a-134">userId</span></span>         | <span data-ttu-id="e6a1a-135">De definida como uma id do usuário para buscar os detalhes e a imagem desse usuário da Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-135">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="e6a1a-136">person-query</span><span class="sxs-lookup"><span data-stu-id="e6a1a-136">person-query</span></span>    | <span data-ttu-id="e6a1a-137">personQuery</span><span class="sxs-lookup"><span data-stu-id="e6a1a-137">personQuery</span></span>    | <span data-ttu-id="e6a1a-138">De definida como um nome ou email de uma pessoa para pesquisar uma pessoa no Microsoft Graph e buscar os detalhes e a imagem da primeira pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-138">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="e6a1a-139">person-details</span><span class="sxs-lookup"><span data-stu-id="e6a1a-139">person-details</span></span>  | <span data-ttu-id="e6a1a-140">personDetails</span><span class="sxs-lookup"><span data-stu-id="e6a1a-140">personDetails</span></span>  | <span data-ttu-id="e6a1a-141">De acordo com um objeto que representa uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-141">Set to an object representing a person.</span></span> <span data-ttu-id="e6a1a-142">Funciona com o objeto de pessoas, usuários, contatos ou grupos, recursos.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-142">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="e6a1a-143">fallback-details</span><span class="sxs-lookup"><span data-stu-id="e6a1a-143">fallback-details</span></span>| <span data-ttu-id="e6a1a-144">fallbackDetails</span><span class="sxs-lookup"><span data-stu-id="e6a1a-144">fallbackDetails</span></span>| <span data-ttu-id="e6a1a-145">De acordo com um objeto que representa uma pessoa quando nenhum usuário/pessoa/contato é encontrado no gráfico.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-145">Set to an object representing a person when no user/person/contact is found in the graph.</span></span>
| <span data-ttu-id="e6a1a-146">person-image</span><span class="sxs-lookup"><span data-stu-id="e6a1a-146">person-image</span></span>    | <span data-ttu-id="e6a1a-147">personImage</span><span class="sxs-lookup"><span data-stu-id="e6a1a-147">personImage</span></span>    | <span data-ttu-id="e6a1a-148">De definir a imagem para mostrar para a pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-148">Set the image to show for the person.</span></span> |
| <span data-ttu-id="e6a1a-149">presença de pessoa</span><span class="sxs-lookup"><span data-stu-id="e6a1a-149">person-presence</span></span> | <span data-ttu-id="e6a1a-150">personPresence</span><span class="sxs-lookup"><span data-stu-id="e6a1a-150">personPresence</span></span> | <span data-ttu-id="e6a1a-151">Desmarcar a presença da pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-151">Set the presence for the person.</span></span> |
| <span data-ttu-id="e6a1a-152">fetch-image</span><span class="sxs-lookup"><span data-stu-id="e6a1a-152">fetch-image</span></span>     | <span data-ttu-id="e6a1a-153">fetchImage</span><span class="sxs-lookup"><span data-stu-id="e6a1a-153">fetchImage</span></span>     | <span data-ttu-id="e6a1a-154">De definir o sinalizador para buscar automaticamente do `personImage` Microsoft Graph com base no objeto fornecido pelo `personDetails` usuário.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-154">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="e6a1a-155">tipo avatar</span><span class="sxs-lookup"><span data-stu-id="e6a1a-155">avatar-type</span></span>     | <span data-ttu-id="e6a1a-156">avatarType</span><span class="sxs-lookup"><span data-stu-id="e6a1a-156">avatarType</span></span>     | <span data-ttu-id="e6a1a-157">Definir ou `initials` `photo` renderizar o estado de exibição - o padrão é foto.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-157">Set to `initials` or `photo` to render either display state - default is photo.</span></span> |
| <span data-ttu-id="e6a1a-158">modo de exibição</span><span class="sxs-lookup"><span data-stu-id="e6a1a-158">view</span></span>            | <span data-ttu-id="e6a1a-159">modo de exibição</span><span class="sxs-lookup"><span data-stu-id="e6a1a-159">view</span></span>           | <span data-ttu-id="e6a1a-160">Definir para controlar como a pessoa é renderizada.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-160">Set to control how the person is rendered.</span></span> <span data-ttu-id="e6a1a-161">O padrão é `avatar`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-161">Default is `avatar`</span></span> <br /> <span data-ttu-id="e6a1a-162">`avatar` - mostrar somente o avatar</span><span class="sxs-lookup"><span data-stu-id="e6a1a-162">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="e6a1a-163">`oneline` - mostrar avatar e primeira linha ( `displayName` por padrão)</span><span class="sxs-lookup"><span data-stu-id="e6a1a-163">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="e6a1a-164">`twolines` - mostrar avatar e duas linhas de texto ( `displayName` `mail` e por padrão)</span><span class="sxs-lookup"><span data-stu-id="e6a1a-164">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="e6a1a-165">line1-property</span><span class="sxs-lookup"><span data-stu-id="e6a1a-165">line1-property</span></span>  | <span data-ttu-id="e6a1a-166">line1Property</span><span class="sxs-lookup"><span data-stu-id="e6a1a-166">line1Property</span></span>  | <span data-ttu-id="e6a1a-167">Define a propriedade da personDetails a ser usada para a primeira linha de texto.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-167">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="e6a1a-168">O padrão é `displayName`.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-168">Default is `displayName`.</span></span>|
| <span data-ttu-id="e6a1a-169">line2-property</span><span class="sxs-lookup"><span data-stu-id="e6a1a-169">line2-property</span></span>  | <span data-ttu-id="e6a1a-170">line2Property</span><span class="sxs-lookup"><span data-stu-id="e6a1a-170">line2Property</span></span>  | <span data-ttu-id="e6a1a-171">Define a propriedade da personDetails a ser usada para a segunda linha de texto.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-171">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="e6a1a-172">O padrão é `mail`.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-172">Default is `mail`.</span></span>|
| <span data-ttu-id="e6a1a-173">line3-property</span><span class="sxs-lookup"><span data-stu-id="e6a1a-173">line3-property</span></span>  | <span data-ttu-id="e6a1a-174">line3Property</span><span class="sxs-lookup"><span data-stu-id="e6a1a-174">line3Property</span></span>  | <span data-ttu-id="e6a1a-175">Define a propriedade da personDetails a ser usada para a terceira linha de texto.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-175">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="e6a1a-176">O padrão é `jobTitle`.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-176">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="e6a1a-177">show-presence</span><span class="sxs-lookup"><span data-stu-id="e6a1a-177">show-presence</span></span>   | <span data-ttu-id="e6a1a-178">showPresence</span><span class="sxs-lookup"><span data-stu-id="e6a1a-178">showPresence</span></span>   | <span data-ttu-id="e6a1a-179">Definir sinalizador para exibir a presença da pessoa - o padrão é `false` .</span><span class="sxs-lookup"><span data-stu-id="e6a1a-179">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="e6a1a-180">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="e6a1a-180">CSS custom properties</span></span>

<span data-ttu-id="e6a1a-181">O `mgt-person` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-181">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  --avatar-cursor: default;
  
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

<span data-ttu-id="e6a1a-182">Para saber mais, confira [componentes de estilo](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="e6a1a-182">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="e6a1a-183">Eventos</span><span class="sxs-lookup"><span data-stu-id="e6a1a-183">Events</span></span>

<span data-ttu-id="e6a1a-184">Os eventos a seguir são disparados do componente.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-184">The following events are fired from the component.</span></span>

| <span data-ttu-id="e6a1a-185">Event</span><span class="sxs-lookup"><span data-stu-id="e6a1a-185">Event</span></span> | <span data-ttu-id="e6a1a-186">Detalhe</span><span class="sxs-lookup"><span data-stu-id="e6a1a-186">Detail</span></span> | <span data-ttu-id="e6a1a-187">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6a1a-187">Description</span></span> |
| --- | --- | --- |
| `line1clicked` | <span data-ttu-id="e6a1a-188">O detalhe contém o objeto `person` respectivo</span><span class="sxs-lookup"><span data-stu-id="e6a1a-188">The detail contains the respective `person` object</span></span> | <span data-ttu-id="e6a1a-189">Acionado quando a linha1 é clicada.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-189">Fired when line1 is clicked.</span></span> |
| `line2clicked` | <span data-ttu-id="e6a1a-190">O detalhe contém o objeto `person` respectivo</span><span class="sxs-lookup"><span data-stu-id="e6a1a-190">The detail contains the respective `person` object</span></span> | <span data-ttu-id="e6a1a-191">Disparado quando a linha2 é clicada.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-191">Fired when line2 is clicked.</span></span> |
| `line3clicked` | <span data-ttu-id="e6a1a-192">O detalhe contém o objeto `person` respectivo</span><span class="sxs-lookup"><span data-stu-id="e6a1a-192">The detail contains the respective `person` object</span></span> | <span data-ttu-id="e6a1a-193">Acionado quando a linha3 é clicada.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-193">Fired when line3 is clicked.</span></span> |

<span data-ttu-id="e6a1a-194">Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).</span><span class="sxs-lookup"><span data-stu-id="e6a1a-194">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="e6a1a-195">Modelos</span><span class="sxs-lookup"><span data-stu-id="e6a1a-195">Templates</span></span>

<span data-ttu-id="e6a1a-196">O `mgt-person` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-196">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="e6a1a-197">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes:</span><span class="sxs-lookup"><span data-stu-id="e6a1a-197">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="e6a1a-198">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="e6a1a-198">Data type</span></span> | <span data-ttu-id="e6a1a-199">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="e6a1a-199">Data context</span></span> | <span data-ttu-id="e6a1a-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6a1a-200">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="e6a1a-201">loading</span><span class="sxs-lookup"><span data-stu-id="e6a1a-201">loading</span></span> | <span data-ttu-id="e6a1a-202">nenhuma</span><span class="sxs-lookup"><span data-stu-id="e6a1a-202">none</span></span> | <span data-ttu-id="e6a1a-203">O modelo a ser render enquanto o componente está em um estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-203">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="e6a1a-204">no-data</span><span class="sxs-lookup"><span data-stu-id="e6a1a-204">no-data</span></span> | <span data-ttu-id="e6a1a-205">nenhuma</span><span class="sxs-lookup"><span data-stu-id="e6a1a-205">none</span></span> | <span data-ttu-id="e6a1a-206">O modelo a ser renderizar quando nenhuma imagem ou dados de pessoa estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-206">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="e6a1a-207">Padrão.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-207">default</span></span> | <span data-ttu-id="e6a1a-208">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="e6a1a-208">person: The person details object</span></span> <br> <span data-ttu-id="e6a1a-209">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="e6a1a-209">`personImage`: The URL of the image</span></span> <br> <span data-ttu-id="e6a1a-210">`personPresence`: O objeto de detalhes de presença para pessoa</span><span class="sxs-lookup"><span data-stu-id="e6a1a-210">`personPresence`: The presence details object for person</span></span>  | <span data-ttu-id="e6a1a-211">O modelo padrão substitui todo o componente por seu próprio.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-211">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="e6a1a-212">person-card</span><span class="sxs-lookup"><span data-stu-id="e6a1a-212">person-card</span></span> | <span data-ttu-id="e6a1a-213">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="e6a1a-213">person: The person details object</span></span> <br> <span data-ttu-id="e6a1a-214">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="e6a1a-214">`personImage`: The URL of the image</span></span> | <span data-ttu-id="e6a1a-215">O modelo para atualizar o mgt-person-card exibido em foco ou clique.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-215">The template to update the mgt-person-card displayed on hover or click.</span></span> |
| <span data-ttu-id="e6a1a-216">line1</span><span class="sxs-lookup"><span data-stu-id="e6a1a-216">line1</span></span> | <span data-ttu-id="e6a1a-217">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="e6a1a-217">person: The person details object</span></span> | <span data-ttu-id="e6a1a-218">O modelo para a primeira linha de metadados de pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-218">The template for the first line of person metadata.</span></span> |
| <span data-ttu-id="e6a1a-219">line2</span><span class="sxs-lookup"><span data-stu-id="e6a1a-219">line2</span></span> | <span data-ttu-id="e6a1a-220">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="e6a1a-220">person: The person details object</span></span> | <span data-ttu-id="e6a1a-221">O modelo para a segunda linha de metadados de pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-221">The template for the second line of person metadata.</span></span> |
| <span data-ttu-id="e6a1a-222">line3</span><span class="sxs-lookup"><span data-stu-id="e6a1a-222">line3</span></span> | <span data-ttu-id="e6a1a-223">pessoa: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="e6a1a-223">person: The person details object</span></span> | <span data-ttu-id="e6a1a-224">O modelo para a terceira linha de metadados de pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-224">The template for the third line of person metadata.</span></span> |

<span data-ttu-id="e6a1a-225">O exemplo a seguir define um modelo para o componente da pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-225">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="e6a1a-226">Cartão pessoal</span><span class="sxs-lookup"><span data-stu-id="e6a1a-226">Person card</span></span>

<span data-ttu-id="e6a1a-227">O `mgt-person` componente pode mostrar um ao passar o mouse ou `mgt-person-card` clicar.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-227">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="e6a1a-228">Adicionar o controle à página HTML</span><span class="sxs-lookup"><span data-stu-id="e6a1a-228">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="e6a1a-229">Atributo</span><span class="sxs-lookup"><span data-stu-id="e6a1a-229">Attribute</span></span>    |  <span data-ttu-id="e6a1a-230">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6a1a-230">Property</span></span>     | <span data-ttu-id="e6a1a-231">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6a1a-231">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="e6a1a-232">person-card</span><span class="sxs-lookup"><span data-stu-id="e6a1a-232">person-card</span></span> | <span data-ttu-id="e6a1a-233">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="e6a1a-233">personCardInteraction</span></span> | <span data-ttu-id="e6a1a-234">Uma enumeração para determinar a ação do usuário necessária para ativar o painel do sub-sub-plano - `hover` ou `click` .</span><span class="sxs-lookup"><span data-stu-id="e6a1a-234">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="e6a1a-235">O valor padrão é `none`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-235">Default value is `none`</span></span> |


<span data-ttu-id="e6a1a-236">Para obter mais informações sobre a templating, o estilo e os atributos, consulte [Person Card component](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="e6a1a-236">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="e6a1a-237">Configuração de componente global</span><span class="sxs-lookup"><span data-stu-id="e6a1a-237">Global component configuration</span></span>

<span data-ttu-id="e6a1a-238">A `MgtPerson` classe expõe um objeto `config` estático que configura todos os componentes da pessoa no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-238">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="e6a1a-239">O exemplo a seguir mostra como usar o objeto config.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-239">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="e6a1a-240">As propriedades a seguir estão disponíveis no objeto config.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-240">The following properties are available on the config object.</span></span>

| <span data-ttu-id="e6a1a-241">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6a1a-241">Property</span></span> | <span data-ttu-id="e6a1a-242">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6a1a-242">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="e6a1a-243">useContactApis</span><span class="sxs-lookup"><span data-stu-id="e6a1a-243">useContactApis</span></span> | <span data-ttu-id="e6a1a-244">`boolean`- Indica se o componente da pessoa pode usar a API de contatos pessoais da Microsoft Graph para pesquisar detalhes de contato e fotos.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-244">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="e6a1a-245">O valor padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-245">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="e6a1a-246">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e6a1a-246">Microsoft Graph permissions</span></span>

<span data-ttu-id="e6a1a-247">Esse controle usa as seguintes APIs Graph Microsoft e permissões.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-247">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="e6a1a-248">Configuração</span><span class="sxs-lookup"><span data-stu-id="e6a1a-248">Configuration</span></span> | <span data-ttu-id="e6a1a-249">Permissão</span><span class="sxs-lookup"><span data-stu-id="e6a1a-249">Permission</span></span> | <span data-ttu-id="e6a1a-250">API</span><span class="sxs-lookup"><span data-stu-id="e6a1a-250">API</span></span> |
| ------------- | ---------- | --- |
| <span data-ttu-id="e6a1a-251">`personDetails` set without image, `fetchImage` set to , set to , `true` `avatarType` `photo` retrieved person is a contact and `useContactApis` set to `true`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-251">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo`, retrieved person is a contact and `useContactApis` set to `true`</span></span> | <span data-ttu-id="e6a1a-252">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e6a1a-252">Contacts.Read</span></span> | [<span data-ttu-id="e6a1a-253">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="e6a1a-253">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) |
| <span data-ttu-id="e6a1a-254">`personDetails` set without image, `fetchImage` set to , set to and person is not a contact or is set `true` `avatarType` `photo` `useContactApis` to `false`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-254">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and person is not a contact or `useContactApis` is set to `false`</span></span> | <span data-ttu-id="e6a1a-255">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="e6a1a-255">User.ReadBasic.All</span></span> | [<span data-ttu-id="e6a1a-256">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="e6a1a-256">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="e6a1a-257">`personDetails` set without image, `fetchImage` set to , set to and user `true` `avatarType` `photo` specified via email</span><span class="sxs-lookup"><span data-stu-id="e6a1a-257">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and user specified via email</span></span> | <span data-ttu-id="e6a1a-258">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="e6a1a-258">User.ReadBasic.All</span></span> | [<span data-ttu-id="e6a1a-259">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="e6a1a-259">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="e6a1a-260">`personDetails` set without image, `fetchImage` set to , set to and contact `true` `avatarType` `photo` specified via email</span><span class="sxs-lookup"><span data-stu-id="e6a1a-260">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and contact specified via email</span></span> | <span data-ttu-id="e6a1a-261">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e6a1a-261">Contacts.Read</span></span> | [<span data-ttu-id="e6a1a-262">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="e6a1a-262">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) |
| <span data-ttu-id="e6a1a-263">`userId` set</span><span class="sxs-lookup"><span data-stu-id="e6a1a-263">`userId` set</span></span> | <span data-ttu-id="e6a1a-264">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="e6a1a-264">User.ReadBasic.All</span></span> | [<span data-ttu-id="e6a1a-265">/users/{id}</span><span class="sxs-lookup"><span data-stu-id="e6a1a-265">/users/{id}</span></span>](/graph/api/user-list-people) |
| <span data-ttu-id="e6a1a-266">`personQuery` definir como `me` e `avatarType` definir como `photo`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-266">`personQuery` set to `me` and `avatarType` set to `photo`</span></span> | <span data-ttu-id="e6a1a-267">User.Read</span><span class="sxs-lookup"><span data-stu-id="e6a1a-267">User.Read</span></span> | [<span data-ttu-id="e6a1a-268">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="e6a1a-268">/me/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="e6a1a-269">`personQuery` definir para `me` e definir para outra coisa que `avatarType` não `photo`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-269">`personQuery` set to `me` and `avatarType` set to something else than `photo`</span></span> | <span data-ttu-id="e6a1a-270">User.Read</span><span class="sxs-lookup"><span data-stu-id="e6a1a-270">User.Read</span></span> | [<span data-ttu-id="e6a1a-271">/me</span><span class="sxs-lookup"><span data-stu-id="e6a1a-271">/me</span></span>](/graph/api/user-get) |
| <span data-ttu-id="e6a1a-272">`personQuery` definido como um valor diferente `me` e `useContactApis` definido como `true`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-272">`personQuery` set to a value other than `me` and `useContactApis` set to `true`</span></span> | <span data-ttu-id="e6a1a-273">People.Read, User.ReadBasic.All, Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e6a1a-273">People.Read, User.ReadBasic.All, Contacts.Read</span></span> | <span data-ttu-id="e6a1a-274">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people), [/me/contacts/ \* ](/graph/api/user-list-contacts)</span><span class="sxs-lookup"><span data-stu-id="e6a1a-274">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people), [/me/contacts/\*](/graph/api/user-list-contacts)</span></span> |
| <span data-ttu-id="e6a1a-275">`personQuery` definido como um valor diferente `me` e `useContactApis` definido como `false`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-275">`personQuery` set to a value other than `me` and `useContactApis` set to `false`</span></span> | <span data-ttu-id="e6a1a-276">People.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="e6a1a-276">People.Read, User.ReadBasic.All</span></span> | <span data-ttu-id="e6a1a-277">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people)</span><span class="sxs-lookup"><span data-stu-id="e6a1a-277">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people)</span></span> |
| <span data-ttu-id="e6a1a-278">`showPresence` definir como `true` e `personQuery` definir como `me`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-278">`showPresence` set to `true` and `personQuery` set to `me`</span></span> | <span data-ttu-id="e6a1a-279">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="e6a1a-279">Presence.Read</span></span> | [<span data-ttu-id="e6a1a-280">/me/presence</span><span class="sxs-lookup"><span data-stu-id="e6a1a-280">/me/presence</span></span>](/graph/api/presence-get) |
| <span data-ttu-id="e6a1a-281">`showPresence` definir como `true` e definir como um valor `personQuery` diferente `me`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-281">`showPresence` set to `true` and `personQuery` set to a value other than `me`</span></span> | <span data-ttu-id="e6a1a-282">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6a1a-282">Presence.Read.All</span></span> | [<span data-ttu-id="e6a1a-283">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="e6a1a-283">/users/{id}/presence</span></span>](/graph/api/presence-get) |
| <span data-ttu-id="e6a1a-284">`personCardInteraction` definido como um valor diferente de `PersonCardInteraction.none`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-284">`personCardInteraction` set to a value other than `PersonCardInteraction.none`</span></span> | <span data-ttu-id="e6a1a-285">Consulte [permissões de cartão de pessoa](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="e6a1a-285">See [person card permissions](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span></span> | <span data-ttu-id="e6a1a-286">Consulte [chamadas de API de cartão de pessoa](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="e6a1a-286">See [person card API calls](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span></span> |

## <a name="authentication"></a><span data-ttu-id="e6a1a-287">Autenticação</span><span class="sxs-lookup"><span data-stu-id="e6a1a-287">Authentication</span></span>

<span data-ttu-id="e6a1a-288">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md) para buscar os dados necessários.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-288">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="e6a1a-289">Cache</span><span class="sxs-lookup"><span data-stu-id="e6a1a-289">Cache</span></span>

|<span data-ttu-id="e6a1a-290">Armazenamento de objetos</span><span class="sxs-lookup"><span data-stu-id="e6a1a-290">Object store</span></span>|<span data-ttu-id="e6a1a-291">Dados armazenados em cache</span><span class="sxs-lookup"><span data-stu-id="e6a1a-291">Cached data</span></span>|<span data-ttu-id="e6a1a-292">Comentários</span><span class="sxs-lookup"><span data-stu-id="e6a1a-292">Remarks</span></span>|
|---------|-----------|-------|
|`photos`|<span data-ttu-id="e6a1a-293">Foto da pessoa</span><span class="sxs-lookup"><span data-stu-id="e6a1a-293">Person's photo</span></span>|<span data-ttu-id="e6a1a-294">Usado, quando `avatarType` é definido como e é definido `photo` `fetchImage` como `true`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-294">Used, when `avatarType` is set to `photo` and `fetchImage` is set to `true`</span></span>|
|`presence`|<span data-ttu-id="e6a1a-295">Presença da pessoa</span><span class="sxs-lookup"><span data-stu-id="e6a1a-295">Person's presence</span></span>|<span data-ttu-id="e6a1a-296">Usado, quando `showPresence` está definido como `true`</span><span class="sxs-lookup"><span data-stu-id="e6a1a-296">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="e6a1a-297">Informações do usuário da pessoa</span><span class="sxs-lookup"><span data-stu-id="e6a1a-297">Person's user information</span></span>|

<span data-ttu-id="e6a1a-298">Consulte [Caching](../customize-components/cache.md) para obter mais detalhes sobre como configurar o cache.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-298">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="e6a1a-299">Estender para obter mais controle</span><span class="sxs-lookup"><span data-stu-id="e6a1a-299">Extend for more control</span></span>

<span data-ttu-id="e6a1a-300">Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-300">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="e6a1a-301">Método</span><span class="sxs-lookup"><span data-stu-id="e6a1a-301">Method</span></span> | <span data-ttu-id="e6a1a-302">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6a1a-302">Description</span></span> |
| - | - |
| <span data-ttu-id="e6a1a-303">renderLoading</span><span class="sxs-lookup"><span data-stu-id="e6a1a-303">renderLoading</span></span> | <span data-ttu-id="e6a1a-304">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-304">Renders the loading state.</span></span> |
| <span data-ttu-id="e6a1a-305">renderNoData</span><span class="sxs-lookup"><span data-stu-id="e6a1a-305">renderNoData</span></span> | <span data-ttu-id="e6a1a-306">Renderiza quando nenhum dado de imagem ou pessoa está disponível.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-306">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="e6a1a-307">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="e6a1a-307">renderAvatar</span></span> | <span data-ttu-id="e6a1a-308">Renderiza o avatar.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-308">Renders the avatar.</span></span> |
| <span data-ttu-id="e6a1a-309">renderDetails</span><span class="sxs-lookup"><span data-stu-id="e6a1a-309">renderDetails</span></span> | <span data-ttu-id="e6a1a-310">Renderiza a parte de detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="e6a1a-310">Renders the person details part.</span></span> |
