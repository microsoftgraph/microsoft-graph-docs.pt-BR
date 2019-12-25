---
title: Componente Person no Microsoft Graph Toolkit
description: O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 8a0498203296f3880741a4bc2cc53ffd69aff518
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866872"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="1d4e8-103">Componente Person no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="1d4e8-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1d4e8-104">O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span>

<span data-ttu-id="1d4e8-105">O componente pessoa também usa a [pessoa de gerenciamento de pessoas](./person-card.md) para exibir um cartão de submenu com informações adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="1d4e8-106">Para obter detalhes, consulte a seção [cartão de pessoa](#person-card) .</span><span class="sxs-lookup"><span data-stu-id="1d4e8-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="1d4e8-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d4e8-107">Example</span></span>

[<span data-ttu-id="1d4e8-108">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="1d4e8-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="1d4e8-109">Adicionar o controle à página HTML</span><span class="sxs-lookup"><span data-stu-id="1d4e8-109">Add the control to the HTML page</span></span>
```html
<mgt-person person-query=""></mgt-person>
```

## <a name="setting-the-person-details"></a><span data-ttu-id="1d4e8-110">Configurando os detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="1d4e8-110">Setting the person details</span></span>

<span data-ttu-id="1d4e8-111">Você pode usar três propriedades para definir os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-111">You can use three properties to set the person details.</span></span> <span data-ttu-id="1d4e8-112">Use apenas uma das seguintes propriedades por instância:</span><span class="sxs-lookup"><span data-stu-id="1d4e8-112">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="1d4e8-113">Defina o `user-id` atributo ou `userId` a propriedade para buscar o usuário do Microsoft Graph usando sua ID.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-113">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="1d4e8-114">Definir o `person-query` atributo ou `personQuery` a propriedade para pesquisar o Microsoft Graph em uma determinada pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-114">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="1d4e8-115">Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-115">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="1d4e8-116">Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-116">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="1d4e8-117">Defina o `person-details` atributo ou `personDetails` a propriedade para definir manualmente os detalhes da pessoa, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-117">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="1d4e8-118">Se nenhuma imagem for fornecida, uma será buscada (se disponível).</span><span class="sxs-lookup"><span data-stu-id="1d4e8-118">If no image is provided, one will be fetched (if available).</span></span>

## <a name="changing-how-the-component-looks"></a><span data-ttu-id="1d4e8-119">Alterar a aparência do componente</span><span class="sxs-lookup"><span data-stu-id="1d4e8-119">Changing how the component looks</span></span>

<span data-ttu-id="1d4e8-120">Você pode usar várias propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-120">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="1d4e8-121">Atributo</span><span class="sxs-lookup"><span data-stu-id="1d4e8-121">Attribute</span></span>    | <span data-ttu-id="1d4e8-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d4e8-122">Property</span></span>   | <span data-ttu-id="1d4e8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d4e8-123">Description</span></span>                                                   |
| -----------  | ---------- | ------------------------------------------------------------- |
| <span data-ttu-id="1d4e8-124">show-Name</span><span class="sxs-lookup"><span data-stu-id="1d4e8-124">show-name</span></span>    | <span data-ttu-id="1d4e8-125">Nome do mesmo</span><span class="sxs-lookup"><span data-stu-id="1d4e8-125">showName</span></span>   | <span data-ttu-id="1d4e8-126">Definir sinalizador para exibir o nome de exibição da pessoa `false`-o padrão é.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-126">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="1d4e8-127">Mostrar-email</span><span class="sxs-lookup"><span data-stu-id="1d4e8-127">show-email</span></span>   | <span data-ttu-id="1d4e8-128">Enviar email</span><span class="sxs-lookup"><span data-stu-id="1d4e8-128">showEmail</span></span>  | <span data-ttu-id="1d4e8-129">Definir sinalizador para exibir o email da pessoa- `false`o padrão é.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-129">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="1d4e8-130">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="1d4e8-130">CSS custom properties</span></span>

<span data-ttu-id="1d4e8-131">O `mgt-person` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-131">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="1d4e8-132">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="1d4e8-132">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="1d4e8-133">Modelos</span><span class="sxs-lookup"><span data-stu-id="1d4e8-133">Templates</span></span>

<span data-ttu-id="1d4e8-134">O `mgt-person` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-134">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="1d4e8-135">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="1d4e8-135">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="1d4e8-136">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="1d4e8-136">Data type</span></span>     | <span data-ttu-id="1d4e8-137">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="1d4e8-137">Data context</span></span>              | <span data-ttu-id="1d4e8-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d4e8-138">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="1d4e8-139">Padrão.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-139">default</span></span>     | <span data-ttu-id="1d4e8-140">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="1d4e8-140">person: The person details object</span></span> <br> <span data-ttu-id="1d4e8-141">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="1d4e8-141">`personImage`: The URL of the image</span></span> | <span data-ttu-id="1d4e8-142">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-142">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="1d4e8-143">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="1d4e8-143">person-card</span></span> | <span data-ttu-id="1d4e8-144">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="1d4e8-144">person: The person details object</span></span> <br> <span data-ttu-id="1d4e8-145">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="1d4e8-145">`personImage`: The URL of the image</span></span> | <span data-ttu-id="1d4e8-146">O modelo para atualizar o item de gerenciamento de pessoa que é exibido ao focalizar ou clique.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-146">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="1d4e8-147">O exemplo a seguir define um modelo para o componente Person.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-147">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="1d4e8-148">Cartão Pessoal</span><span class="sxs-lookup"><span data-stu-id="1d4e8-148">Person Card</span></span>

<span data-ttu-id="1d4e8-149">O `mgt-person` componente pode mostrar um `mgt-person-card` em foco ou clique.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-149">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="1d4e8-150">Adicionar o controle à página HTML</span><span class="sxs-lookup"><span data-stu-id="1d4e8-150">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="1d4e8-151">Atributo</span><span class="sxs-lookup"><span data-stu-id="1d4e8-151">Attribute</span></span>    |  <span data-ttu-id="1d4e8-152">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d4e8-152">Property</span></span>     | <span data-ttu-id="1d4e8-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d4e8-153">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="1d4e8-154">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="1d4e8-154">person-card</span></span> | <span data-ttu-id="1d4e8-155">personCard</span><span class="sxs-lookup"><span data-stu-id="1d4e8-155">personCard</span></span> | <span data-ttu-id="1d4e8-156">Uma enumeração para determinar a ação do usuário necessária para ativar o `hover` painel `click`ou o menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-156">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="1d4e8-157">O valor padrão é`none`</span><span class="sxs-lookup"><span data-stu-id="1d4e8-157">Default value is `none`</span></span> |


<span data-ttu-id="1d4e8-158">Para obter mais informações sobre modelos, estilos e atributos, consulte [componente de cartão de pessoa](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="1d4e8-158">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="1d4e8-159">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1d4e8-159">Microsoft Graph permissions</span></span>

<span data-ttu-id="1d4e8-160">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-160">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="1d4e8-161">Recurso</span><span class="sxs-lookup"><span data-stu-id="1d4e8-161">Resource</span></span>                                                                                                    | <span data-ttu-id="1d4e8-162">Permissão</span><span class="sxs-lookup"><span data-stu-id="1d4e8-162">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="1d4e8-163">/me</span><span class="sxs-lookup"><span data-stu-id="1d4e8-163">/me</span></span>](/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="1d4e8-164">User.Read</span><span class="sxs-lookup"><span data-stu-id="1d4e8-164">User.Read</span></span>          |
| [<span data-ttu-id="1d4e8-165">$value/me/Photo/</span><span class="sxs-lookup"><span data-stu-id="1d4e8-165">/me/photo/$value</span></span>](/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="1d4e8-166">User.Read</span><span class="sxs-lookup"><span data-stu-id="1d4e8-166">User.Read</span></span>          |
| [<span data-ttu-id="1d4e8-167">/me/People/? $search =</span><span class="sxs-lookup"><span data-stu-id="1d4e8-167">/me/people/?$search=</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="1d4e8-168">People.Read</span><span class="sxs-lookup"><span data-stu-id="1d4e8-168">People.Read</span></span>        |
| [<span data-ttu-id="1d4e8-169">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="1d4e8-169">/me/contacts/\*</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="1d4e8-170">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1d4e8-170">Contacts.Read</span></span>      |
| [<span data-ttu-id="1d4e8-171">$value/Users/{ID}/Photo/</span><span class="sxs-lookup"><span data-stu-id="1d4e8-171">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="1d4e8-172">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="1d4e8-172">User.ReadBasic.All</span></span> |

> <span data-ttu-id="1d4e8-173">**Observação:** para acessar os `*/photo/$value` recursos para contas pessoais da Microsoft, use o ponto de extremidade beta do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-173">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="1d4e8-174">Autenticação</span><span class="sxs-lookup"><span data-stu-id="1d4e8-174">Authentication</span></span>

<span data-ttu-id="1d4e8-175">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md) para buscar os dados necessários.</span><span class="sxs-lookup"><span data-stu-id="1d4e8-175">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
