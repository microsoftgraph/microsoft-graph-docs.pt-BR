---
title: Provedor MSAL 2
description: O provedor MSAL 2 usa o msal-browser para entrar em usuários e adquirir tokens para usar com o microsoft Graph
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: f583845f5c1929669242323501d08fa4a861197e
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579785"
---
# <a name="msal-2--provider"></a><span data-ttu-id="7dc76-103">Provedor MSAL 2</span><span class="sxs-lookup"><span data-stu-id="7dc76-103">MSAL 2  provider</span></span>

<span data-ttu-id="7dc76-104">O provedor MSAL 2 usa [o msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) para entrar nos usuários e adquirir tokens para usar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7dc76-104">The MSAL 2 provider uses [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>
<span data-ttu-id="7dc76-105">Para saber mais, confira [provedores](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="7dc76-105">To learn more, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="7dc76-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="7dc76-106">Get started</span></span>

<span data-ttu-id="7dc76-107">Você pode inicializar o provedor MSAL 2.0 em HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="7dc76-107">You can initialize the MSAL 2.0 provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="7dc76-108">Inicializar em sua página HTML</span><span class="sxs-lookup"><span data-stu-id="7dc76-108">Initialize in your HTML page</span></span>

<span data-ttu-id="7dc76-109">Inicializar o provedor MSAL 2 em HTML é a maneira mais simples de criar um novo provedor.</span><span class="sxs-lookup"><span data-stu-id="7dc76-109">Initializing the MSAL 2 provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="7dc76-110">Use o `mgt-msal2-provider` componente para definir a **id do** cliente e outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="7dc76-110">Use the `mgt-msal2-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="7dc76-111">Isso criará uma nova instância que será usada para todos os tokens de autenticação `PublicClientApplication` e aquisição.</span><span class="sxs-lookup"><span data-stu-id="7dc76-111">This will create a new `PublicClientApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
    <mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"
                        login-type="redirect/popup" 
                        scopes="user.read,people.read" 
                        redirect-uri="https://my.redirect/uri" 
                        authority=""> 
    </mgt-msal2-provider> 
```

| <span data-ttu-id="7dc76-112">Atributo</span><span class="sxs-lookup"><span data-stu-id="7dc76-112">Attribute</span></span>    | <span data-ttu-id="7dc76-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dc76-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7dc76-114">client-id</span><span class="sxs-lookup"><span data-stu-id="7dc76-114">client-id</span></span>    | <span data-ttu-id="7dc76-115">ID do cliente de cadeia de caracteres (consulte Criando uma ID de aplicativo/cliente).</span><span class="sxs-lookup"><span data-stu-id="7dc76-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="7dc76-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dc76-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="7dc76-117">tipo de logon</span><span class="sxs-lookup"><span data-stu-id="7dc76-117">login-type</span></span>   | <span data-ttu-id="7dc76-118">Enumeração entre `redirect` e - o valor padrão é `popup` `redirect` .</span><span class="sxs-lookup"><span data-stu-id="7dc76-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="7dc76-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7dc76-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="7dc76-120">escopos</span><span class="sxs-lookup"><span data-stu-id="7dc76-120">scopes</span></span>       | <span data-ttu-id="7dc76-121">Cadeias de caracteres separadas por vírgulas para escopos que o usuário deve consentir ao entrar.</span><span class="sxs-lookup"><span data-stu-id="7dc76-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="7dc76-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7dc76-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="7dc76-123">authority</span><span class="sxs-lookup"><span data-stu-id="7dc76-123">authority</span></span>    | <span data-ttu-id="7dc76-124">Cadeia de caracteres de autoridade - padrão é a autoridade comum.</span><span class="sxs-lookup"><span data-stu-id="7dc76-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="7dc76-125">Para aplicativos de locatário único, use sua ID de locatário ou nome de locatário.</span><span class="sxs-lookup"><span data-stu-id="7dc76-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="7dc76-126">Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="7dc76-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="7dc76-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7dc76-127">Optional.</span></span> |
| <span data-ttu-id="7dc76-128">redirect-uri</span><span class="sxs-lookup"><span data-stu-id="7dc76-128">redirect-uri</span></span> | <span data-ttu-id="7dc76-129">Cadeia de caracteres de URI de redirecionamento - por padrão, o URI da janela atual é usado.</span><span class="sxs-lookup"><span data-stu-id="7dc76-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="7dc76-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7dc76-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="7dc76-131">prompt</span><span class="sxs-lookup"><span data-stu-id="7dc76-131">prompt</span></span>       | <span data-ttu-id="7dc76-132">Tipo de prompt a ser usado para logon, entre ```SELECT_ACCOUNT``` e ```CONSENT``` ```LOGIN``` .</span><span class="sxs-lookup"><span data-stu-id="7dc76-132">Type of prompt to use for login, between ```SELECT_ACCOUNT```, ```CONSENT``` and ```LOGIN```.</span></span> <span data-ttu-id="7dc76-133">O padrão é ```SELECT_ACCOUNT```.</span><span class="sxs-lookup"><span data-stu-id="7dc76-133">Default is ```SELECT_ACCOUNT```.</span></span> <span data-ttu-id="7dc76-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7dc76-134">Optional.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="7dc76-135">Inicializar em JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dc76-135">Initialize in JavaScript</span></span>

<span data-ttu-id="7dc76-136">Você pode fornecer mais opções inicializando o provedor em JavaScript.</span><span class="sxs-lookup"><span data-stu-id="7dc76-136">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
    import {Providers, LoginType} from '@microsoft/mgt-element';
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';

    // initialize the auth provider globally
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID',
      scopes?: string[],
      authority?: string,
      redirectUri?: string,
      loginType?: LoginType, // LoginType.Popup or LoginType.Redirect (redirect is default)
      prompt?: PromptType, // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
      sid?: string, // Session ID
      loginHint?: string,
      domainHint?: string,
      options?: Configuration // msal js Configuration object
    });
```

## <a name="creating-an-appclient-id"></a><span data-ttu-id="7dc76-137">Criando uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="7dc76-137">Creating an app/client ID</span></span>

<span data-ttu-id="7dc76-138">Para obter detalhes sobre como registrar um aplicativo e obter uma ID do cliente, consulte [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span><span class="sxs-lookup"><span data-stu-id="7dc76-138">For details about how to register an app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>

## <a name="difference-between-msal2provider-and-msalprovider"></a><span data-ttu-id="7dc76-139">Diferença entre Msal2Provider e MsalProvider</span><span class="sxs-lookup"><span data-stu-id="7dc76-139">Difference between Msal2Provider and MsalProvider</span></span>
<span data-ttu-id="7dc76-140">Embora o uso seja muito semelhante, MsalProvider e Msal2Provider são construídos em cima de fluxos OAuth diferentes.</span><span class="sxs-lookup"><span data-stu-id="7dc76-140">Although the usage is very similar, MsalProvider and Msal2Provider are built on top of different OAuth flows.</span></span> <span data-ttu-id="7dc76-141">O MsalProvider é criado sobre o MSAL.js, que implementa o Flow [.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)</span><span class="sxs-lookup"><span data-stu-id="7dc76-141">MsalProvider is built on top of MSAL.js, which implements the OAuth2.0 [Implicit Grant Flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span> <span data-ttu-id="7dc76-142">Msal2Provider é criado sobre [o msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser), que implementa o código de autorização [OAuth](/azure/active-directory/develop/v2-oauth2-auth-code-flow) 2.0 Flow com PKCE.</span><span class="sxs-lookup"><span data-stu-id="7dc76-142">Msal2Provider is built on top of [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser), which implements the OAuth 2.0 [Authorization Code Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow) with PKCE.</span></span>
<span data-ttu-id="7dc76-143">O Código de Autorização Flow é considerado mais seguro do que a concessão implícita Flow aplicativos Web, portanto, recomendamos o uso do MSAL2Provider sobre o MSALProvider.</span><span class="sxs-lookup"><span data-stu-id="7dc76-143">Authorization Code Flow is deemed more secure than Implicit Grant Flow for web applications, so we recommend usage of MSAL2Provider over MSALProvider.</span></span> <span data-ttu-id="7dc76-144">Para obter detalhes sobre problemas de segurança relacionados ao fluxo de concessão implícito, consulte [Desvantagens do fluxo implícito](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6).</span><span class="sxs-lookup"><span data-stu-id="7dc76-144">For details about security issues related to implicit grant flow, see [Disadvantages of the implicit flow](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6).</span></span>

## <a name="migrating-from-msal-provider-to-msal-2-provider"></a><span data-ttu-id="7dc76-145">Migrando do provedor MSAL para o provedor MSAL 2</span><span class="sxs-lookup"><span data-stu-id="7dc76-145">Migrating from MSAL Provider to MSAL 2 Provider</span></span>
<span data-ttu-id="7dc76-146">Para migrar um aplicativo que está usando o provedor MSAL para o Provedor MSAL 2:</span><span class="sxs-lookup"><span data-stu-id="7dc76-146">To migrate an application that's using MSAL provider to the MSAL 2 Provider:</span></span>
1. <span data-ttu-id="7dc76-147">Vá para o portal do Azure em https://portal.azure.com .</span><span class="sxs-lookup"><span data-stu-id="7dc76-147">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="7dc76-148">No menu, selecione **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="7dc76-148">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="7dc76-149">No menu Azure Active Directory, selecione **Registros de aplicativos**.</span><span class="sxs-lookup"><span data-stu-id="7dc76-149">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="7dc76-150">Selecione o registro do aplicativo do aplicativo que você está usando no momento.</span><span class="sxs-lookup"><span data-stu-id="7dc76-150">Select the app registration of the app that you're currently using.</span></span> 
1. <span data-ttu-id="7dc76-151">Vá para **Autenticação** no menu esquerdo.</span><span class="sxs-lookup"><span data-stu-id="7dc76-151">Go to **Authentication** on the left menu.</span></span>
1. <span data-ttu-id="7dc76-152">Em **Configurações de plataforma,** clique em **Adicionar uma plataforma** e selecione Aplicativo de página **única.**</span><span class="sxs-lookup"><span data-stu-id="7dc76-152">Under **Platform configurations**, click on **Add a platform** and select **Single-page Application**.</span></span>
1. <span data-ttu-id="7dc76-153">Remova todas as URIs de redirecionamento que você registrou no momento na **Web** e, em vez disso, **adicione-as** em aplicativo de página única.</span><span class="sxs-lookup"><span data-stu-id="7dc76-153">Remove all the redirect URIs that you have currently registered under **Web**, and instead add them under **Single-page application**.</span></span>
1. <span data-ttu-id="7dc76-154">Em seu código, substitua MSALProvider por MSAL2Provider.</span><span class="sxs-lookup"><span data-stu-id="7dc76-154">In your code, replace MSALProvider with MSAL2Provider.</span></span>

    <span data-ttu-id="7dc76-155">Se você estiver inicializando seu provedor no código JS/TS, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="7dc76-155">If you are initializing your provider in the JS/TS code, follow these steps:</span></span>
    
    <span data-ttu-id="7dc76-156">Substitua a instrução import ```mgt-msal-provider``` por</span><span class="sxs-lookup"><span data-stu-id="7dc76-156">Replace the import statement for ```mgt-msal-provider``` with</span></span> 
    ```ts 
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';
    ```

    <span data-ttu-id="7dc76-157">Substituir a inicialização de MsalProvider por</span><span class="sxs-lookup"><span data-stu-id="7dc76-157">Replace the initialization of MsalProvider with</span></span>
    ```ts
    Providers.globalProvider = new Msal2Provider({ 
      clientId: 'REPLACE_WITH_CLIENTID'
      ...
    })
    ```
    <span data-ttu-id="7dc76-158">Se você estiver inicializando o provedor em HTML, substitua</span><span class="sxs-lookup"><span data-stu-id="7dc76-158">If you are initializing the provider in HTML, replace</span></span> 
    ```html
    <mgt-msal-provider client-id="" ... ></mgt-msal-provider>
    ``` 
    <span data-ttu-id="7dc76-159">com</span><span class="sxs-lookup"><span data-stu-id="7dc76-159">with</span></span> 
    ```html
    <mgt-msal2-provider  client-id="" ... ></mgt-msal2-provider>
     ```
    <span data-ttu-id="7dc76-160">Para obter detalhes, [consulte Inicializar em sua página HTML](#initialize-in-your-html-page).</span><span class="sxs-lookup"><span data-stu-id="7dc76-160">For details, see [Initialize in your HTML page](#initialize-in-your-html-page).</span></span>
