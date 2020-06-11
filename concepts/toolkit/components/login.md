---
title: Componente de logon no kit de ferramentas do Microsoft Graph
description: Um componente de logon é um botão e um controle de submenu para facilitar a autenticação da plataforma de identidade da Microsoft.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 441639c309025eb8fefbbe551dd60b6324a7fd3c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682030"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="46785-103">Componente de logon no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="46785-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="46785-104">Um componente de logon é um botão e um controle de submenu para facilitar a autenticação da plataforma de identidade da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="46785-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="46785-105">Ele fornece dois Estados:</span><span class="sxs-lookup"><span data-stu-id="46785-105">It provides two states:</span></span>
* <span data-ttu-id="46785-106">Quando o usuário não está conectado, o controle é um botão simples para iniciar o processo de entrada.</span><span class="sxs-lookup"><span data-stu-id="46785-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="46785-107">Quando o usuário está conectado, o controle exibe o nome de usuário conectado atual, a imagem de perfil e o email.</span><span class="sxs-lookup"><span data-stu-id="46785-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="46785-108">Quando clicado, um submenu é aberto com um comando para sair.</span><span class="sxs-lookup"><span data-stu-id="46785-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="46785-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46785-109">Example</span></span>

<span data-ttu-id="46785-110">O exemplo a seguir mostra o `mgt-login` componente com um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="46785-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="46785-111">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="46785-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="46785-112">Usando o controle sem um provedor de autenticação</span><span class="sxs-lookup"><span data-stu-id="46785-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="46785-113">O componente funciona com um provedor e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="46785-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="46785-114">No entanto, se você quiser fornecer sua própria lógica e autenticação, você pode usar a `userDetails` propriedade para definir os detalhes do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="46785-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="46785-115">Atributo</span><span class="sxs-lookup"><span data-stu-id="46785-115">Attribute</span></span> | <span data-ttu-id="46785-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46785-116">Property</span></span> | <span data-ttu-id="46785-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="46785-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="46785-118">User-detalhes</span><span class="sxs-lookup"><span data-stu-id="46785-118">user-details</span></span> | <span data-ttu-id="46785-119">userdetails</span><span class="sxs-lookup"><span data-stu-id="46785-119">userDetails</span></span> | <span data-ttu-id="46785-120">Defina o objeto de usuário que será exibido no controle.</span><span class="sxs-lookup"><span data-stu-id="46785-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="46785-121">O exemplo a seguir define os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="46785-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="46785-122">`userDetails`A configuração para vai `null` para o estado de desconectar.</span><span class="sxs-lookup"><span data-stu-id="46785-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="46785-123">Use os `loginInitiated` `logoutInitiated` eventos e para lidar com a entrada e a saída.</span><span class="sxs-lookup"><span data-stu-id="46785-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="46785-124">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="46785-124">CSS custom properties</span></span>

<span data-ttu-id="46785-125">O `mgt-login` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="46785-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --color: #201f1e;
  --color-hover: var(--theme-primary-color);
  --background-color: transparent;
  --background-color--hover: #edebe9;
  --popup-content-background-color: white;
  --popup-command-font-size: 12px;
  --popup-color: #201f1e;
}
```

<span data-ttu-id="46785-126">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="46785-126">To learn more, see [styling components](../style.md).</span></span>

## <a name="events"></a><span data-ttu-id="46785-127">Eventos</span><span class="sxs-lookup"><span data-stu-id="46785-127">Events</span></span>

<span data-ttu-id="46785-128">Os eventos a seguir são acionados do controle.</span><span class="sxs-lookup"><span data-stu-id="46785-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="46785-129">Evento</span><span class="sxs-lookup"><span data-stu-id="46785-129">Event</span></span> | <span data-ttu-id="46785-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="46785-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="46785-131">O usuário clicou no botão entrar para iniciar o processo de logon-cancelable.</span><span class="sxs-lookup"><span data-stu-id="46785-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="46785-132">o processo de login foi bem-sucedido e o usuário está conectado.</span><span class="sxs-lookup"><span data-stu-id="46785-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="46785-133">O usuário cancelou o processo de logon ou não pôde entrar.</span><span class="sxs-lookup"><span data-stu-id="46785-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="46785-134">O usuário iniciou o logout-cancelamento.</span><span class="sxs-lookup"><span data-stu-id="46785-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="46785-135">O usuário saiu.</span><span class="sxs-lookup"><span data-stu-id="46785-135">The user signed out.</span></span> |

## <a name="templates"></a><span data-ttu-id="46785-136">Modelos</span><span class="sxs-lookup"><span data-stu-id="46785-136">Templates</span></span>

<span data-ttu-id="46785-137">O `mgt-login` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="46785-137">The `mgt-login` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="46785-138">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos valores listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="46785-138">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="46785-139">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="46785-139">Data type</span></span> | <span data-ttu-id="46785-140">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="46785-140">Data context</span></span> | <span data-ttu-id="46785-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="46785-141">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="46785-142">conectado ao botão de conteúdo</span><span class="sxs-lookup"><span data-stu-id="46785-142">signed-in-button-content</span></span> | <span data-ttu-id="46785-143">personDetails: objeto Person, `personImage` : cadeia de caracteres de imagem de pessoa</span><span class="sxs-lookup"><span data-stu-id="46785-143">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="46785-144">O modelo usado para renderizar o conteúdo no botão quando o usuário está conectado.</span><span class="sxs-lookup"><span data-stu-id="46785-144">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="46785-145">desconectado-botão-conteúdo</span><span class="sxs-lookup"><span data-stu-id="46785-145">signed-out-button-content</span></span> | <span data-ttu-id="46785-146">null</span><span class="sxs-lookup"><span data-stu-id="46785-146">null</span></span> | <span data-ttu-id="46785-147">O modelo usado para renderizar o conteúdo no botão quando o usuário não está conectado.</span><span class="sxs-lookup"><span data-stu-id="46785-147">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="46785-148">submenu-comandos</span><span class="sxs-lookup"><span data-stu-id="46785-148">flyout-commands</span></span> | <span data-ttu-id="46785-149">handleSignOut: função de saída</span><span class="sxs-lookup"><span data-stu-id="46785-149">handleSignOut: sign out function</span></span> | <span data-ttu-id="46785-150">O modelo usado para renderizar os comandos no submenu</span><span class="sxs-lookup"><span data-stu-id="46785-150">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="46785-151">submenu de pessoas-detalhes</span><span class="sxs-lookup"><span data-stu-id="46785-151">flyout-person-details</span></span> | <span data-ttu-id="46785-152">personDetails: objeto Person, personImage: cadeia de caracteres de imagem de pessoa</span><span class="sxs-lookup"><span data-stu-id="46785-152">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="46785-153">O modelo usado para renderizar os detalhes da pessoa no submenu.</span><span class="sxs-lookup"><span data-stu-id="46785-153">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="46785-154">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="46785-154">Microsoft Graph permissions</span></span>

<span data-ttu-id="46785-155">Este componente usa o [componente Person](./person.md) para exibir o usuário e herda todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="46785-155">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="46785-156">Autenticação</span><span class="sxs-lookup"><span data-stu-id="46785-156">Authentication</span></span>

<span data-ttu-id="46785-157">O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="46785-157">The login control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

## <a name="extend-for-more-control"></a><span data-ttu-id="46785-158">Estender para mais controle</span><span class="sxs-lookup"><span data-stu-id="46785-158">Extend for more control</span></span>

<span data-ttu-id="46785-159">Para cenários mais complexos ou uma UX verdadeiramente personalizada, esse componente expõe vários `protected render*` métodos para substituir em extensões de componente.</span><span class="sxs-lookup"><span data-stu-id="46785-159">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="46785-160">Método</span><span class="sxs-lookup"><span data-stu-id="46785-160">Method</span></span> | <span data-ttu-id="46785-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="46785-161">Description</span></span> |
| - | - |
| <span data-ttu-id="46785-162">renderButton</span><span class="sxs-lookup"><span data-stu-id="46785-162">renderButton</span></span> | <span data-ttu-id="46785-163">Renderiza o cromo do botão.</span><span class="sxs-lookup"><span data-stu-id="46785-163">Renders the button chrome.</span></span> |
| <span data-ttu-id="46785-164">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="46785-164">renderButtonContent</span></span> | <span data-ttu-id="46785-165">Renderiza o conteúdo do botão.</span><span class="sxs-lookup"><span data-stu-id="46785-165">Renders the button content.</span></span> |
| <span data-ttu-id="46785-166">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="46785-166">renderSignedInButtonContent</span></span> | <span data-ttu-id="46785-167">Processe o conteúdo do botão quando o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="46785-167">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="46785-168">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="46785-168">renderSignedOutButtonContent</span></span> | <span data-ttu-id="46785-169">Renderiza o conteúdo do botão quando o usuário não está conectado.</span><span class="sxs-lookup"><span data-stu-id="46785-169">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="46785-170">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="46785-170">renderFlyout</span></span> | <span data-ttu-id="46785-171">Renderiza o cromo domenu.</span><span class="sxs-lookup"><span data-stu-id="46785-171">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="46785-172">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="46785-172">renderFlyoutContent</span></span> | <span data-ttu-id="46785-173">Renderiza o conteúdo do submenu.</span><span class="sxs-lookup"><span data-stu-id="46785-173">Renders the flyout content.</span></span> |
| <span data-ttu-id="46785-174">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="46785-174">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="46785-175">Renderizar os detalhes da pessoa de submenu.</span><span class="sxs-lookup"><span data-stu-id="46785-175">Render the flyout person details.</span></span> |
| <span data-ttu-id="46785-176">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="46785-176">renderFlyoutCommands</span></span> | <span data-ttu-id="46785-177">Renderizar os comandos de submenu.</span><span class="sxs-lookup"><span data-stu-id="46785-177">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="46785-178">Traga seu próprio submenu</span><span class="sxs-lookup"><span data-stu-id="46785-178">Bring your own flyout</span></span>

<span data-ttu-id="46785-179">É possível usar seu próprio componente de submenu no lugar do interno, substituindo o `renderFlyout()` método e fornecendo o novo submenu.</span><span class="sxs-lookup"><span data-stu-id="46785-179">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="46785-180">Nesse caso, verifique se o componente de login continua funcionando conforme o esperado, substituindo os `protected` métodos de exibição de submenu para atualizar a visibilidade do submenu alternativo.</span><span class="sxs-lookup"><span data-stu-id="46785-180">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="46785-181">Método</span><span class="sxs-lookup"><span data-stu-id="46785-181">Method</span></span> | <span data-ttu-id="46785-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="46785-182">Description</span></span> |
| - | - |
| <span data-ttu-id="46785-183">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="46785-183">hideFlyout</span></span> | <span data-ttu-id="46785-184">Descarta o submenu.</span><span class="sxs-lookup"><span data-stu-id="46785-184">Dismisses the flyout.</span></span> |
| <span data-ttu-id="46785-185">Menu de atalho</span><span class="sxs-lookup"><span data-stu-id="46785-185">showFlyout</span></span> | <span data-ttu-id="46785-186">Exibe o submenu.</span><span class="sxs-lookup"><span data-stu-id="46785-186">Displays the flyout.</span></span> |
| <span data-ttu-id="46785-187">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="46785-187">toggleFlyout</span></span> | <span data-ttu-id="46785-188">Alterna o estado do submenu.</span><span class="sxs-lookup"><span data-stu-id="46785-188">Toggles the state of the flyout.</span></span> |
