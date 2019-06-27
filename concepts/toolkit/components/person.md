---
title: Componente Person no Microsoft Graph Toolkit
description: O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b9102259258bb691dee2c56449257740db7b1913
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242926"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="928ed-103">Componente Person no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="928ed-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="928ed-104">O componente pessoa é usado para exibir uma pessoa ou contato usando sua foto, nome e/ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="928ed-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span> 

## <a name="example"></a><span data-ttu-id="928ed-105">Exemplo</span><span class="sxs-lookup"><span data-stu-id="928ed-105">Example</span></span>

[<span data-ttu-id="928ed-106">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="928ed-106">jsfiddle example</span></span>](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="928ed-107">Adicionar o controle à página HTML</span><span class="sxs-lookup"><span data-stu-id="928ed-107">Add the control to the HTML page</span></span>
```html
<mgt-person person-query=""></mgt-person>
```

## <a name="setting-the-person-details"></a><span data-ttu-id="928ed-108">Configurando os detalhes da pessoa</span><span class="sxs-lookup"><span data-stu-id="928ed-108">Setting the person details</span></span>

<span data-ttu-id="928ed-109">Você pode usar três propriedades para definir os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="928ed-109">You can use three properties to set the person details.</span></span> <span data-ttu-id="928ed-110">Use apenas uma das seguintes propriedades por instância:</span><span class="sxs-lookup"><span data-stu-id="928ed-110">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="928ed-111">Defina o `user-id` atributo ou `userId` a propriedade para buscar o usuário do Microsoft Graph usando sua ID.</span><span class="sxs-lookup"><span data-stu-id="928ed-111">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>  

* <span data-ttu-id="928ed-112">Definir o `person-query` atributo ou `personQuery` a propriedade para pesquisar o Microsoft Graph em uma determinada pessoa.</span><span class="sxs-lookup"><span data-stu-id="928ed-112">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="928ed-113">Ele escolherá a primeira pessoa disponível e buscará os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="928ed-113">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="928ed-114">Um email funciona melhor para garantir que a pessoa certa seja consultada, mas um nome também funciona.</span><span class="sxs-lookup"><span data-stu-id="928ed-114">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="928ed-115">Defina o `person-details` atributo ou `personDetails` a propriedade para definir manualmente os detalhes da pessoa, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="928ed-115">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="928ed-116">Se nenhuma imagem for fornecida, uma será buscada (se disponível).</span><span class="sxs-lookup"><span data-stu-id="928ed-116">If no image is provided, one will be fetched (if available).</span></span>

## <a name="changing-how-the-component-looks"></a><span data-ttu-id="928ed-117">Alterar a aparência do componente</span><span class="sxs-lookup"><span data-stu-id="928ed-117">Changing how the component looks</span></span>

<span data-ttu-id="928ed-118">Você pode usar várias Propriedadespara personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="928ed-118">You can use several propertiesto customize the component.</span></span>

| <span data-ttu-id="928ed-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="928ed-119">Property</span></span> | <span data-ttu-id="928ed-120">Atributo</span><span class="sxs-lookup"><span data-stu-id="928ed-120">Attribute</span></span> | <span data-ttu-id="928ed-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="928ed-121">Description</span></span> |
| --- | --- | --- |
| `showName` | `show-name` | <span data-ttu-id="928ed-122">Definir sinalizador para exibir o nome de exibição da pessoa `false`-o padrão é.</span><span class="sxs-lookup"><span data-stu-id="928ed-122">Set flag to display person display name - default is `false`.</span></span> |
| `showEmail` | `show-email` | <span data-ttu-id="928ed-123">Definir sinalizador para exibir o email da pessoa- `false`o padrão é.</span><span class="sxs-lookup"><span data-stu-id="928ed-123">Set flag to display person email - default is `false`.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="928ed-124">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="928ed-124">CSS custom properties</span></span>

<span data-ttu-id="928ed-125">O `mgt-person` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="928ed-125">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="928ed-126">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="928ed-126">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="928ed-127">Modelos</span><span class="sxs-lookup"><span data-stu-id="928ed-127">Templates</span></span>

<span data-ttu-id="928ed-128">O `mgt-person` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="928ed-128">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="928ed-129">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="928ed-129">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="928ed-130">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="928ed-130">Data type</span></span> | <span data-ttu-id="928ed-131">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="928ed-131">Data context</span></span> | <span data-ttu-id="928ed-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="928ed-132">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="928ed-133">`person`: um objeto Person</span><span class="sxs-lookup"><span data-stu-id="928ed-133">`person`: a person object</span></span> | <span data-ttu-id="928ed-134">O modelo padrão substitui todo o componente pelo seu.</span><span class="sxs-lookup"><span data-stu-id="928ed-134">The default template replaces the entire component with your own.</span></span> |

<span data-ttu-id="928ed-135">O exemplo a seguir define um modelo para o componente Person:</span><span class="sxs-lookup"><span data-stu-id="928ed-135">The following example defines a template for the person component:</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="928ed-136">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="928ed-136">Microsoft Graph permissions</span></span>

<span data-ttu-id="928ed-137">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="928ed-137">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="928ed-138">Resource</span><span class="sxs-lookup"><span data-stu-id="928ed-138">Resource</span></span> | <span data-ttu-id="928ed-139">Permissão/escopo</span><span class="sxs-lookup"><span data-stu-id="928ed-139">Permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="928ed-140">/me</span><span class="sxs-lookup"><span data-stu-id="928ed-140">/me</span></span>](https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0) | `User.Read` |
| [<span data-ttu-id="928ed-141">$value/me/Photo/</span><span class="sxs-lookup"><span data-stu-id="928ed-141">/me/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/profilephoto-get?view=graph-rest-beta) | `User.Read` |
| [<span data-ttu-id="928ed-142">/me/People/? $search =</span><span class="sxs-lookup"><span data-stu-id="928ed-142">/me/people/?$search=</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |
| [<span data-ttu-id="928ed-143">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="928ed-143">/me/contacts/\*</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | `Contacts.Read` |
| [<span data-ttu-id="928ed-144">$value/Users/{ID}/Photo/</span><span class="sxs-lookup"><span data-stu-id="928ed-144">/users/{id}/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `User.ReadBasic.All` |

> <span data-ttu-id="928ed-145">**Observação:** para acessar os `*/photo/$value` recursos para contas pessoais da Microsoft, use o ponto de extremidade beta do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="928ed-145">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="928ed-146">Autenticação</span><span class="sxs-lookup"><span data-stu-id="928ed-146">Authentication</span></span>

<span data-ttu-id="928ed-147">O controle usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md) para buscar os dados necessários.</span><span class="sxs-lookup"><span data-stu-id="928ed-147">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
