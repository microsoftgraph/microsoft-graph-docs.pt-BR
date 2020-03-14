---
title: Componente Person no Microsoft Graph Toolkit
description: O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0202d8bc8c8ae23f98cb4add9f9d5ca96afea04d
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639951"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="5fb3b-103">Componente Person no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="5fb3b-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="5fb3b-104">O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span>

<span data-ttu-id="5fb3b-105">O componente pessoa também usa a [pessoa de gerenciamento de pessoas](./person-card.md) para exibir um cartão de submenu com informações adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="5fb3b-106">Para obter detalhes, consulte a seção [cartão de pessoa](#person-card) .</span><span class="sxs-lookup"><span data-stu-id="5fb3b-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="5fb3b-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5fb3b-107">Example</span></span>

<span data-ttu-id="5fb3b-108">O exemplo a seguir exibe uma pessoa usando `mgt-person` o componente.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="5fb3b-109">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="5fb3b-110">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="5fb3b-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="5fb3b-111">Configurando os detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="5fb3b-111">Setting the person details</span></span>

<span data-ttu-id="5fb3b-112">Você pode usar três propriedades para definir os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="5fb3b-113">Use apenas uma das seguintes propriedades por instância:</span><span class="sxs-lookup"><span data-stu-id="5fb3b-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="5fb3b-114">Defina o `user-id` atributo ou `userId` a propriedade para buscar o usuário do Microsoft Graph usando sua ID.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="5fb3b-115">Definir o `person-query` atributo ou `personQuery` a propriedade para pesquisar o Microsoft Graph em uma determinada pessoa.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="5fb3b-116">Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="5fb3b-117">Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="5fb3b-118">Defina o `person-details` atributo ou `personDetails` a propriedade para definir manualmente os detalhes da pessoa, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-118">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="5fb3b-119">Se nenhuma imagem for fornecida, uma será buscada (se disponível).</span><span class="sxs-lookup"><span data-stu-id="5fb3b-119">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="5fb3b-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5fb3b-120">Properties</span></span>

<span data-ttu-id="5fb3b-121">Você pode usar várias propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-121">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="5fb3b-122">Atributo</span><span class="sxs-lookup"><span data-stu-id="5fb3b-122">Attribute</span></span>    | <span data-ttu-id="5fb3b-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fb3b-123">Property</span></span>   | <span data-ttu-id="5fb3b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fb3b-124">Description</span></span>                                                   |
| -----------  | ---------- | ------------------------------------------------------------- |
| <span data-ttu-id="5fb3b-125">show-Name</span><span class="sxs-lookup"><span data-stu-id="5fb3b-125">show-name</span></span>    | <span data-ttu-id="5fb3b-126">Nome do mesmo</span><span class="sxs-lookup"><span data-stu-id="5fb3b-126">showName</span></span>   | <span data-ttu-id="5fb3b-127">Definir sinalizador para exibir o nome de exibição da pessoa `false`-o padrão é.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-127">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="5fb3b-128">Mostrar-email</span><span class="sxs-lookup"><span data-stu-id="5fb3b-128">show-email</span></span>   | <span data-ttu-id="5fb3b-129">Enviar email</span><span class="sxs-lookup"><span data-stu-id="5fb3b-129">showEmail</span></span>  | <span data-ttu-id="5fb3b-130">Definir sinalizador para exibir o email da pessoa- `false`o padrão é.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-130">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="5fb3b-131">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="5fb3b-131">CSS custom properties</span></span>

<span data-ttu-id="5fb3b-132">O `mgt-person` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-132">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="5fb3b-133">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="5fb3b-133">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="5fb3b-134">Modelos</span><span class="sxs-lookup"><span data-stu-id="5fb3b-134">Templates</span></span>

<span data-ttu-id="5fb3b-135">O `mgt-person` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-135">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="5fb3b-136">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="5fb3b-136">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="5fb3b-137">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="5fb3b-137">Data type</span></span>     | <span data-ttu-id="5fb3b-138">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="5fb3b-138">Data context</span></span>              | <span data-ttu-id="5fb3b-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fb3b-139">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="5fb3b-140">Padrão.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-140">default</span></span>     | <span data-ttu-id="5fb3b-141">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="5fb3b-141">person: The person details object</span></span> <br> <span data-ttu-id="5fb3b-142">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="5fb3b-142">`personImage`: The URL of the image</span></span> | <span data-ttu-id="5fb3b-143">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-143">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="5fb3b-144">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="5fb3b-144">person-card</span></span> | <span data-ttu-id="5fb3b-145">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="5fb3b-145">person: The person details object</span></span> <br> <span data-ttu-id="5fb3b-146">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="5fb3b-146">`personImage`: The URL of the image</span></span> | <span data-ttu-id="5fb3b-147">O modelo para atualizar o item de gerenciamento de pessoa que é exibido ao focalizar ou clique.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-147">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="5fb3b-148">O exemplo a seguir define um modelo para o componente Person.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-148">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="5fb3b-149">Cartão Pessoal</span><span class="sxs-lookup"><span data-stu-id="5fb3b-149">Person Card</span></span>

<span data-ttu-id="5fb3b-150">O `mgt-person` componente pode mostrar um `mgt-person-card` em foco ou clique.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-150">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="5fb3b-151">Adicionar o controle à página HTML</span><span class="sxs-lookup"><span data-stu-id="5fb3b-151">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="5fb3b-152">Atributo</span><span class="sxs-lookup"><span data-stu-id="5fb3b-152">Attribute</span></span>    |  <span data-ttu-id="5fb3b-153">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fb3b-153">Property</span></span>     | <span data-ttu-id="5fb3b-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fb3b-154">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="5fb3b-155">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="5fb3b-155">person-card</span></span> | <span data-ttu-id="5fb3b-156">personCard</span><span class="sxs-lookup"><span data-stu-id="5fb3b-156">personCard</span></span> | <span data-ttu-id="5fb3b-157">Uma enumeração para determinar a ação do usuário necessária para ativar o `hover` painel `click`ou o menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-157">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="5fb3b-158">O valor padrão é`none`</span><span class="sxs-lookup"><span data-stu-id="5fb3b-158">Default value is `none`</span></span> |


<span data-ttu-id="5fb3b-159">Para obter mais informações sobre modelos, estilos e atributos, consulte [componente de cartão de pessoa](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="5fb3b-159">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="5fb3b-160">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5fb3b-160">Microsoft Graph permissions</span></span>

<span data-ttu-id="5fb3b-161">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-161">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="5fb3b-162">Resource</span><span class="sxs-lookup"><span data-stu-id="5fb3b-162">Resource</span></span>                                                                                                    | <span data-ttu-id="5fb3b-163">Permissão</span><span class="sxs-lookup"><span data-stu-id="5fb3b-163">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="5fb3b-164">/me</span><span class="sxs-lookup"><span data-stu-id="5fb3b-164">/me</span></span>](/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="5fb3b-165">User.Read</span><span class="sxs-lookup"><span data-stu-id="5fb3b-165">User.Read</span></span>          |
| [<span data-ttu-id="5fb3b-166">$value/me/Photo/</span><span class="sxs-lookup"><span data-stu-id="5fb3b-166">/me/photo/$value</span></span>](/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="5fb3b-167">User.Read</span><span class="sxs-lookup"><span data-stu-id="5fb3b-167">User.Read</span></span>          |
| [<span data-ttu-id="5fb3b-168">/me/People/? $search =</span><span class="sxs-lookup"><span data-stu-id="5fb3b-168">/me/people/?$search=</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="5fb3b-169">People.Read</span><span class="sxs-lookup"><span data-stu-id="5fb3b-169">People.Read</span></span>        |
| [<span data-ttu-id="5fb3b-170">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="5fb3b-170">/me/contacts/\*</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="5fb3b-171">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5fb3b-171">Contacts.Read</span></span>      |
| [<span data-ttu-id="5fb3b-172">$value/Users/{ID}/Photo/</span><span class="sxs-lookup"><span data-stu-id="5fb3b-172">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="5fb3b-173">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="5fb3b-173">User.ReadBasic.All</span></span> |

> <span data-ttu-id="5fb3b-174">**Observação:** para acessar os `*/photo/$value` recursos para contas pessoais da Microsoft, use o ponto de extremidade beta do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-174">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="5fb3b-175">Autenticação</span><span class="sxs-lookup"><span data-stu-id="5fb3b-175">Authentication</span></span>

<span data-ttu-id="5fb3b-176">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md) para buscar os dados necessários.</span><span class="sxs-lookup"><span data-stu-id="5fb3b-176">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
