---
title: Componente Person no Microsoft Graph Toolkit
description: O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b4664cf545c858dbb2d49ad5191ab7cf5118092e
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275700"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="43916-103">Componente Person no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="43916-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="43916-104">O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="43916-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span> 

<span data-ttu-id="43916-105">O componente pessoa também usa a [pessoa de gerenciamento de pessoas](./person-card.md) para exibir um cartão de submenu com informações adicionais sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="43916-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="43916-106">Para obter detalhes, consulte a seção [cartão de pessoa](#person-card) .</span><span class="sxs-lookup"><span data-stu-id="43916-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="43916-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43916-107">Example</span></span>

[<span data-ttu-id="43916-108">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="43916-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="43916-109">Adicionar o controle à página HTML</span><span class="sxs-lookup"><span data-stu-id="43916-109">Add the control to the HTML page</span></span>
```html
<mgt-person person-query=""></mgt-person>
```

## <a name="setting-the-person-details"></a><span data-ttu-id="43916-110">Configurando os detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="43916-110">Setting the person details</span></span>

<span data-ttu-id="43916-111">Você pode usar três propriedades para definir os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="43916-111">You can use three properties to set the person details.</span></span> <span data-ttu-id="43916-112">Use apenas uma das seguintes propriedades por instância:</span><span class="sxs-lookup"><span data-stu-id="43916-112">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="43916-113">Defina o `user-id` atributo ou `userId` a propriedade para buscar o usuário do Microsoft Graph usando sua ID.</span><span class="sxs-lookup"><span data-stu-id="43916-113">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>  

* <span data-ttu-id="43916-114">Definir o `person-query` atributo ou `personQuery` a propriedade para pesquisar o Microsoft Graph em uma determinada pessoa.</span><span class="sxs-lookup"><span data-stu-id="43916-114">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="43916-115">Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="43916-115">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="43916-116">Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.</span><span class="sxs-lookup"><span data-stu-id="43916-116">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="43916-117">Defina o `person-details` atributo ou `personDetails` a propriedade para definir manualmente os detalhes da pessoa, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="43916-117">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="43916-118">Se nenhuma imagem for fornecida, uma será buscada (se disponível).</span><span class="sxs-lookup"><span data-stu-id="43916-118">If no image is provided, one will be fetched (if available).</span></span>

## <a name="changing-how-the-component-looks"></a><span data-ttu-id="43916-119">Alterar a aparência do componente</span><span class="sxs-lookup"><span data-stu-id="43916-119">Changing how the component looks</span></span>

<span data-ttu-id="43916-120">Você pode usar várias propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="43916-120">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="43916-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43916-121">Property</span></span>    | <span data-ttu-id="43916-122">Atributo</span><span class="sxs-lookup"><span data-stu-id="43916-122">Attribute</span></span>    | <span data-ttu-id="43916-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="43916-123">Description</span></span>                                                   |
| ----------- | ------------ | ------------------------------------------------------------- |
| <span data-ttu-id="43916-124">Nome do mesmo</span><span class="sxs-lookup"><span data-stu-id="43916-124">showName</span></span>  | <span data-ttu-id="43916-125">show-Name</span><span class="sxs-lookup"><span data-stu-id="43916-125">show-name</span></span>  | <span data-ttu-id="43916-126">Definir sinalizador para exibir o nome de exibição da pessoa `false`-o padrão é.</span><span class="sxs-lookup"><span data-stu-id="43916-126">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="43916-127">Enviar email</span><span class="sxs-lookup"><span data-stu-id="43916-127">showEmail</span></span> | <span data-ttu-id="43916-128">Mostrar-email</span><span class="sxs-lookup"><span data-stu-id="43916-128">show-email</span></span> | <span data-ttu-id="43916-129">Definir sinalizador para exibir o email da pessoa- `false`o padrão é.</span><span class="sxs-lookup"><span data-stu-id="43916-129">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="43916-130">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="43916-130">CSS custom properties</span></span>

<span data-ttu-id="43916-131">O `mgt-person` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="43916-131">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="43916-132">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="43916-132">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="43916-133">Modelos</span><span class="sxs-lookup"><span data-stu-id="43916-133">Templates</span></span>

<span data-ttu-id="43916-134">O `mgt-person` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="43916-134">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="43916-135">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="43916-135">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="43916-136">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="43916-136">Data type</span></span>     | <span data-ttu-id="43916-137">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="43916-137">Data context</span></span>              | <span data-ttu-id="43916-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="43916-138">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="43916-139">Padrão.</span><span class="sxs-lookup"><span data-stu-id="43916-139">default</span></span>     | <span data-ttu-id="43916-140">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="43916-140">person: The person details object</span></span> <br> <span data-ttu-id="43916-141">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="43916-141">`personImage`: The URL of the image</span></span> | <span data-ttu-id="43916-142">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="43916-142">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="43916-143">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="43916-143">person-card</span></span> | <span data-ttu-id="43916-144">Person: o objeto de detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="43916-144">person: The person details object</span></span> <br> <span data-ttu-id="43916-145">`personImage`: A URL da imagem</span><span class="sxs-lookup"><span data-stu-id="43916-145">`personImage`: The URL of the image</span></span> | <span data-ttu-id="43916-146">O modelo para atualizar o item de gerenciamento de pessoa que é exibido ao focalizar ou clique.</span><span class="sxs-lookup"><span data-stu-id="43916-146">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="43916-147">O exemplo a seguir define um modelo para o componente Person.</span><span class="sxs-lookup"><span data-stu-id="43916-147">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="43916-148">Cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="43916-148">Person Card</span></span>

<span data-ttu-id="43916-149">O `mgt-person` componente pode mostrar um `mgt-person-card` em foco ou clique.</span><span class="sxs-lookup"><span data-stu-id="43916-149">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="43916-150">Adicionar o controle à página HTML</span><span class="sxs-lookup"><span data-stu-id="43916-150">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="43916-151">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43916-151">Property</span></span>     | <span data-ttu-id="43916-152">Atributo</span><span class="sxs-lookup"><span data-stu-id="43916-152">Attribute</span></span>     | <span data-ttu-id="43916-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="43916-153">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="43916-154">personCard</span><span class="sxs-lookup"><span data-stu-id="43916-154">personCard</span></span> | <span data-ttu-id="43916-155">cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="43916-155">person-card</span></span> | <span data-ttu-id="43916-156">Uma enumeração para determinar a ação do usuário necessária para ativar o `hover` painel `click`ou o menu suspenso.</span><span class="sxs-lookup"><span data-stu-id="43916-156">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="43916-157">O valor padrão é`none`</span><span class="sxs-lookup"><span data-stu-id="43916-157">Default value is `none`</span></span> |


<span data-ttu-id="43916-158">Para obter mais informações sobre modelos, estilos e atributos, consulte [componente de cartão de pessoa](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="43916-158">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="43916-159">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="43916-159">Microsoft Graph permissions</span></span>

<span data-ttu-id="43916-160">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="43916-160">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="43916-161">Resource</span><span class="sxs-lookup"><span data-stu-id="43916-161">Resource</span></span>                                                                                                    | <span data-ttu-id="43916-162">Permissão</span><span class="sxs-lookup"><span data-stu-id="43916-162">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="43916-163">/me</span><span class="sxs-lookup"><span data-stu-id="43916-163">/me</span></span>](https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="43916-164">User.Read</span><span class="sxs-lookup"><span data-stu-id="43916-164">User.Read</span></span>          |
| [<span data-ttu-id="43916-165">$value/me/Photo/</span><span class="sxs-lookup"><span data-stu-id="43916-165">/me/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="43916-166">User.Read</span><span class="sxs-lookup"><span data-stu-id="43916-166">User.Read</span></span>          |
| [<span data-ttu-id="43916-167">/me/People/? $search =</span><span class="sxs-lookup"><span data-stu-id="43916-167">/me/people/?$search=</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="43916-168">People.Read</span><span class="sxs-lookup"><span data-stu-id="43916-168">People.Read</span></span>        |
| [<span data-ttu-id="43916-169">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="43916-169">/me/contacts/\*</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="43916-170">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="43916-170">Contacts.Read</span></span>      |
| [<span data-ttu-id="43916-171">$value/Users/{ID}/Photo/</span><span class="sxs-lookup"><span data-stu-id="43916-171">/users/{id}/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="43916-172">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="43916-172">User.ReadBasic.All</span></span> |

> <span data-ttu-id="43916-173">**Observação:** para acessar os `*/photo/$value` recursos para contas pessoais da Microsoft, use o ponto de extremidade beta do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="43916-173">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="43916-174">Autenticação</span><span class="sxs-lookup"><span data-stu-id="43916-174">Authentication</span></span>

<span data-ttu-id="43916-175">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md) para buscar os dados necessários.</span><span class="sxs-lookup"><span data-stu-id="43916-175">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
