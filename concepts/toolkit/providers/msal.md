---
title: Provedor MSAL
description: O provedor MSAL usa MSAL.js para entrar em usuários e adquirir tokens para usar com o microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e612e11e7b1a26765175ba10097c8e54317e9e1d
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579757"
---
# <a name="msal-provider"></a><span data-ttu-id="8263c-103">Provedor MSAL</span><span class="sxs-lookup"><span data-stu-id="8263c-103">MSAL provider</span></span>

<span data-ttu-id="8263c-104">O provedor MSAL usa [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8263c-104">The MSAL provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>

<span data-ttu-id="8263c-105">Para saber mais, confira [provedores](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="8263c-105">To learn more, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="8263c-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="8263c-106">Get started</span></span>

<span data-ttu-id="8263c-107">Você pode inicializar o provedor MSAL em HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8263c-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="8263c-108">Inicializar em sua página HTML</span><span class="sxs-lookup"><span data-stu-id="8263c-108">Initialize in your HTML page</span></span>

<span data-ttu-id="8263c-109">Inicializar o provedor MSAL em HTML é a maneira mais simples de criar um novo provedor.</span><span class="sxs-lookup"><span data-stu-id="8263c-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="8263c-110">Use o `mgt-msal-provider` componente para definir a **id do** cliente e outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="8263c-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="8263c-111">Isso criará uma nova instância que será usada para todos os tokens de autenticação `UserAgentApplication` e aquisição.</span><span class="sxs-lookup"><span data-stu-id="8263c-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""
                   domainHint="mydomain.com"
                   prompt="consent"></mgt-msal-provider>
```

| <span data-ttu-id="8263c-112">Atributo</span><span class="sxs-lookup"><span data-stu-id="8263c-112">Attribute</span></span>    | <span data-ttu-id="8263c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="8263c-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8263c-114">client-id</span><span class="sxs-lookup"><span data-stu-id="8263c-114">client-id</span></span>    | <span data-ttu-id="8263c-115">ID do cliente de cadeia de caracteres (consulte Criando uma ID de aplicativo/cliente).</span><span class="sxs-lookup"><span data-stu-id="8263c-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="8263c-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8263c-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="8263c-117">tipo de logon</span><span class="sxs-lookup"><span data-stu-id="8263c-117">login-type</span></span>   | <span data-ttu-id="8263c-118">Enumeração entre `redirect` e - o valor padrão é `popup` `redirect` .</span><span class="sxs-lookup"><span data-stu-id="8263c-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="8263c-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8263c-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="8263c-120">escopos</span><span class="sxs-lookup"><span data-stu-id="8263c-120">scopes</span></span>       | <span data-ttu-id="8263c-121">Cadeias de caracteres separadas por vírgulas para escopos que o usuário deve consentir ao entrar.</span><span class="sxs-lookup"><span data-stu-id="8263c-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="8263c-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8263c-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="8263c-123">authority</span><span class="sxs-lookup"><span data-stu-id="8263c-123">authority</span></span>    | <span data-ttu-id="8263c-124">Cadeia de caracteres de autoridade - padrão é a autoridade comum.</span><span class="sxs-lookup"><span data-stu-id="8263c-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="8263c-125">Para aplicativos de locatário único, use sua ID de locatário ou nome de locatário.</span><span class="sxs-lookup"><span data-stu-id="8263c-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="8263c-126">Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="8263c-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="8263c-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8263c-127">Optional.</span></span> |
| <span data-ttu-id="8263c-128">redirect-uri</span><span class="sxs-lookup"><span data-stu-id="8263c-128">redirect-uri</span></span> | <span data-ttu-id="8263c-129">Cadeia de caracteres de URI de redirecionamento - por padrão, o URI da janela atual é usado.</span><span class="sxs-lookup"><span data-stu-id="8263c-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="8263c-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8263c-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="8263c-131">depends-on</span><span class="sxs-lookup"><span data-stu-id="8263c-131">depends-on</span></span>   | <span data-ttu-id="8263c-132">Cadeia de caracteres do seletor de elemento de outro componente de provedor de prioridade mais alta.</span><span class="sxs-lookup"><span data-stu-id="8263c-132">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="8263c-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8263c-133">Optional.</span></span> 
| <span data-ttu-id="8263c-134">domain-hint</span><span class="sxs-lookup"><span data-stu-id="8263c-134">domain-hint</span></span>  | <span data-ttu-id="8263c-135">Cadeia de caracteres de consulta do local do domínio para encaminhamento da experiência de login.</span><span class="sxs-lookup"><span data-stu-id="8263c-135">Query string of domain location for forwarding sign in experience.</span></span> <span data-ttu-id="8263c-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8263c-136">Optional.</span></span>              
| <span data-ttu-id="8263c-137">prompt</span><span class="sxs-lookup"><span data-stu-id="8263c-137">prompt</span></span> | <span data-ttu-id="8263c-138">Seleção para o tipo de interação do usuário necessário para fazer logon.</span><span class="sxs-lookup"><span data-stu-id="8263c-138">Selection for type of user interaction required to login.</span></span> <span data-ttu-id="8263c-139">As opções válidas incluem:</span><span class="sxs-lookup"><span data-stu-id="8263c-139">Valid options include:</span></span> <ul><li><span data-ttu-id="8263c-140">`login` força o usuário a inserir credenciais à solicitação</span><span class="sxs-lookup"><span data-stu-id="8263c-140">`login` forces the user to enter credentials on request</span></span> </li><li><span data-ttu-id="8263c-141">`none` para nenhum prompt interativo</span><span class="sxs-lookup"><span data-stu-id="8263c-141">`none` for no interactive prompt</span></span></li> <li><span data-ttu-id="8263c-142">`select_account` para enviar o usuário para um selador de conta</span><span class="sxs-lookup"><span data-stu-id="8263c-142">`select_account` to send the user to an account picker</span></span></li><li><span data-ttu-id="8263c-143">`consent` para enviar o usuário para uma caixa de diálogo de consentimento OAuth</span><span class="sxs-lookup"><span data-stu-id="8263c-143">`consent` to send the user to a OAuth consent dialog</span></span></li></ul> <span data-ttu-id="8263c-144">Para obter mais informações de prompt, consulte [o comportamento do prompt no MSAL.js](/azure/active-directory/develop/msal-js-prompt-behavior) artigo.</span><span class="sxs-lookup"><span data-stu-id="8263c-144">For more prompt information, see the [prompt behavior in MSAL.js](/azure/active-directory/develop/msal-js-prompt-behavior) article.</span></span> <span data-ttu-id="8263c-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8263c-145">Optional.</span></span>                                                                                                                                                                            |


### <a name="initialize-in-javascript"></a><span data-ttu-id="8263c-146">Inicializar em JavaScript</span><span class="sxs-lookup"><span data-stu-id="8263c-146">Initialize in JavaScript</span></span>

<span data-ttu-id="8263c-147">Você pode fornecer mais opções inicializando o provedor em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8263c-147">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="8263c-148">Você pode configurar o `MsalProvider` parâmetro construtor de duas maneiras, conforme descrito nas seções a seguir.</span><span class="sxs-lookup"><span data-stu-id="8263c-148">You can configure the `MsalProvider` constructor parameter in two ways, as described in the following sections.</span></span>

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a><span data-ttu-id="8263c-149">Fornecer um `clientId` para criar um novo `UserAgentApplication`</span><span class="sxs-lookup"><span data-stu-id="8263c-149">Provide a `clientId` to create a new `UserAgentApplication`</span></span>

<span data-ttu-id="8263c-150">Essa opção faz sentido quando Graph Toolkit é responsável por toda a autenticação em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8263c-150">This option makes sense when Graph Toolkit is responsible for all authentication in your application.</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
  domainHint?: string;
  prompt?: string; // "login", "none", "select_account", "consent"
}
```

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a><span data-ttu-id="8263c-151">Passe um existente `UserAgentApplication` na `userAgentApplication` propriedade.</span><span class="sxs-lookup"><span data-stu-id="8263c-151">Pass an existing `UserAgentApplication` in the `userAgentApplication` property.</span></span>

<span data-ttu-id="8263c-152">Use isso quando seu aplicativo usa a funcionalidade MSAL além do que é exposto pelos recursos `MsalProvider` do Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="8263c-152">Use this when your app uses MSAL functionality beyond what's exposed by the `MsalProvider` and other Microsoft Graph Toolkit features.</span></span> <span data-ttu-id="8263c-153">Isso é particularmente apropriado se uma estrutura instancie e exponha automaticamente um para você; por exemplo, ao `UserAgentApplication` usar [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).</span><span class="sxs-lookup"><span data-stu-id="8263c-153">This is particularly appropriate if a framework automatically instantiates and exposes a `UserAgentApplication` for you; for example, when using [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).</span></span>

<span data-ttu-id="8263c-154">Certifique-se de entender as oportunidades de colisões ao usar essa opção.</span><span class="sxs-lookup"><span data-stu-id="8263c-154">Be sure to understand opportunities for collisions when using this option.</span></span> <span data-ttu-id="8263c-155">Por sua própria natureza, há o risco de que o estado de uma sessão possa mudar, por exemplo, fazendo com que o usuário entre ou consenta com `MsalProvider` escopos adicionais.</span><span class="sxs-lookup"><span data-stu-id="8263c-155">By its very nature, there is a risk that the `MsalProvider` can change the state of a session, for example by having the user sign in or consent to additional scopes.</span></span> <span data-ttu-id="8263c-156">Certifique-se de que seu aplicativo e outras estruturas respondam normalmente a essas alterações no estado ou considere usar um [provedor personalizado](./custom.md) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="8263c-156">Make sure that your app and other frameworks respond gracefully to these changes in state, or consider using a [custom provider](./custom.md) instead.</span></span>

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

<span data-ttu-id="8263c-157">Para saber mais sobre MSAL.js opções adicionais que você pode usar ao inicializar a biblioteca MSAL, consulte a [documentação MSAL](/azure/active-directory/develop/msal-js-initializing-client-applications).</span><span class="sxs-lookup"><span data-stu-id="8263c-157">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="8263c-158">Criando uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="8263c-158">Creating an app/client ID</span></span>

<span data-ttu-id="8263c-159">Para obter detalhes sobre como registrar um aplicativo e obter uma ID do cliente, consulte [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span><span class="sxs-lookup"><span data-stu-id="8263c-159">For details about how to register an app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>
