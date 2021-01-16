---
title: Provedor MSAL
description: O provedor MSAL usa MSAL.js para entrar usuários e adquirir tokens para usar com o Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 738e8ebcd24b3e7e528bdf0a1676dd54103ee2ea
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883022"
---
# <a name="msal-provider"></a><span data-ttu-id="44f10-103">Provedor MSAL</span><span class="sxs-lookup"><span data-stu-id="44f10-103">MSAL provider</span></span>

<span data-ttu-id="44f10-104">O provedor MSAL usa [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) para entrar usuários e adquirir tokens para usar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="44f10-104">The MSAL provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>

<span data-ttu-id="44f10-105">Para saber mais, consulte [provedores.](./providers.md)</span><span class="sxs-lookup"><span data-stu-id="44f10-105">To learn more, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="44f10-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="44f10-106">Get started</span></span>

<span data-ttu-id="44f10-107">Você pode inicializar o provedor MSAL em HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="44f10-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="44f10-108">Inicializar em sua página HTML</span><span class="sxs-lookup"><span data-stu-id="44f10-108">Initialize in your HTML page</span></span>

<span data-ttu-id="44f10-109">Inicializar o provedor MSAL em HTML é a maneira mais simples de criar um novo provedor.</span><span class="sxs-lookup"><span data-stu-id="44f10-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="44f10-110">Use o `mgt-msal-provider` componente para definir a **ID do cliente** e outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="44f10-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="44f10-111">Isso criará uma nova `UserAgentApplication` instância que será usada para toda a autenticação e aquisição de tokens.</span><span class="sxs-lookup"><span data-stu-id="44f10-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="44f10-112">Atributo</span><span class="sxs-lookup"><span data-stu-id="44f10-112">Attribute</span></span>    | <span data-ttu-id="44f10-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="44f10-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="44f10-114">client-id</span><span class="sxs-lookup"><span data-stu-id="44f10-114">client-id</span></span>    | <span data-ttu-id="44f10-115">ID do cliente de cadeia de caracteres (consulte Criando uma ID de aplicativo/cliente).</span><span class="sxs-lookup"><span data-stu-id="44f10-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="44f10-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44f10-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="44f10-117">tipo de logon</span><span class="sxs-lookup"><span data-stu-id="44f10-117">login-type</span></span>   | <span data-ttu-id="44f10-118">Enumeração entre `redirect` e - o valor padrão é `popup` `redirect` .</span><span class="sxs-lookup"><span data-stu-id="44f10-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="44f10-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="44f10-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="44f10-120">escopos</span><span class="sxs-lookup"><span data-stu-id="44f10-120">scopes</span></span>       | <span data-ttu-id="44f10-121">Cadeias de caracteres separadas por vírgulas para escopos que o usuário deve consentir ao entrar.</span><span class="sxs-lookup"><span data-stu-id="44f10-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="44f10-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="44f10-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="44f10-123">autoridade</span><span class="sxs-lookup"><span data-stu-id="44f10-123">authority</span></span>    | <span data-ttu-id="44f10-124">Cadeia de caracteres de autoridade – o padrão é a autoridade comum.</span><span class="sxs-lookup"><span data-stu-id="44f10-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="44f10-125">Para aplicativos de locatário único, use a ID do locatário ou o nome do locatário.</span><span class="sxs-lookup"><span data-stu-id="44f10-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="44f10-126">Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="44f10-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="44f10-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="44f10-127">Optional.</span></span> |
| <span data-ttu-id="44f10-128">redirect-uri</span><span class="sxs-lookup"><span data-stu-id="44f10-128">redirect-uri</span></span> | <span data-ttu-id="44f10-129">Cadeia de caracteres de URI de redirecionamento - por padrão, o URI da janela atual é usado.</span><span class="sxs-lookup"><span data-stu-id="44f10-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="44f10-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="44f10-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="44f10-131">depende</span><span class="sxs-lookup"><span data-stu-id="44f10-131">depends-on</span></span>   | <span data-ttu-id="44f10-132">Cadeia de caracteres do seletor de elemento de outro componente de provedor de prioridade mais alta.</span><span class="sxs-lookup"><span data-stu-id="44f10-132">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="44f10-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="44f10-133">Optional.</span></span>                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a><span data-ttu-id="44f10-134">Inicializar em JavaScript</span><span class="sxs-lookup"><span data-stu-id="44f10-134">Initialize in JavaScript</span></span>

<span data-ttu-id="44f10-135">Você pode fornecer mais opções inicializando o provedor em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="44f10-135">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="44f10-136">Você pode configurar o `MsalProvider` parâmetro do construtor de duas maneiras, conforme descrito nas seções a seguir.</span><span class="sxs-lookup"><span data-stu-id="44f10-136">You can configure the `MsalProvider` constructor parameter in two ways, as described in the following sections.</span></span>

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a><span data-ttu-id="44f10-137">Fornecer um `clientId` para criar um novo `UserAgentApplication`</span><span class="sxs-lookup"><span data-stu-id="44f10-137">Provide a `clientId` to create a new `UserAgentApplication`</span></span>

<span data-ttu-id="44f10-138">Essa opção faz sentido quando o Graph Toolkit é responsável por toda a autenticação em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44f10-138">This option makes sense when Graph Toolkit is responsible for all authentication in your application.</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
}
```

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a><span data-ttu-id="44f10-139">Passe um existente `UserAgentApplication` na `userAgentApplication` propriedade.</span><span class="sxs-lookup"><span data-stu-id="44f10-139">Pass an existing `UserAgentApplication` in the `userAgentApplication` property.</span></span>

<span data-ttu-id="44f10-140">Use isso quando seu aplicativo usa a funcionalidade MSAL além do que é exposto pelos recursos e outros recursos do `MsalProvider` Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="44f10-140">Use this when your app uses MSAL functionality beyond what's exposed by the `MsalProvider` and other Microsoft Graph Toolkit features.</span></span> <span data-ttu-id="44f10-141">Isso é particularmente apropriado se uma estrutura instanciá-la automaticamente e expor uma para você; por exemplo, ao usar `UserAgentApplication` [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).</span><span class="sxs-lookup"><span data-stu-id="44f10-141">This is particularly appropriate if a framework automatically instantiates and exposes a `UserAgentApplication` for you; for example, when using [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).</span></span>

<span data-ttu-id="44f10-142">Certifique-se de entender as oportunidades de colisões ao usar essa opção.</span><span class="sxs-lookup"><span data-stu-id="44f10-142">Be sure to understand opportunities for collisions when using this option.</span></span> <span data-ttu-id="44f10-143">Por sua própria natureza, há um risco de que o estado de uma sessão possa ser diferente, por exemplo, fazendo o usuário entrar ou consentir com `MsalProvider` escopos adicionais.</span><span class="sxs-lookup"><span data-stu-id="44f10-143">By its very nature, there is a risk that the `MsalProvider` can change the state of a session, for example by having the user sign in or consent to additional scopes.</span></span> <span data-ttu-id="44f10-144">Certifique-se de que seu aplicativo e outras estruturas respondam normalmente a essas alterações de estado ou considere usar um [provedor personalizado.](./custom.md)</span><span class="sxs-lookup"><span data-stu-id="44f10-144">Make sure that your app and other frameworks respond gracefully to these changes in state, or consider using a [custom provider](./custom.md) instead.</span></span>

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

<span data-ttu-id="44f10-145">Para saber mais sobre MSAL.js e para opções adicionais que você pode usar ao inicializar a biblioteca MSAL, consulte a documentação [da MSAL.](/azure/active-directory/develop/msal-js-initializing-client-applications)</span><span class="sxs-lookup"><span data-stu-id="44f10-145">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="44f10-146">Criando uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="44f10-146">Creating an app/client ID</span></span>

<span data-ttu-id="44f10-147">Para obter detalhes sobre como registrar um aplicativo e obter uma ID de cliente, consulte [Criar um aplicativo do Azure Active Directory.](../get-started/add-aad-app-registration.md)</span><span class="sxs-lookup"><span data-stu-id="44f10-147">For details about how to register an app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>