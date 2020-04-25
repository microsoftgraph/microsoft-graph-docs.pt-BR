---
title: Componente Person no Microsoft Graph Toolkit
description: O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: a23d5432c868881f05c04b84626962d684f7d1eb
ms.sourcegitcommit: d2536f56e3a424219660bc0495ec8632932b4fb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2020
ms.locfileid: "43812545"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="ccfcf-103">Componente Person no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="ccfcf-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ccfcf-104">O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span>

<span data-ttu-id="ccfcf-105">O componente pessoa também usa a [pessoa de gerenciamento de pessoas](./person-card.md) para exibir um cartão de submenu com informações adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="ccfcf-106">Para obter detalhes, consulte a seção [cartão de pessoa](#person-card) .</span><span class="sxs-lookup"><span data-stu-id="ccfcf-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="ccfcf-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ccfcf-107">Example</span></span>

<span data-ttu-id="ccfcf-108">O exemplo a seguir exibe uma pessoa usando `mgt-person` o componente.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="ccfcf-109">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="ccfcf-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="ccfcf-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="ccfcf-111">Configurando os detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="ccfcf-111">Setting the person details</span></span>

<span data-ttu-id="ccfcf-112">Você pode usar três propriedades para definir os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="ccfcf-113">Use apenas uma das seguintes propriedades por instância:</span><span class="sxs-lookup"><span data-stu-id="ccfcf-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="ccfcf-114">Defina o `user-id` atributo ou `userId` a propriedade para buscar o usuário do Microsoft Graph usando sua ID.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="ccfcf-115">Definir o `person-query` atributo ou `personQuery` a propriedade para pesquisar o Microsoft Graph em uma determinada pessoa.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="ccfcf-116">Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="ccfcf-117">Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="ccfcf-118">Defina o `person-details` atributo ou `personDetails` a propriedade para definir manualmente os detalhes da pessoa, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-118">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="ccfcf-119">Se nenhuma imagem for fornecida, uma será buscada (se disponível).</span><span class="sxs-lookup"><span data-stu-id="ccfcf-119">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="ccfcf-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccfcf-120">Properties</span></span>

<span data-ttu-id="ccfcf-121">Você pode usar várias propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-121">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="ccfcf-122">Atributo</span><span class="sxs-lookup"><span data-stu-id="ccfcf-122">Attribute</span></span>    | <span data-ttu-id="ccfcf-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccfcf-123">Property</span></span>   | <span data-ttu-id="ccfcf-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccfcf-124">Description</span></span>                                                   |
| -----------  | ---------- | ------------------------------------------------------------- |
| <span data-ttu-id="ccfcf-125">show-Name</span><span class="sxs-lookup"><span data-stu-id="ccfcf-125">show-name</span></span>    | <span data-ttu-id="ccfcf-126">Nome do mesmo</span><span class="sxs-lookup"><span data-stu-id="ccfcf-126">showName</span></span>   | <span data-ttu-id="ccfcf-127">Definir sinalizador para exibir o nome de exibição da pessoa `false`-o padrão é.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-127">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="ccfcf-128">Mostrar-email</span><span class="sxs-lookup"><span data-stu-id="ccfcf-128">show-email</span></span>   | <span data-ttu-id="ccfcf-129">Enviar email</span><span class="sxs-lookup"><span data-stu-id="ccfcf-129">showEmail</span></span>  | <span data-ttu-id="ccfcf-130">Definir sinalizador para exibir o email da pessoa- `false`o padrão é.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-130">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="ccfcf-131">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="ccfcf-131">CSS custom properties</span></span>

<span data-ttu-id="ccfcf-132">O `mgt-person` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-132">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size-s: 24px;
  --avatar-size: 48px; // avatar size when both name and email are shown
  --avatar-font-size--s: 16px;
  --avatar-font-size: 32px; // font-size when both name and email are shown
  --avatar-border: 0;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-size: 12px;
  --font-weight: 500;
  --color: black;
  --email-font-size: 12px;
  --email-color: black;
}
```

<span data-ttu-id="ccfcf-133">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="ccfcf-133">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="ccfcf-134">Modelos</span><span class="sxs-lookup"><span data-stu-id="ccfcf-134">Templates</span></span>

<span data-ttu-id="ccfcf-135">O `mgt-person` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-135">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="ccfcf-136">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="ccfcf-136">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="ccfcf-137">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="ccfcf-137">Data type</span></span> | <span data-ttu-id="ccfcf-138">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="ccfcf-138">Data context</span></span> | <span data-ttu-id="ccfcf-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccfcf-139">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="ccfcf-140">carregando</span><span class="sxs-lookup"><span data-stu-id="ccfcf-140">loading</span></span> | <span data-ttu-id="ccfcf-141">nenhuma</span><span class="sxs-lookup"><span data-stu-id="ccfcf-141">none</span></span> | <span data-ttu-id="ccfcf-142">O modelo a ser renderizado enquanto o componente está em um estado laoding.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-142">The template to render while the component is in a laoding state.</span></span> |
| <span data-ttu-id="ccfcf-143">sem dados</span><span class="sxs-lookup"><span data-stu-id="ccfcf-143">no-data</span></span> | <span data-ttu-id="ccfcf-144">nenhuma</span><span class="sxs-lookup"><span data-stu-id="ccfcf-144">none</span></span> | <span data-ttu-id="ccfcf-145">O modelo a ser renderizado quando nenhuma imagem de pessoa ou dados estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-145">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="ccfcf-146">Padrão.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-146">default</span></span> | <span data-ttu-id="ccfcf-147">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="ccfcf-147">person: The person details object</span></span> <br> <span data-ttu-id="ccfcf-148">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="ccfcf-148">`personImage`: The URL of the image</span></span> | <span data-ttu-id="ccfcf-149">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-149">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="ccfcf-150">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="ccfcf-150">person-card</span></span> | <span data-ttu-id="ccfcf-151">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="ccfcf-151">person: The person details object</span></span> <br> <span data-ttu-id="ccfcf-152">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="ccfcf-152">`personImage`: The URL of the image</span></span> | <span data-ttu-id="ccfcf-153">O modelo para atualizar o item de gerenciamento de pessoa que é exibido ao focalizar ou clique.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-153">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="ccfcf-154">O exemplo a seguir define um modelo para o componente Person.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-154">The following example defines a template for the person component.</span></span>

```html
<mgt-person>
  <template>
    <div data-if="person.image">
      <img src="{{person.image}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a><span data-ttu-id="ccfcf-155">Cartão Pessoal</span><span class="sxs-lookup"><span data-stu-id="ccfcf-155">Person Card</span></span>

<span data-ttu-id="ccfcf-156">O `mgt-person` componente pode mostrar um `mgt-person-card` em foco ou clique.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-156">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="ccfcf-157">Adicionar o controle à página HTML</span><span class="sxs-lookup"><span data-stu-id="ccfcf-157">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="ccfcf-158">Atributo</span><span class="sxs-lookup"><span data-stu-id="ccfcf-158">Attribute</span></span>    |  <span data-ttu-id="ccfcf-159">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccfcf-159">Property</span></span>     | <span data-ttu-id="ccfcf-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccfcf-160">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="ccfcf-161">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="ccfcf-161">person-card</span></span> | <span data-ttu-id="ccfcf-162">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="ccfcf-162">personCardInteraction</span></span> | <span data-ttu-id="ccfcf-163">Uma enumeração para determinar a ação do usuário necessária para ativar o `hover` painel `click`ou o menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-163">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="ccfcf-164">O valor padrão é`none`</span><span class="sxs-lookup"><span data-stu-id="ccfcf-164">Default value is `none`</span></span> |


<span data-ttu-id="ccfcf-165">Para obter mais informações sobre modelos, estilos e atributos, consulte [componente de cartão de pessoa](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="ccfcf-165">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="ccfcf-166">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ccfcf-166">Microsoft Graph permissions</span></span>

<span data-ttu-id="ccfcf-167">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-167">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="ccfcf-168">Resource</span><span class="sxs-lookup"><span data-stu-id="ccfcf-168">Resource</span></span>                                                                                                    | <span data-ttu-id="ccfcf-169">Permissão</span><span class="sxs-lookup"><span data-stu-id="ccfcf-169">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="ccfcf-170">/me</span><span class="sxs-lookup"><span data-stu-id="ccfcf-170">/me</span></span>](/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="ccfcf-171">User.Read</span><span class="sxs-lookup"><span data-stu-id="ccfcf-171">User.Read</span></span>          |
| [<span data-ttu-id="ccfcf-172">$value/me/Photo/</span><span class="sxs-lookup"><span data-stu-id="ccfcf-172">/me/photo/$value</span></span>](/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="ccfcf-173">User.Read</span><span class="sxs-lookup"><span data-stu-id="ccfcf-173">User.Read</span></span>          |
| [<span data-ttu-id="ccfcf-174">/me/People/? $search =</span><span class="sxs-lookup"><span data-stu-id="ccfcf-174">/me/people/?$search=</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="ccfcf-175">People.Read</span><span class="sxs-lookup"><span data-stu-id="ccfcf-175">People.Read</span></span>        |
| [<span data-ttu-id="ccfcf-176">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="ccfcf-176">/me/contacts/\*</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="ccfcf-177">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ccfcf-177">Contacts.Read</span></span>      |
| [<span data-ttu-id="ccfcf-178">$value/Users/{ID}/Photo/</span><span class="sxs-lookup"><span data-stu-id="ccfcf-178">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="ccfcf-179">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="ccfcf-179">User.ReadBasic.All</span></span> |

> <span data-ttu-id="ccfcf-180">**Observação:** para acessar os `*/photo/$value` recursos para contas pessoais da Microsoft, use o ponto de extremidade beta do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-180">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="ccfcf-181">Autenticação</span><span class="sxs-lookup"><span data-stu-id="ccfcf-181">Authentication</span></span>

<span data-ttu-id="ccfcf-182">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md) para buscar os dados necessários.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-182">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="ccfcf-183">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="ccfcf-183">Extend for more control</span></span>

<span data-ttu-id="ccfcf-184">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-184">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="ccfcf-185">Método</span><span class="sxs-lookup"><span data-stu-id="ccfcf-185">Method</span></span> | <span data-ttu-id="ccfcf-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccfcf-186">Description</span></span> |
| - | - |
| <span data-ttu-id="ccfcf-187">renderLoading</span><span class="sxs-lookup"><span data-stu-id="ccfcf-187">renderLoading</span></span> | <span data-ttu-id="ccfcf-188">Renderiza o estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-188">Renders the loading state.</span></span> |
| <span data-ttu-id="ccfcf-189">renderImage</span><span class="sxs-lookup"><span data-stu-id="ccfcf-189">renderImage</span></span> | <span data-ttu-id="ccfcf-190">Renderiza a parte da imagem.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-190">Renders the image part.</span></span> |
| <span data-ttu-id="ccfcf-191">renderNoData</span><span class="sxs-lookup"><span data-stu-id="ccfcf-191">renderNoData</span></span> | <span data-ttu-id="ccfcf-192">Renderiza quando nenhum dado de imagem ou pessoa está disponível.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-192">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="ccfcf-193">renderDetails</span><span class="sxs-lookup"><span data-stu-id="ccfcf-193">renderDetails</span></span> | <span data-ttu-id="ccfcf-194">Renderiza a parte de detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-194">Renders the person details part.</span></span> |
| <span data-ttu-id="ccfcf-195">renderEmail</span><span class="sxs-lookup"><span data-stu-id="ccfcf-195">renderEmail</span></span> | <span data-ttu-id="ccfcf-196">Renderiza a subparte de email dos detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-196">Renders the email sub-part of the person details.</span></span> |
| <span data-ttu-id="ccfcf-197">rendername</span><span class="sxs-lookup"><span data-stu-id="ccfcf-197">renderName</span></span> | <span data-ttu-id="ccfcf-198">Renderiza o nome subparte dos detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="ccfcf-198">Renders the name sub-part of the person details.</span></span> |
