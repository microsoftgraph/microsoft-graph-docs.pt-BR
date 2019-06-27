---
title: Componente de logon no kit de ferramentas do Microsoft Graph
description: Um componente de logon é um botão e um controle de submenu para facilitar a autenticação da plataforma de identidade da Microsoft.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e7c657b3b6c9772b2d7b7b8e64a57c9982f4caef
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242944"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="727bd-103">Componente de logon no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="727bd-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="727bd-104">Um componente de logon é um botão e um controle de submenu para facilitar a autenticação da plataforma de identidade da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="727bd-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="727bd-105">Ele fornece dois Estados:</span><span class="sxs-lookup"><span data-stu-id="727bd-105">It provides two states:</span></span>
* <span data-ttu-id="727bd-106">Quando o usuário não está conectado, o controle é um botão simples para iniciar o processo de entrada.</span><span class="sxs-lookup"><span data-stu-id="727bd-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="727bd-107">Quando o usuário está conectado, o controle exibe o nome de usuário conectado atual, a imagem de perfil e o email.</span><span class="sxs-lookup"><span data-stu-id="727bd-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="727bd-108">Quando clicado, um submenu é aberto com um comando para sair.</span><span class="sxs-lookup"><span data-stu-id="727bd-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="727bd-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="727bd-109">Example</span></span>

[<span data-ttu-id="727bd-110">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="727bd-110">jsfiddle example</span></span>](https://jsfiddle.net/metulev/scb9muh4)

```html
<mgt-login></mgt-login>
```

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="727bd-111">Usando o controle sem um provedor de autenticação</span><span class="sxs-lookup"><span data-stu-id="727bd-111">Using the control without an authentication provider</span></span>

<span data-ttu-id="727bd-112">O componente funciona com um provedor e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="727bd-112">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="727bd-113">No entanto, se você quiser fornecer sua própria lógica e autenticação, você pode usar `userDetails` a propriedade para definir os detalhes do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="727bd-113">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="727bd-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="727bd-114">Property</span></span> | <span data-ttu-id="727bd-115">Atributo</span><span class="sxs-lookup"><span data-stu-id="727bd-115">Attribute</span></span> | <span data-ttu-id="727bd-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="727bd-116">Description</span></span> |
| --- | --- | -- |
| `userDetails` | `user-details` | <span data-ttu-id="727bd-117">Defina o objeto de usuário que será exibido no controle.</span><span class="sxs-lookup"><span data-stu-id="727bd-117">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="727bd-118">O exemplo a seguir define os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="727bd-118">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    email: 'nikola@contoso.com',
    profileImage: 'url'
}
```

<span data-ttu-id="727bd-119">A `userDetails` configuração `null` para vai para o estado de desconectar.</span><span class="sxs-lookup"><span data-stu-id="727bd-119">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="727bd-120">Use os `loginInitiated` eventos `logoutInitiated` e para lidar com a entrada e a saída.</span><span class="sxs-lookup"><span data-stu-id="727bd-120">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="727bd-121">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="727bd-121">CSS custom properties</span></span>

<span data-ttu-id="727bd-122">O `mgt-login` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="727bd-122">The `mgt-login` component defines the following CSS custom properties.</span></span>

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --color: #201f1e;
  --background-color: transparent;
  --background-color--hover: #edebe9;
  --popup-content-background-color: white;
  --popup-command-font-size: 12px; }
}
```

<span data-ttu-id="727bd-123">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="727bd-123">To learn more, see [styling components](../style.md).</span></span>

## <a name="events"></a><span data-ttu-id="727bd-124">Eventos</span><span class="sxs-lookup"><span data-stu-id="727bd-124">Events</span></span>

<span data-ttu-id="727bd-125">Os eventos a seguir são acionados do controle.</span><span class="sxs-lookup"><span data-stu-id="727bd-125">The following events are fired from the control.</span></span>

| <span data-ttu-id="727bd-126">Evento</span><span class="sxs-lookup"><span data-stu-id="727bd-126">Event</span></span> | <span data-ttu-id="727bd-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="727bd-127">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="727bd-128">O usuário clicou no botão entrar para iniciar o processo de logon-cancelable.</span><span class="sxs-lookup"><span data-stu-id="727bd-128">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="727bd-129">o processo de login foi bem-sucedido e o usuário está conectado.</span><span class="sxs-lookup"><span data-stu-id="727bd-129">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="727bd-130">O usuário cancelou o processo de logon ou não pôde entrar.</span><span class="sxs-lookup"><span data-stu-id="727bd-130">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="727bd-131">O usuário iniciou o logout-cancelamento.</span><span class="sxs-lookup"><span data-stu-id="727bd-131">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="727bd-132">O usuário saiu.</span><span class="sxs-lookup"><span data-stu-id="727bd-132">The user signed out.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="727bd-133">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="727bd-133">Microsoft Graph permissions</span></span>

<span data-ttu-id="727bd-134">Este componente usa o [componente Person](./person.md) para exibir o usuário e herda todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="727bd-134">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="727bd-135">Autenticação</span><span class="sxs-lookup"><span data-stu-id="727bd-135">Authentication</span></span>

<span data-ttu-id="727bd-136">O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="727bd-136">The login control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
