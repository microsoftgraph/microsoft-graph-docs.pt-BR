---
title: Componente de logon no microsoft Graph Toolkit
description: Um componente de Logon é um botão e um controle de sobrevoo para facilitar plataforma de identidade da Microsoft autenticação.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: ea7df01c77900eecc415b3670db0ea2736447d8c
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781076"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="f774a-103">Componente de logon no microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="f774a-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f774a-104">Um componente de Logon é um botão e um controle de sobrevoo para facilitar plataforma de identidade da Microsoft autenticação.</span><span class="sxs-lookup"><span data-stu-id="f774a-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="f774a-105">Ele fornece dois estados:</span><span class="sxs-lookup"><span data-stu-id="f774a-105">It provides two states:</span></span>
* <span data-ttu-id="f774a-106">Quando o usuário não está assinado, o controle é um botão simples para iniciar o processo de logoff.</span><span class="sxs-lookup"><span data-stu-id="f774a-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="f774a-107">Quando o usuário está assinado, o controle exibe o nome de usuário, a imagem do perfil e o email.</span><span class="sxs-lookup"><span data-stu-id="f774a-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="f774a-108">Quando clicado, um sobrevoo é aberto com um comando para sair.</span><span class="sxs-lookup"><span data-stu-id="f774a-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="f774a-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f774a-109">Example</span></span>

<span data-ttu-id="f774a-110">O exemplo a seguir mostra `mgt-login` o componente com um usuário internado.</span><span class="sxs-lookup"><span data-stu-id="f774a-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="f774a-111">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="f774a-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="f774a-112">Usando o controle sem um provedor de autenticação</span><span class="sxs-lookup"><span data-stu-id="f774a-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="f774a-113">O componente funciona com um provedor e a Microsoft Graph fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="f774a-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="f774a-114">No entanto, se você quiser fornecer sua própria lógica e autenticação, poderá usar a propriedade para definir os detalhes `userDetails` do usuário.</span><span class="sxs-lookup"><span data-stu-id="f774a-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="f774a-115">Atributo</span><span class="sxs-lookup"><span data-stu-id="f774a-115">Attribute</span></span> | <span data-ttu-id="f774a-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f774a-116">Property</span></span> | <span data-ttu-id="f774a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f774a-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="f774a-118">user-details</span><span class="sxs-lookup"><span data-stu-id="f774a-118">user-details</span></span> | <span data-ttu-id="f774a-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="f774a-119">userDetails</span></span> | <span data-ttu-id="f774a-120">De definir o objeto do usuário que será exibido no controle.</span><span class="sxs-lookup"><span data-stu-id="f774a-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="f774a-121">O exemplo a seguir define os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="f774a-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="f774a-122">A `userDetails` `null` configuração para irá para o estado de saída.</span><span class="sxs-lookup"><span data-stu-id="f774a-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="f774a-123">Use os `loginInitiated` eventos e para manipular a saída e a `logoutInitiated` saída.</span><span class="sxs-lookup"><span data-stu-id="f774a-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="f774a-124">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="f774a-124">CSS custom properties</span></span>

<span data-ttu-id="f774a-125">O `mgt-login` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="f774a-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --weith: '100%';
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --button-color: #201f1e;
  --button-color--hover: var(--theme-primary-color);
  --button-background-color: transparent;
  --button-background-color--hover: #edebe9;
  --popup-background-color: white;
  --popup-command-font-size: 12px;
  --popup-color: #201f1e;
}
```

<span data-ttu-id="f774a-126">Para saber mais, confira [componentes de estilo](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="f774a-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="f774a-127">Eventos</span><span class="sxs-lookup"><span data-stu-id="f774a-127">Events</span></span>

<span data-ttu-id="f774a-128">Os eventos a seguir são disparados do controle.</span><span class="sxs-lookup"><span data-stu-id="f774a-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="f774a-129">Evento</span><span class="sxs-lookup"><span data-stu-id="f774a-129">Event</span></span> | <span data-ttu-id="f774a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f774a-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="f774a-131">O usuário clicou no botão entrar para iniciar o processo de logon - cancelável.</span><span class="sxs-lookup"><span data-stu-id="f774a-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="f774a-132">o processo de logon foi bem-sucedido e o usuário agora está login.</span><span class="sxs-lookup"><span data-stu-id="f774a-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="f774a-133">O usuário cancelou o processo de logon ou não pôde entrar.</span><span class="sxs-lookup"><span data-stu-id="f774a-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="f774a-134">O usuário começou a fazer logout - cancelável.</span><span class="sxs-lookup"><span data-stu-id="f774a-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="f774a-135">O usuário se alistou.</span><span class="sxs-lookup"><span data-stu-id="f774a-135">The user signed out.</span></span> |

## <a name="templates"></a><span data-ttu-id="f774a-136">Modelos</span><span class="sxs-lookup"><span data-stu-id="f774a-136">Templates</span></span>

<span data-ttu-id="f774a-137">O `mgt-login` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="f774a-137">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="f774a-138">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o valor como um dos `<template>` `data-type` valores listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f774a-138">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="f774a-139">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="f774a-139">Data type</span></span> | <span data-ttu-id="f774a-140">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="f774a-140">Data context</span></span> | <span data-ttu-id="f774a-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="f774a-141">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="f774a-142">signed-in-button-content</span><span class="sxs-lookup"><span data-stu-id="f774a-142">signed-in-button-content</span></span> | <span data-ttu-id="f774a-143">personDetails: objeto person, `personImage` : cadeia de caracteres de imagem da pessoa</span><span class="sxs-lookup"><span data-stu-id="f774a-143">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="f774a-144">O modelo usado para renderizar o conteúdo no botão quando o usuário está assinado.</span><span class="sxs-lookup"><span data-stu-id="f774a-144">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="f774a-145">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="f774a-145">signed-out-button-content</span></span> | <span data-ttu-id="f774a-146">null</span><span class="sxs-lookup"><span data-stu-id="f774a-146">null</span></span> | <span data-ttu-id="f774a-147">O modelo usado para renderizar o conteúdo no botão quando o usuário não estiver assinado.</span><span class="sxs-lookup"><span data-stu-id="f774a-147">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="f774a-148">comandos de sub-</span><span class="sxs-lookup"><span data-stu-id="f774a-148">flyout-commands</span></span> | <span data-ttu-id="f774a-149">handleSignOut: função de saída</span><span class="sxs-lookup"><span data-stu-id="f774a-149">handleSignOut: sign out function</span></span> | <span data-ttu-id="f774a-150">O modelo usado para renderizar os comandos no flyout</span><span class="sxs-lookup"><span data-stu-id="f774a-150">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="f774a-151">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="f774a-151">flyout-person-details</span></span> | <span data-ttu-id="f774a-152">personDetails: objeto person, personImage: cadeia de caracteres de imagem da pessoa</span><span class="sxs-lookup"><span data-stu-id="f774a-152">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="f774a-153">O modelo usado para renderizar os detalhes da pessoa no sobremenu.</span><span class="sxs-lookup"><span data-stu-id="f774a-153">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="f774a-154">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f774a-154">Microsoft Graph permissions</span></span>

<span data-ttu-id="f774a-155">Este componente usa as seguintes APIs Graph Microsoft e permissões:</span><span class="sxs-lookup"><span data-stu-id="f774a-155">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="f774a-156">Configuração</span><span class="sxs-lookup"><span data-stu-id="f774a-156">Configuration</span></span> | <span data-ttu-id="f774a-157">Permissão</span><span class="sxs-lookup"><span data-stu-id="f774a-157">Permission</span></span> | <span data-ttu-id="f774a-158">API</span><span class="sxs-lookup"><span data-stu-id="f774a-158">API</span></span>
| - | - | - |
| <span data-ttu-id="f774a-159">Padrão.</span><span class="sxs-lookup"><span data-stu-id="f774a-159">default</span></span> | <span data-ttu-id="f774a-160">User.Read</span><span class="sxs-lookup"><span data-stu-id="f774a-160">User.Read</span></span> | [<span data-ttu-id="f774a-161">/users/me/</span><span class="sxs-lookup"><span data-stu-id="f774a-161">/users/me/</span></span>](/graph/api/user-get) |

<span data-ttu-id="f774a-162">Ao usar o padrão e os modelos, esse componente usa o componente Person para exibir o usuário e `signed-in-button-content` `flyout-person-details` herda todas as permissões. [](./person.md)</span><span class="sxs-lookup"><span data-stu-id="f774a-162">When using the default `signed-in-button-content` and `flyout-person-details` templates, this component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span>

## <a name="authentication"></a><span data-ttu-id="f774a-163">Autenticação</span><span class="sxs-lookup"><span data-stu-id="f774a-163">Authentication</span></span>

<span data-ttu-id="f774a-164">O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="f774a-164">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="f774a-165">Cache</span><span class="sxs-lookup"><span data-stu-id="f774a-165">Cache</span></span>

<span data-ttu-id="f774a-166">Esse componente usa o [componente Person](./person.md) para exibir o usuário e herda toda a configuração de cache dele.</span><span class="sxs-lookup"><span data-stu-id="f774a-166">This component uses the [Person component](./person.md) to display the user and inherits all cache configuration from it.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="f774a-167">Estender para obter mais controle</span><span class="sxs-lookup"><span data-stu-id="f774a-167">Extend for more control</span></span>

<span data-ttu-id="f774a-168">Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes.</span><span class="sxs-lookup"><span data-stu-id="f774a-168">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="f774a-169">Método</span><span class="sxs-lookup"><span data-stu-id="f774a-169">Method</span></span> | <span data-ttu-id="f774a-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="f774a-170">Description</span></span> |
| - | - |
| <span data-ttu-id="f774a-171">renderButton</span><span class="sxs-lookup"><span data-stu-id="f774a-171">renderButton</span></span> | <span data-ttu-id="f774a-172">Renderiza o botão cromado.</span><span class="sxs-lookup"><span data-stu-id="f774a-172">Renders the button chrome.</span></span> |
| <span data-ttu-id="f774a-173">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="f774a-173">renderButtonContent</span></span> | <span data-ttu-id="f774a-174">Renderiza o conteúdo do botão.</span><span class="sxs-lookup"><span data-stu-id="f774a-174">Renders the button content.</span></span> |
| <span data-ttu-id="f774a-175">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="f774a-175">renderSignedInButtonContent</span></span> | <span data-ttu-id="f774a-176">Renderizar o conteúdo do botão quando o usuário estiver dentro.</span><span class="sxs-lookup"><span data-stu-id="f774a-176">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="f774a-177">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="f774a-177">renderSignedOutButtonContent</span></span> | <span data-ttu-id="f774a-178">Renderizar o conteúdo do botão quando o usuário não estiver assinado.</span><span class="sxs-lookup"><span data-stu-id="f774a-178">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="f774a-179">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="f774a-179">renderFlyout</span></span> | <span data-ttu-id="f774a-180">Renderiza o cromado do flyout.</span><span class="sxs-lookup"><span data-stu-id="f774a-180">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="f774a-181">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="f774a-181">renderFlyoutContent</span></span> | <span data-ttu-id="f774a-182">Renderiza o conteúdo do sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="f774a-182">Renders the flyout content.</span></span> |
| <span data-ttu-id="f774a-183">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="f774a-183">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="f774a-184">Renderizar os detalhes da pessoa do sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="f774a-184">Render the flyout person details.</span></span> |
| <span data-ttu-id="f774a-185">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="f774a-185">renderFlyoutCommands</span></span> | <span data-ttu-id="f774a-186">Renderizar os comandos de sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="f774a-186">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="f774a-187">Traga seu próprio flyout</span><span class="sxs-lookup"><span data-stu-id="f774a-187">Bring your own flyout</span></span>

<span data-ttu-id="f774a-188">É possível usar seu próprio componente sub-1 no lugar do um integrado, substituindo o método e fornecendo `renderFlyout()` o novo sub-20.</span><span class="sxs-lookup"><span data-stu-id="f774a-188">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="f774a-189">Nesse caso, certifique-se de que o componente de logon continue a funcionar conforme o esperado substituindo os métodos de exibição do sobrevoo para atualizar a visibilidade do seu `protected` flyout alternativo.</span><span class="sxs-lookup"><span data-stu-id="f774a-189">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="f774a-190">Método</span><span class="sxs-lookup"><span data-stu-id="f774a-190">Method</span></span> | <span data-ttu-id="f774a-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="f774a-191">Description</span></span> |
| - | - |
| <span data-ttu-id="f774a-192">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="f774a-192">hideFlyout</span></span> | <span data-ttu-id="f774a-193">Descarta o sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="f774a-193">Dismisses the flyout.</span></span> |
| <span data-ttu-id="f774a-194">showFlyout</span><span class="sxs-lookup"><span data-stu-id="f774a-194">showFlyout</span></span> | <span data-ttu-id="f774a-195">Exibe o sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="f774a-195">Displays the flyout.</span></span> |
| <span data-ttu-id="f774a-196">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="f774a-196">toggleFlyout</span></span> | <span data-ttu-id="f774a-197">Alterna o estado do sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="f774a-197">Toggles the state of the flyout.</span></span> |
