---
title: Componente de logon no kit de ferramentas do Microsoft Graph
description: Um componente de logon é um botão e um controle de submenu para facilitar a autenticação da plataforma de identidade da Microsoft.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 3b326cc97bf7a3463e43ffcf757cc34d5cc00975
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639979"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="9d804-103">Componente de logon no kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9d804-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9d804-104">Um componente de logon é um botão e um controle de submenu para facilitar a autenticação da plataforma de identidade da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9d804-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="9d804-105">Ele fornece dois Estados:</span><span class="sxs-lookup"><span data-stu-id="9d804-105">It provides two states:</span></span>
* <span data-ttu-id="9d804-106">Quando o usuário não está conectado, o controle é um botão simples para iniciar o processo de entrada.</span><span class="sxs-lookup"><span data-stu-id="9d804-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="9d804-107">Quando o usuário está conectado, o controle exibe o nome de usuário conectado atual, a imagem de perfil e o email.</span><span class="sxs-lookup"><span data-stu-id="9d804-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="9d804-108">Quando clicado, um submenu é aberto com um comando para sair.</span><span class="sxs-lookup"><span data-stu-id="9d804-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="9d804-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d804-109">Example</span></span>

<span data-ttu-id="9d804-110">O exemplo a seguir mostra `mgt-login` o componente com um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="9d804-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="9d804-111">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="9d804-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="9d804-112">Usando o controle sem um provedor de autenticação</span><span class="sxs-lookup"><span data-stu-id="9d804-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="9d804-113">O componente funciona com um provedor e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9d804-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="9d804-114">No entanto, se você quiser fornecer sua própria lógica e autenticação, você pode usar `userDetails` a propriedade para definir os detalhes do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="9d804-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="9d804-115">Atributo</span><span class="sxs-lookup"><span data-stu-id="9d804-115">Attribute</span></span> | <span data-ttu-id="9d804-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d804-116">Property</span></span> | <span data-ttu-id="9d804-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d804-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="9d804-118">User-detalhes</span><span class="sxs-lookup"><span data-stu-id="9d804-118">user-details</span></span> | <span data-ttu-id="9d804-119">userdetails</span><span class="sxs-lookup"><span data-stu-id="9d804-119">userDetails</span></span> | <span data-ttu-id="9d804-120">Defina o objeto de usuário que será exibido no controle.</span><span class="sxs-lookup"><span data-stu-id="9d804-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="9d804-121">O exemplo a seguir define os detalhes da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9d804-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    email: 'nikola@contoso.com',
    profileImage: 'url'
}
```

<span data-ttu-id="9d804-122">A `userDetails` configuração `null` para vai para o estado de desconectar.</span><span class="sxs-lookup"><span data-stu-id="9d804-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="9d804-123">Use os `loginInitiated` eventos `logoutInitiated` e para lidar com a entrada e a saída.</span><span class="sxs-lookup"><span data-stu-id="9d804-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="9d804-124">Propriedades personalizadas de CSS</span><span class="sxs-lookup"><span data-stu-id="9d804-124">CSS custom properties</span></span>

<span data-ttu-id="9d804-125">O `mgt-login` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="9d804-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="9d804-126">Para saber mais, confira [estilos de componentes](../style.md).</span><span class="sxs-lookup"><span data-stu-id="9d804-126">To learn more, see [styling components](../style.md).</span></span>

## <a name="events"></a><span data-ttu-id="9d804-127">Eventos</span><span class="sxs-lookup"><span data-stu-id="9d804-127">Events</span></span>

<span data-ttu-id="9d804-128">Os eventos a seguir são acionados do controle.</span><span class="sxs-lookup"><span data-stu-id="9d804-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="9d804-129">Evento</span><span class="sxs-lookup"><span data-stu-id="9d804-129">Event</span></span> | <span data-ttu-id="9d804-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d804-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="9d804-131">O usuário clicou no botão entrar para iniciar o processo de logon-cancelable.</span><span class="sxs-lookup"><span data-stu-id="9d804-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="9d804-132">o processo de login foi bem-sucedido e o usuário está conectado.</span><span class="sxs-lookup"><span data-stu-id="9d804-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="9d804-133">O usuário cancelou o processo de logon ou não pôde entrar.</span><span class="sxs-lookup"><span data-stu-id="9d804-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="9d804-134">O usuário iniciou o logout-cancelamento.</span><span class="sxs-lookup"><span data-stu-id="9d804-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="9d804-135">O usuário saiu.</span><span class="sxs-lookup"><span data-stu-id="9d804-135">The user signed out.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="9d804-136">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9d804-136">Microsoft Graph permissions</span></span>

<span data-ttu-id="9d804-137">Este componente usa o [componente Person](./person.md) para exibir o usuário e herda todas as permissões.</span><span class="sxs-lookup"><span data-stu-id="9d804-137">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="9d804-138">Autenticação</span><span class="sxs-lookup"><span data-stu-id="9d804-138">Authentication</span></span>

<span data-ttu-id="9d804-139">O controle de logon usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="9d804-139">The login control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
