---
title: Componente de logon no microsoft Graph Toolkit
description: Um componente de Logon é um botão e um controle de sobrevoo para facilitar plataforma de identidade da Microsoft autenticação.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 1042201492720dce92016a13bd7bbd8477ce2d2c
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082150"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d6074-103">Componente de logon no microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="d6074-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d6074-104">Um componente de Logon é um botão e um controle de sobrevoo para facilitar plataforma de identidade da Microsoft autenticação.</span><span class="sxs-lookup"><span data-stu-id="d6074-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="d6074-105">Ele fornece dois estados:</span><span class="sxs-lookup"><span data-stu-id="d6074-105">It provides two states:</span></span>
* <span data-ttu-id="d6074-106">Quando o usuário não está assinado, o controle é um botão simples para iniciar o processo de logoff.</span><span class="sxs-lookup"><span data-stu-id="d6074-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="d6074-107">Quando o usuário está assinado, o controle exibe o nome de usuário, a imagem do perfil e o email.</span><span class="sxs-lookup"><span data-stu-id="d6074-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="d6074-108">Quando clicado, um sobrevoo é aberto com um comando para sair.</span><span class="sxs-lookup"><span data-stu-id="d6074-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="d6074-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6074-109">Example</span></span>

<span data-ttu-id="d6074-110">O exemplo a seguir mostra `mgt-login` o componente com um usuário internado.</span><span class="sxs-lookup"><span data-stu-id="d6074-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="d6074-111">Abrir este exemplo no mgt.dev</span><span class="sxs-lookup"><span data-stu-id="d6074-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="d6074-112">Usando o controle sem um provedor de autenticação</span><span class="sxs-lookup"><span data-stu-id="d6074-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="d6074-113">O componente funciona com um provedor e a Microsoft Graph fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="d6074-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="d6074-114">No entanto, se você quiser fornecer sua própria lógica e autenticação, poderá usar a propriedade para definir os detalhes `userDetails` do usuário.</span><span class="sxs-lookup"><span data-stu-id="d6074-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="d6074-115">Atributo</span><span class="sxs-lookup"><span data-stu-id="d6074-115">Attribute</span></span> | <span data-ttu-id="d6074-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6074-116">Property</span></span> | <span data-ttu-id="d6074-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6074-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="d6074-118">user-details</span><span class="sxs-lookup"><span data-stu-id="d6074-118">user-details</span></span> | <span data-ttu-id="d6074-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="d6074-119">userDetails</span></span> | <span data-ttu-id="d6074-120">De definir o objeto do usuário que será exibido no controle.</span><span class="sxs-lookup"><span data-stu-id="d6074-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="d6074-121">O exemplo a seguir define os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="d6074-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="d6074-122">A `userDetails` `null` configuração para irá para o estado de saída.</span><span class="sxs-lookup"><span data-stu-id="d6074-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="d6074-123">Use os `loginInitiated` eventos e para manipular a saída e a `logoutInitiated` saída.</span><span class="sxs-lookup"><span data-stu-id="d6074-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="d6074-124">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="d6074-124">CSS custom properties</span></span>

<span data-ttu-id="d6074-125">O `mgt-login` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="d6074-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="d6074-126">Para saber mais, confira [componentes de estilo](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="d6074-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="d6074-127">Eventos</span><span class="sxs-lookup"><span data-stu-id="d6074-127">Events</span></span>

<span data-ttu-id="d6074-128">Os eventos a seguir são disparados do controle.</span><span class="sxs-lookup"><span data-stu-id="d6074-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="d6074-129">Evento</span><span class="sxs-lookup"><span data-stu-id="d6074-129">Event</span></span> | <span data-ttu-id="d6074-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6074-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="d6074-131">O usuário clicou no botão entrar para iniciar o processo de logon - cancelável.</span><span class="sxs-lookup"><span data-stu-id="d6074-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="d6074-132">o processo de logon foi bem-sucedido e o usuário agora está login.</span><span class="sxs-lookup"><span data-stu-id="d6074-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="d6074-133">O usuário cancelou o processo de logon ou não pôde entrar.</span><span class="sxs-lookup"><span data-stu-id="d6074-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="d6074-134">O usuário começou a fazer logout - cancelável.</span><span class="sxs-lookup"><span data-stu-id="d6074-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="d6074-135">O usuário se alistou.</span><span class="sxs-lookup"><span data-stu-id="d6074-135">The user signed out.</span></span> |

<span data-ttu-id="d6074-136">Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).</span><span class="sxs-lookup"><span data-stu-id="d6074-136">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="d6074-137">Modelos</span><span class="sxs-lookup"><span data-stu-id="d6074-137">Templates</span></span>

<span data-ttu-id="d6074-138">O `mgt-login` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="d6074-138">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="d6074-139">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o valor como um dos `<template>` `data-type` valores listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="d6074-139">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="d6074-140">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="d6074-140">Data type</span></span> | <span data-ttu-id="d6074-141">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="d6074-141">Data context</span></span> | <span data-ttu-id="d6074-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6074-142">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="d6074-143">signed-in-button-content</span><span class="sxs-lookup"><span data-stu-id="d6074-143">signed-in-button-content</span></span> | <span data-ttu-id="d6074-144">personDetails: objeto person, `personImage` : cadeia de caracteres de imagem da pessoa</span><span class="sxs-lookup"><span data-stu-id="d6074-144">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="d6074-145">O modelo usado para renderizar o conteúdo no botão quando o usuário está assinado.</span><span class="sxs-lookup"><span data-stu-id="d6074-145">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="d6074-146">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="d6074-146">signed-out-button-content</span></span> | <span data-ttu-id="d6074-147">null</span><span class="sxs-lookup"><span data-stu-id="d6074-147">null</span></span> | <span data-ttu-id="d6074-148">O modelo usado para renderizar o conteúdo no botão quando o usuário não estiver assinado.</span><span class="sxs-lookup"><span data-stu-id="d6074-148">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="d6074-149">comandos de sub-</span><span class="sxs-lookup"><span data-stu-id="d6074-149">flyout-commands</span></span> | <span data-ttu-id="d6074-150">handleSignOut: função de saída</span><span class="sxs-lookup"><span data-stu-id="d6074-150">handleSignOut: sign out function</span></span> | <span data-ttu-id="d6074-151">O modelo usado para renderizar os comandos no flyout</span><span class="sxs-lookup"><span data-stu-id="d6074-151">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="d6074-152">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="d6074-152">flyout-person-details</span></span> | <span data-ttu-id="d6074-153">personDetails: objeto person, personImage: cadeia de caracteres de imagem da pessoa</span><span class="sxs-lookup"><span data-stu-id="d6074-153">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="d6074-154">O modelo usado para renderizar os detalhes da pessoa no sobremenu.</span><span class="sxs-lookup"><span data-stu-id="d6074-154">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="d6074-155">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6074-155">Microsoft Graph permissions</span></span>

<span data-ttu-id="d6074-156">Este componente usa as seguintes APIs Graph Microsoft e permissões:</span><span class="sxs-lookup"><span data-stu-id="d6074-156">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="d6074-157">Configuração</span><span class="sxs-lookup"><span data-stu-id="d6074-157">Configuration</span></span> | <span data-ttu-id="d6074-158">Permissão</span><span class="sxs-lookup"><span data-stu-id="d6074-158">Permission</span></span> | <span data-ttu-id="d6074-159">API</span><span class="sxs-lookup"><span data-stu-id="d6074-159">API</span></span>
| - | - | - |
| <span data-ttu-id="d6074-160">Padrão.</span><span class="sxs-lookup"><span data-stu-id="d6074-160">default</span></span> | <span data-ttu-id="d6074-161">User.Read</span><span class="sxs-lookup"><span data-stu-id="d6074-161">User.Read</span></span> | [<span data-ttu-id="d6074-162">/users/me/</span><span class="sxs-lookup"><span data-stu-id="d6074-162">/users/me/</span></span>](/graph/api/user-get) |

<span data-ttu-id="d6074-163">Ao usar o padrão e os modelos, esse componente usa o componente Person para exibir o usuário e `signed-in-button-content` `flyout-person-details` herda todas as permissões. [](./person.md)</span><span class="sxs-lookup"><span data-stu-id="d6074-163">When using the default `signed-in-button-content` and `flyout-person-details` templates, this component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span>

## <a name="authentication"></a><span data-ttu-id="d6074-164">Autenticação</span><span class="sxs-lookup"><span data-stu-id="d6074-164">Authentication</span></span>

<span data-ttu-id="d6074-165">O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="d6074-165">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="d6074-166">Cache</span><span class="sxs-lookup"><span data-stu-id="d6074-166">Cache</span></span>

<span data-ttu-id="d6074-167">Esse componente usa o [componente Person](./person.md) para exibir o usuário e herda toda a configuração de cache dele.</span><span class="sxs-lookup"><span data-stu-id="d6074-167">This component uses the [Person component](./person.md) to display the user and inherits all cache configuration from it.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="d6074-168">Estender para obter mais controle</span><span class="sxs-lookup"><span data-stu-id="d6074-168">Extend for more control</span></span>

<span data-ttu-id="d6074-169">Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes.</span><span class="sxs-lookup"><span data-stu-id="d6074-169">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="d6074-170">Método</span><span class="sxs-lookup"><span data-stu-id="d6074-170">Method</span></span> | <span data-ttu-id="d6074-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6074-171">Description</span></span> |
| - | - |
| <span data-ttu-id="d6074-172">renderButton</span><span class="sxs-lookup"><span data-stu-id="d6074-172">renderButton</span></span> | <span data-ttu-id="d6074-173">Renderiza o botão cromado.</span><span class="sxs-lookup"><span data-stu-id="d6074-173">Renders the button chrome.</span></span> |
| <span data-ttu-id="d6074-174">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="d6074-174">renderButtonContent</span></span> | <span data-ttu-id="d6074-175">Renderiza o conteúdo do botão.</span><span class="sxs-lookup"><span data-stu-id="d6074-175">Renders the button content.</span></span> |
| <span data-ttu-id="d6074-176">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="d6074-176">renderSignedInButtonContent</span></span> | <span data-ttu-id="d6074-177">Renderizar o conteúdo do botão quando o usuário estiver dentro.</span><span class="sxs-lookup"><span data-stu-id="d6074-177">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="d6074-178">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="d6074-178">renderSignedOutButtonContent</span></span> | <span data-ttu-id="d6074-179">Renderizar o conteúdo do botão quando o usuário não estiver assinado.</span><span class="sxs-lookup"><span data-stu-id="d6074-179">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="d6074-180">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="d6074-180">renderFlyout</span></span> | <span data-ttu-id="d6074-181">Renderiza o cromado do flyout.</span><span class="sxs-lookup"><span data-stu-id="d6074-181">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="d6074-182">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="d6074-182">renderFlyoutContent</span></span> | <span data-ttu-id="d6074-183">Renderiza o conteúdo do sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="d6074-183">Renders the flyout content.</span></span> |
| <span data-ttu-id="d6074-184">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="d6074-184">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="d6074-185">Renderizar os detalhes da pessoa do sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="d6074-185">Render the flyout person details.</span></span> |
| <span data-ttu-id="d6074-186">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="d6074-186">renderFlyoutCommands</span></span> | <span data-ttu-id="d6074-187">Renderizar os comandos de sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="d6074-187">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="d6074-188">Traga seu próprio flyout</span><span class="sxs-lookup"><span data-stu-id="d6074-188">Bring your own flyout</span></span>

<span data-ttu-id="d6074-189">É possível usar seu próprio componente sub-1 no lugar do um integrado, substituindo o método e fornecendo `renderFlyout()` o novo sub-20.</span><span class="sxs-lookup"><span data-stu-id="d6074-189">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="d6074-190">Nesse caso, certifique-se de que o componente de logon continue a funcionar conforme o esperado substituindo os métodos de exibição do sobrevoo para atualizar a visibilidade do seu `protected` flyout alternativo.</span><span class="sxs-lookup"><span data-stu-id="d6074-190">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="d6074-191">Método</span><span class="sxs-lookup"><span data-stu-id="d6074-191">Method</span></span> | <span data-ttu-id="d6074-192">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6074-192">Description</span></span> |
| - | - |
| <span data-ttu-id="d6074-193">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="d6074-193">hideFlyout</span></span> | <span data-ttu-id="d6074-194">Descarta o sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="d6074-194">Dismisses the flyout.</span></span> |
| <span data-ttu-id="d6074-195">showFlyout</span><span class="sxs-lookup"><span data-stu-id="d6074-195">showFlyout</span></span> | <span data-ttu-id="d6074-196">Exibe o sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="d6074-196">Displays the flyout.</span></span> |
| <span data-ttu-id="d6074-197">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="d6074-197">toggleFlyout</span></span> | <span data-ttu-id="d6074-198">Alterna o estado do sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="d6074-198">Toggles the state of the flyout.</span></span> |
