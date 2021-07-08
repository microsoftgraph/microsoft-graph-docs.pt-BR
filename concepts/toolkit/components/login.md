---
title: Componente de logon no microsoft Graph Toolkit
description: Um componente de Logon é um botão e um controle de sobrevoo para facilitar plataforma de identidade da Microsoft autenticação.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 5dd610407fde25089a9c323b6b0cfb7965d33671
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334763"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="58f68-103">Componente de logon no microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="58f68-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="58f68-104">Um componente de Logon é um botão e um controle de sobrevoo para facilitar plataforma de identidade da Microsoft autenticação.</span><span class="sxs-lookup"><span data-stu-id="58f68-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="58f68-105">Ele fornece dois estados:</span><span class="sxs-lookup"><span data-stu-id="58f68-105">It provides two states:</span></span>
* <span data-ttu-id="58f68-106">Quando o usuário não está assinado, o controle é um botão simples para iniciar o processo de logoff.</span><span class="sxs-lookup"><span data-stu-id="58f68-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="58f68-107">Quando o usuário está assinado, o controle exibe o nome de usuário, a imagem do perfil e o email.</span><span class="sxs-lookup"><span data-stu-id="58f68-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="58f68-108">Quando clicado, um sobrevoo é aberto com um comando para sair.</span><span class="sxs-lookup"><span data-stu-id="58f68-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="58f68-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58f68-109">Example</span></span>

<span data-ttu-id="58f68-110">O exemplo a seguir mostra `mgt-login` o componente com um usuário internado.</span><span class="sxs-lookup"><span data-stu-id="58f68-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="58f68-111">Abrir este exemplo no mgt.dev</span><span class="sxs-lookup"><span data-stu-id="58f68-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="58f68-112">Usando o controle sem um provedor de autenticação</span><span class="sxs-lookup"><span data-stu-id="58f68-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="58f68-113">O componente funciona com um provedor e a Microsoft Graph fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="58f68-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="58f68-114">No entanto, se você quiser fornecer sua própria lógica e autenticação, poderá usar a propriedade para definir os detalhes `userDetails` do usuário.</span><span class="sxs-lookup"><span data-stu-id="58f68-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="58f68-115">Atributo</span><span class="sxs-lookup"><span data-stu-id="58f68-115">Attribute</span></span> | <span data-ttu-id="58f68-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58f68-116">Property</span></span> | <span data-ttu-id="58f68-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="58f68-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="58f68-118">user-details</span><span class="sxs-lookup"><span data-stu-id="58f68-118">user-details</span></span> | <span data-ttu-id="58f68-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="58f68-119">userDetails</span></span> | <span data-ttu-id="58f68-120">De definir o objeto do usuário que será exibido no controle.</span><span class="sxs-lookup"><span data-stu-id="58f68-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="58f68-121">O exemplo a seguir define os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="58f68-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="58f68-122">A `userDetails` `null` configuração para irá para o estado de saída.</span><span class="sxs-lookup"><span data-stu-id="58f68-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="58f68-123">Use os `loginInitiated` eventos e para manipular a saída e a `logoutInitiated` saída.</span><span class="sxs-lookup"><span data-stu-id="58f68-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="58f68-124">Propriedades personalizadas CSS</span><span class="sxs-lookup"><span data-stu-id="58f68-124">CSS custom properties</span></span>

<span data-ttu-id="58f68-125">O `mgt-login` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="58f68-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="58f68-126">Para saber mais, confira [componentes de estilo](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="58f68-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="58f68-127">Eventos</span><span class="sxs-lookup"><span data-stu-id="58f68-127">Events</span></span>

<span data-ttu-id="58f68-128">Os eventos a seguir são disparados do controle.</span><span class="sxs-lookup"><span data-stu-id="58f68-128">The following events are fired from the control.</span></span>

<span data-ttu-id="58f68-129">Evento</span><span class="sxs-lookup"><span data-stu-id="58f68-129">Event</span></span> | <span data-ttu-id="58f68-130">Quando é emitido</span><span class="sxs-lookup"><span data-stu-id="58f68-130">When is it emitted</span></span> | <span data-ttu-id="58f68-131">Dados personalizados</span><span class="sxs-lookup"><span data-stu-id="58f68-131">Custom data</span></span> | <span data-ttu-id="58f68-132">Cancelável</span><span class="sxs-lookup"><span data-stu-id="58f68-132">Cancelable</span></span> | <span data-ttu-id="58f68-133">Bolhas</span><span class="sxs-lookup"><span data-stu-id="58f68-133">Bubbles</span></span> | <span data-ttu-id="58f68-134">Funciona com modelo personalizado</span><span class="sxs-lookup"><span data-stu-id="58f68-134">Works with custom template</span></span>
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`loginInitiated` | <span data-ttu-id="58f68-135">O usuário clicou no botão entrar para iniciar o processo de logon</span><span class="sxs-lookup"><span data-stu-id="58f68-135">The user clicked the sign in button to start the login process</span></span> | <span data-ttu-id="58f68-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58f68-136">None</span></span> | <span data-ttu-id="58f68-137">Sim</span><span class="sxs-lookup"><span data-stu-id="58f68-137">Yes</span></span> | <span data-ttu-id="58f68-138">Não</span><span class="sxs-lookup"><span data-stu-id="58f68-138">No</span></span> | <span data-ttu-id="58f68-139">Sim</span><span class="sxs-lookup"><span data-stu-id="58f68-139">Yes</span></span>
`loginCompleted` | <span data-ttu-id="58f68-140">O processo de logon foi bem-sucedido e o usuário agora está login</span><span class="sxs-lookup"><span data-stu-id="58f68-140">The login process was successful and the user is now signed in</span></span> | <span data-ttu-id="58f68-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58f68-141">None</span></span> | <span data-ttu-id="58f68-142">Não</span><span class="sxs-lookup"><span data-stu-id="58f68-142">No</span></span> | <span data-ttu-id="58f68-143">Não</span><span class="sxs-lookup"><span data-stu-id="58f68-143">No</span></span> | <span data-ttu-id="58f68-144">Sim</span><span class="sxs-lookup"><span data-stu-id="58f68-144">Yes</span></span>
`loginFailed` | <span data-ttu-id="58f68-145">O usuário cancelou o processo de logon ou não pôde entrar</span><span class="sxs-lookup"><span data-stu-id="58f68-145">The user canceled the login process or was unable to sign in</span></span> | <span data-ttu-id="58f68-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58f68-146">None</span></span> | <span data-ttu-id="58f68-147">Não</span><span class="sxs-lookup"><span data-stu-id="58f68-147">No</span></span> | <span data-ttu-id="58f68-148">Não</span><span class="sxs-lookup"><span data-stu-id="58f68-148">No</span></span> | <span data-ttu-id="58f68-149">Sim</span><span class="sxs-lookup"><span data-stu-id="58f68-149">Yes</span></span>
`logoutInitiated` | <span data-ttu-id="58f68-150">O usuário começou a fazer logout</span><span class="sxs-lookup"><span data-stu-id="58f68-150">The user started to logout</span></span> | <span data-ttu-id="58f68-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58f68-151">None</span></span> | <span data-ttu-id="58f68-152">Sim</span><span class="sxs-lookup"><span data-stu-id="58f68-152">Yes</span></span> | <span data-ttu-id="58f68-153">Não</span><span class="sxs-lookup"><span data-stu-id="58f68-153">No</span></span> | <span data-ttu-id="58f68-154">Sim</span><span class="sxs-lookup"><span data-stu-id="58f68-154">Yes</span></span>
`logoutCompleted` | <span data-ttu-id="58f68-155">O usuário saiu</span><span class="sxs-lookup"><span data-stu-id="58f68-155">The user signed out</span></span> | <span data-ttu-id="58f68-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58f68-156">None</span></span> | <span data-ttu-id="58f68-157">Não</span><span class="sxs-lookup"><span data-stu-id="58f68-157">No</span></span> | <span data-ttu-id="58f68-158">Não</span><span class="sxs-lookup"><span data-stu-id="58f68-158">No</span></span> | <span data-ttu-id="58f68-159">Sim</span><span class="sxs-lookup"><span data-stu-id="58f68-159">Yes</span></span>

<span data-ttu-id="58f68-160">Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).</span><span class="sxs-lookup"><span data-stu-id="58f68-160">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="58f68-161">Modelos</span><span class="sxs-lookup"><span data-stu-id="58f68-161">Templates</span></span>

<span data-ttu-id="58f68-162">O `mgt-login` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="58f68-162">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="58f68-163">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o valor como um dos `<template>` `data-type` valores listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="58f68-163">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="58f68-164">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="58f68-164">Data type</span></span> | <span data-ttu-id="58f68-165">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="58f68-165">Data context</span></span> | <span data-ttu-id="58f68-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="58f68-166">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="58f68-167">signed-in-button-content</span><span class="sxs-lookup"><span data-stu-id="58f68-167">signed-in-button-content</span></span> | <span data-ttu-id="58f68-168">personDetails: objeto person, `personImage` : cadeia de caracteres de imagem da pessoa</span><span class="sxs-lookup"><span data-stu-id="58f68-168">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="58f68-169">O modelo usado para renderizar o conteúdo no botão quando o usuário está assinado.</span><span class="sxs-lookup"><span data-stu-id="58f68-169">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="58f68-170">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="58f68-170">signed-out-button-content</span></span> | <span data-ttu-id="58f68-171">null</span><span class="sxs-lookup"><span data-stu-id="58f68-171">null</span></span> | <span data-ttu-id="58f68-172">O modelo usado para renderizar o conteúdo no botão quando o usuário não estiver assinado.</span><span class="sxs-lookup"><span data-stu-id="58f68-172">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="58f68-173">comandos de sub-</span><span class="sxs-lookup"><span data-stu-id="58f68-173">flyout-commands</span></span> | <span data-ttu-id="58f68-174">handleSignOut: função de saída</span><span class="sxs-lookup"><span data-stu-id="58f68-174">handleSignOut: sign out function</span></span> | <span data-ttu-id="58f68-175">O modelo usado para renderizar os comandos no flyout</span><span class="sxs-lookup"><span data-stu-id="58f68-175">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="58f68-176">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="58f68-176">flyout-person-details</span></span> | <span data-ttu-id="58f68-177">personDetails: objeto person, personImage: cadeia de caracteres de imagem da pessoa</span><span class="sxs-lookup"><span data-stu-id="58f68-177">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="58f68-178">O modelo usado para renderizar os detalhes da pessoa no sobremenu.</span><span class="sxs-lookup"><span data-stu-id="58f68-178">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="58f68-179">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="58f68-179">Microsoft Graph permissions</span></span>

<span data-ttu-id="58f68-180">Este componente usa as seguintes APIs Graph Microsoft e permissões:</span><span class="sxs-lookup"><span data-stu-id="58f68-180">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="58f68-181">Configuração</span><span class="sxs-lookup"><span data-stu-id="58f68-181">Configuration</span></span> | <span data-ttu-id="58f68-182">Permissão</span><span class="sxs-lookup"><span data-stu-id="58f68-182">Permission</span></span> | <span data-ttu-id="58f68-183">API</span><span class="sxs-lookup"><span data-stu-id="58f68-183">API</span></span>
| - | - | - |
| <span data-ttu-id="58f68-184">Padrão.</span><span class="sxs-lookup"><span data-stu-id="58f68-184">default</span></span> | <span data-ttu-id="58f68-185">User.Read</span><span class="sxs-lookup"><span data-stu-id="58f68-185">User.Read</span></span> | [<span data-ttu-id="58f68-186">/users/me/</span><span class="sxs-lookup"><span data-stu-id="58f68-186">/users/me/</span></span>](/graph/api/user-get) |

<span data-ttu-id="58f68-187">Ao usar o padrão e os modelos, esse componente usa o componente Person para exibir o usuário e `signed-in-button-content` `flyout-person-details` herda todas as permissões. [](./person.md)</span><span class="sxs-lookup"><span data-stu-id="58f68-187">When using the default `signed-in-button-content` and `flyout-person-details` templates, this component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span>

## <a name="authentication"></a><span data-ttu-id="58f68-188">Autenticação</span><span class="sxs-lookup"><span data-stu-id="58f68-188">Authentication</span></span>

<span data-ttu-id="58f68-189">O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="58f68-189">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="58f68-190">Cache</span><span class="sxs-lookup"><span data-stu-id="58f68-190">Cache</span></span>

<span data-ttu-id="58f68-191">Esse componente usa o [componente Person](./person.md) para exibir o usuário e herda toda a configuração de cache dele.</span><span class="sxs-lookup"><span data-stu-id="58f68-191">This component uses the [Person component](./person.md) to display the user and inherits all cache configuration from it.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="58f68-192">Estender para obter mais controle</span><span class="sxs-lookup"><span data-stu-id="58f68-192">Extend for more control</span></span>

<span data-ttu-id="58f68-193">Para cenários mais complexos ou um UX realmente personalizado, esse componente expõe vários métodos para substituição `protected render*` em extensões de componentes.</span><span class="sxs-lookup"><span data-stu-id="58f68-193">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="58f68-194">Método</span><span class="sxs-lookup"><span data-stu-id="58f68-194">Method</span></span> | <span data-ttu-id="58f68-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="58f68-195">Description</span></span> |
| - | - |
| <span data-ttu-id="58f68-196">renderButton</span><span class="sxs-lookup"><span data-stu-id="58f68-196">renderButton</span></span> | <span data-ttu-id="58f68-197">Renderiza o botão cromado.</span><span class="sxs-lookup"><span data-stu-id="58f68-197">Renders the button chrome.</span></span> |
| <span data-ttu-id="58f68-198">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="58f68-198">renderButtonContent</span></span> | <span data-ttu-id="58f68-199">Renderiza o conteúdo do botão.</span><span class="sxs-lookup"><span data-stu-id="58f68-199">Renders the button content.</span></span> |
| <span data-ttu-id="58f68-200">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="58f68-200">renderSignedInButtonContent</span></span> | <span data-ttu-id="58f68-201">Renderizar o conteúdo do botão quando o usuário estiver dentro.</span><span class="sxs-lookup"><span data-stu-id="58f68-201">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="58f68-202">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="58f68-202">renderSignedOutButtonContent</span></span> | <span data-ttu-id="58f68-203">Renderizar o conteúdo do botão quando o usuário não estiver assinado.</span><span class="sxs-lookup"><span data-stu-id="58f68-203">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="58f68-204">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="58f68-204">renderFlyout</span></span> | <span data-ttu-id="58f68-205">Renderiza o cromado do flyout.</span><span class="sxs-lookup"><span data-stu-id="58f68-205">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="58f68-206">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="58f68-206">renderFlyoutContent</span></span> | <span data-ttu-id="58f68-207">Renderiza o conteúdo do sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="58f68-207">Renders the flyout content.</span></span> |
| <span data-ttu-id="58f68-208">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="58f68-208">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="58f68-209">Renderizar os detalhes da pessoa do sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="58f68-209">Render the flyout person details.</span></span> |
| <span data-ttu-id="58f68-210">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="58f68-210">renderFlyoutCommands</span></span> | <span data-ttu-id="58f68-211">Renderizar os comandos de sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="58f68-211">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="58f68-212">Traga seu próprio flyout</span><span class="sxs-lookup"><span data-stu-id="58f68-212">Bring your own flyout</span></span>

<span data-ttu-id="58f68-213">É possível usar seu próprio componente sub-1 no lugar do um integrado, substituindo o método e fornecendo `renderFlyout()` o novo sub-20.</span><span class="sxs-lookup"><span data-stu-id="58f68-213">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="58f68-214">Nesse caso, certifique-se de que o componente de logon continue a funcionar conforme o esperado substituindo os métodos de exibição do sobrevoo para atualizar a visibilidade do seu `protected` flyout alternativo.</span><span class="sxs-lookup"><span data-stu-id="58f68-214">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="58f68-215">Método</span><span class="sxs-lookup"><span data-stu-id="58f68-215">Method</span></span> | <span data-ttu-id="58f68-216">Descrição</span><span class="sxs-lookup"><span data-stu-id="58f68-216">Description</span></span> |
| - | - |
| <span data-ttu-id="58f68-217">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="58f68-217">hideFlyout</span></span> | <span data-ttu-id="58f68-218">Descarta o sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="58f68-218">Dismisses the flyout.</span></span> |
| <span data-ttu-id="58f68-219">showFlyout</span><span class="sxs-lookup"><span data-stu-id="58f68-219">showFlyout</span></span> | <span data-ttu-id="58f68-220">Exibe o sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="58f68-220">Displays the flyout.</span></span> |
| <span data-ttu-id="58f68-221">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="58f68-221">toggleFlyout</span></span> | <span data-ttu-id="58f68-222">Alterna o estado do sobrevoo.</span><span class="sxs-lookup"><span data-stu-id="58f68-222">Toggles the state of the flyout.</span></span> |
