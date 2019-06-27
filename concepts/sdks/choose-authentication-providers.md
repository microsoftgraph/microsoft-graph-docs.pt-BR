---
title: Escolher um provedor de autenticação do Microsoft Graph
description: Saiba como escolher provedores de autenticação específicos do cenário para seu aplicativo.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 8f69312b4993320e76e2fe46a2977d98c0a42c93
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275555"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="c2e35-103">Escolher um provedor de autenticação do Microsoft Graph com base no cenário</span><span class="sxs-lookup"><span data-stu-id="c2e35-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="c2e35-104">Os provedores de autenticação implementam o código necessário para adquirir um token usando a biblioteca de autenticação da Microsoft (MSAL); gerenciar vários erros potenciais para casos como o consentimento incremental, senhas expiradas e acesso condicional; e, em seguida, defina o cabeçalho de autorização da solicitação HTTP.</span><span class="sxs-lookup"><span data-stu-id="c2e35-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="c2e35-105">A tabela a seguir lista o conjunto de provedores que correspondem aos cenários para diferentes [tipos de aplicativos](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types).</span><span class="sxs-lookup"><span data-stu-id="c2e35-105">The following table lists the set of providers that match the scenarios for different [application types](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="c2e35-106">Cenário</span><span class="sxs-lookup"><span data-stu-id="c2e35-106">Scenario</span></span> | <span data-ttu-id="c2e35-107">Fluxo/concessão</span><span class="sxs-lookup"><span data-stu-id="c2e35-107">Flow/Grant</span></span> | <span data-ttu-id="c2e35-108">Público-alvo</span><span class="sxs-lookup"><span data-stu-id="c2e35-108">Audience</span></span> | <span data-ttu-id="c2e35-109">Provedor</span><span class="sxs-lookup"><span data-stu-id="c2e35-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="c2e35-110">Aplicativo de página única</span><span class="sxs-lookup"><span data-stu-id="c2e35-110">Single Page App</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="c2e35-111">Implícito</span><span class="sxs-lookup"><span data-stu-id="c2e35-111">Implicit</span></span> | <span data-ttu-id="c2e35-112">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="c2e35-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="c2e35-113">Provedor implícito</span><span class="sxs-lookup"><span data-stu-id="c2e35-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="c2e35-114">Aplicativo Web que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="c2e35-114">Web App that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="c2e35-115">Código de Autorização</span><span class="sxs-lookup"><span data-stu-id="c2e35-115">Authorization Code</span></span> | <span data-ttu-id="c2e35-116">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="c2e35-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="c2e35-117">Provedor de código de autorização</span><span class="sxs-lookup"><span data-stu-id="c2e35-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="c2e35-118">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="c2e35-118">Client Credentials</span></span>  | <span data-ttu-id="c2e35-119">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2e35-119">App Only</span></span> | [<span data-ttu-id="c2e35-120">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="c2e35-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="c2e35-121">API Web que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="c2e35-121">Web API that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="c2e35-122">Em nome de</span><span class="sxs-lookup"><span data-stu-id="c2e35-122">On Behalf Of</span></span> | <span data-ttu-id="c2e35-123">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="c2e35-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="c2e35-124">Em nome do provedor</span><span class="sxs-lookup"><span data-stu-id="c2e35-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="c2e35-125">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="c2e35-125">Client Credentials</span></span>  | <span data-ttu-id="c2e35-126">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2e35-126">App Only</span></span> | [<span data-ttu-id="c2e35-127">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="c2e35-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="c2e35-128">Aplicativo de área de trabalho que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="c2e35-128">Desktop app that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="c2e35-129">Interativo</span><span class="sxs-lookup"><span data-stu-id="c2e35-129">Interactive</span></span> | <span data-ttu-id="c2e35-130">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="c2e35-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="c2e35-131">Provedor interativo</span><span class="sxs-lookup"><span data-stu-id="c2e35-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="c2e35-132">Integrada do Windows</span><span class="sxs-lookup"><span data-stu-id="c2e35-132">Integrated Windows</span></span> | <span data-ttu-id="c2e35-133">Organização delegada</span><span class="sxs-lookup"><span data-stu-id="c2e35-133">Delegated Org</span></span> | [<span data-ttu-id="c2e35-134">Provedor integrado do Windows</span><span class="sxs-lookup"><span data-stu-id="c2e35-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="c2e35-135">Proprietário do recurso</span><span class="sxs-lookup"><span data-stu-id="c2e35-135">Resource Owner</span></span>  | <span data-ttu-id="c2e35-136">Organização delegada</span><span class="sxs-lookup"><span data-stu-id="c2e35-136">Delegated Org</span></span> | [<span data-ttu-id="c2e35-137">Provedor de nome de usuário/senha</span><span class="sxs-lookup"><span data-stu-id="c2e35-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="c2e35-138">Código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c2e35-138">Device Code</span></span>  | <span data-ttu-id="c2e35-139">Organização delegada</span><span class="sxs-lookup"><span data-stu-id="c2e35-139">Delegated Org</span></span> | [<span data-ttu-id="c2e35-140">Provedor de código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c2e35-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="c2e35-141">Aplicativo daemon</span><span class="sxs-lookup"><span data-stu-id="c2e35-141">Daemon app</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="c2e35-142">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="c2e35-142">Client Credentials</span></span>  | <span data-ttu-id="c2e35-143">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2e35-143">App Only</span></span> | [<span data-ttu-id="c2e35-144">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="c2e35-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="c2e35-145">Aplicativo móvel que chama as APIs Web</span><span class="sxs-lookup"><span data-stu-id="c2e35-145">Mobile app that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="c2e35-146">Interativo</span><span class="sxs-lookup"><span data-stu-id="c2e35-146">Interactive</span></span> | <span data-ttu-id="c2e35-147">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="c2e35-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="c2e35-148">Provedor interativo</span><span class="sxs-lookup"><span data-stu-id="c2e35-148">Interactive Provider</span></span>](#InteractiveProvider) |


## <a name="a-nameauthcodeproviderauthorization-code-provider"></a><span data-ttu-id="c2e35-149"><a name="AuthCodeProvider"/>Provedor de código de autorização</span><span class="sxs-lookup"><span data-stu-id="c2e35-149"><a name="AuthCodeProvider"/>Authorization code provider</span></span>

<span data-ttu-id="c2e35-150">O fluxo de código de autorização permite que aplicativos nativos e Web obtenham tokens com segurança no nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="c2e35-150">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="c2e35-151">Para saber mais, confira [Microsoft Identity Platform and OAuth 2,0 Authorization Code Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span><span class="sxs-lookup"><span data-stu-id="c2e35-151">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="c2e35-152">C#</span><span class="sxs-lookup"><span data-stu-id="c2e35-152">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = AuthorizationCodeProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2e35-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2e35-153">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c2e35-154">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="c2e35-154">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="c2e35-155">Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="c2e35-155">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="c2e35-156">Java</span><span class="sxs-lookup"><span data-stu-id="c2e35-156">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="c2e35-157">Android</span><span class="sxs-lookup"><span data-stu-id="c2e35-157">Android</span></span>](#tab/Android)

<span data-ttu-id="c2e35-158">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-158">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2e35-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2e35-159">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c2e35-160">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-160">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="c2e35-161">PHP</span><span class="sxs-lookup"><span data-stu-id="c2e35-161">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c2e35-162">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-162">Not yet available.</span></span> <span data-ttu-id="c2e35-163">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-163">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="c2e35-164">Ruby</span><span class="sxs-lookup"><span data-stu-id="c2e35-164">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c2e35-165">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="c2e35-165">Not available, yet.</span></span> <span data-ttu-id="c2e35-166">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-166">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameclientcredentialsproviderclient-credentials-provider"></a><span data-ttu-id="c2e35-167"><a name="ClientCredentialsProvider"/>Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="c2e35-167"><a name="ClientCredentialsProvider"/>Client credentials provider</span></span>

<span data-ttu-id="c2e35-168">O fluxo de credenciais do cliente permite que aplicativos de serviço sejam executados sem interação do usuário.</span><span class="sxs-lookup"><span data-stu-id="c2e35-168">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="c2e35-169">O acesso baseia-se na identidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c2e35-169">Access is based on the identity of the application.</span></span> <span data-ttu-id="c2e35-170">Para obter mais informações, consulte [Microsoft Identity Platform e The OAuth 2,0 Client Credentials Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="c2e35-170">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="c2e35-171">C#</span><span class="sxs-lookup"><span data-stu-id="c2e35-171">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = ClientCredentialProvider.CreateClientApplication(clientId, clientCredential);
ClientCredentialProvider authProvider = new ClientCredentialProvider(clientApplication);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2e35-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2e35-172">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c2e35-173">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="c2e35-173">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="c2e35-174">Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="c2e35-174">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="c2e35-175">Java</span><span class="sxs-lookup"><span data-stu-id="c2e35-175">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="c2e35-176">Android</span><span class="sxs-lookup"><span data-stu-id="c2e35-176">Android</span></span>](#tab/Android)

<span data-ttu-id="c2e35-177">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-177">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2e35-178">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2e35-178">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c2e35-179">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-179">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="c2e35-180">PHP</span><span class="sxs-lookup"><span data-stu-id="c2e35-180">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c2e35-181">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="c2e35-181">Not available, yet.</span></span> <span data-ttu-id="c2e35-182">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-182">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="c2e35-183">Ruby</span><span class="sxs-lookup"><span data-stu-id="c2e35-183">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c2e35-184">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="c2e35-184">Not available, yet.</span></span> <span data-ttu-id="c2e35-185">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-185">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameonbehalfofprovideron-behalf-of-provider"></a><span data-ttu-id="c2e35-186"><a name="OnBehalfOfProvider"/>Provedor em nome de</span><span class="sxs-lookup"><span data-stu-id="c2e35-186"><a name="OnBehalfOfProvider"/>On-behalf-of provider</span></span>

<span data-ttu-id="c2e35-187">O fluxo em nome de é aplicável quando o aplicativo chama uma API de serviço/Web que, em seguida, chama a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c2e35-187">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="c2e35-188">Saiba mais lendo a [plataforma de identidade da Microsoft e o fluxo em nome de do OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="c2e35-188">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="c2e35-189">C#</span><span class="sxs-lookup"><span data-stu-id="c2e35-189">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = OnBehalfOfProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
OnBehalfOfProvider authProvider = new OnBehalfOfProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2e35-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2e35-190">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c2e35-191">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="c2e35-191">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="c2e35-192">Leia [usando provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="c2e35-192">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="c2e35-193">Java</span><span class="sxs-lookup"><span data-stu-id="c2e35-193">Java</span></span>](#tab/Java)

<span data-ttu-id="c2e35-194">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-194">Not yet available.</span></span> <span data-ttu-id="c2e35-195">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-195">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="c2e35-196">Android</span><span class="sxs-lookup"><span data-stu-id="c2e35-196">Android</span></span>](#tab/Android)

<span data-ttu-id="c2e35-197">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-197">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2e35-198">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2e35-198">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c2e35-199">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-199">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="c2e35-200">PHP</span><span class="sxs-lookup"><span data-stu-id="c2e35-200">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c2e35-201">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-201">Not yet available.</span></span> <span data-ttu-id="c2e35-202">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-202">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="c2e35-203">Ruby</span><span class="sxs-lookup"><span data-stu-id="c2e35-203">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c2e35-204">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-204">Not yet available.</span></span> <span data-ttu-id="c2e35-205">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-205">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="a-nameimplicitproviderimplicit-provider"></a><span data-ttu-id="c2e35-206"><a name="ImplicitProvider"/>Provedor implícito</span><span class="sxs-lookup"><span data-stu-id="c2e35-206"><a name="ImplicitProvider"/>Implicit provider</span></span>

<span data-ttu-id="c2e35-207">O fluxo de concessão implícito é usado em aplicativos baseados em navegador.</span><span class="sxs-lookup"><span data-stu-id="c2e35-207">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="c2e35-208">Para obter mais informações, consulte [Microsoft Identity Platform and implícito Grant Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="c2e35-208">For more information, see [Microsoft identity platform and Implicit grant flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="c2e35-209">C#</span><span class="sxs-lookup"><span data-stu-id="c2e35-209">C#</span></span>](#tab/CS)

<span data-ttu-id="c2e35-210">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-210">Not applicable.</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2e35-211">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2e35-211">Javascript</span></span>](#tab/Javascript)

```javascript
const clientId = "your_client_id"; // Client Id of the registered application
const callback = (errorDesc, token, error, tokenType) => {};
// An Optional options for initializing the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#configuration-options
const options = {
    redirectUri: "Your redirect URI",
};
const graphScopes = ["user.read", "mail.send"]; // An array of graph scopes

// Initialize the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#initialization-of-msal
const userAgentApplication = new Msal.UserAgentApplication(clientId, undefined, callback, options);
const authProvider = new MicrosoftGraph.MSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

# <a name="javatabjava"></a>[<span data-ttu-id="c2e35-212">Java</span><span class="sxs-lookup"><span data-stu-id="c2e35-212">Java</span></span>](#tab/Java)

<span data-ttu-id="c2e35-213">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-213">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="c2e35-214">Android</span><span class="sxs-lookup"><span data-stu-id="c2e35-214">Android</span></span>](#tab/Android)

<span data-ttu-id="c2e35-215">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-215">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2e35-216">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2e35-216">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c2e35-217">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-217">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="c2e35-218">PHP</span><span class="sxs-lookup"><span data-stu-id="c2e35-218">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c2e35-219">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-219">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="c2e35-220">Ruby</span><span class="sxs-lookup"><span data-stu-id="c2e35-220">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c2e35-221">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-221">Not applicable.</span></span>

---

##  <a name="a-namedevicecodeproviderdevice-code-provider"></a><span data-ttu-id="c2e35-222"><a name="DeviceCodeProvider"/>Provedor de código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c2e35-222"><a name="DeviceCodeProvider"/>Device code provider</span></span>

<span data-ttu-id="c2e35-223">O fluxo de código de dispositivo permite entrar em dispositivos por meio de outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c2e35-223">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="c2e35-224">Para obter detalhes, consulte [plataforma de identidade da Microsoft e o fluxo de código de dispositivo OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span><span class="sxs-lookup"><span data-stu-id="c2e35-224">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="c2e35-225">C#</span><span class="sxs-lookup"><span data-stu-id="c2e35-225">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = DeviceCodeProvider.CreateClientApplication(clientId);
DeviceCodeProvider authProvider = new DeviceCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2e35-226">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2e35-226">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c2e35-227">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-227">Not yet available.</span></span> <span data-ttu-id="c2e35-228">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-228">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="c2e35-229">Java</span><span class="sxs-lookup"><span data-stu-id="c2e35-229">Java</span></span>](#tab/Java)

<span data-ttu-id="c2e35-230">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="c2e35-230">Not available, yet.</span></span> <span data-ttu-id="c2e35-231">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-231">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="c2e35-232">Android</span><span class="sxs-lookup"><span data-stu-id="c2e35-232">Android</span></span>](#tab/Android)

<span data-ttu-id="c2e35-233">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-233">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2e35-234">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2e35-234">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c2e35-235">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-235">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="c2e35-236">PHP</span><span class="sxs-lookup"><span data-stu-id="c2e35-236">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c2e35-237">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-237">Not yet available.</span></span> <span data-ttu-id="c2e35-238">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-238">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="c2e35-239">Ruby</span><span class="sxs-lookup"><span data-stu-id="c2e35-239">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c2e35-240">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-240">Not yet available.</span></span> <span data-ttu-id="c2e35-241">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameintegratedwindowsproviderintegrated-windows-provider"></a><span data-ttu-id="c2e35-242"><a name="IntegratedWindowsProvider"/>Provedor integrado do Windows</span><span class="sxs-lookup"><span data-stu-id="c2e35-242"><a name="IntegratedWindowsProvider"/>Integrated Windows provider</span></span>

<span data-ttu-id="c2e35-243">O fluxo integrado do Windows oferece uma maneira para que os computadores com Windows adquiram um token de acesso de forma silenciosa quando são associados ao domínio.</span><span class="sxs-lookup"><span data-stu-id="c2e35-243">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="c2e35-244">Para obter detalhes, consulte [autenticação integrada do Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span><span class="sxs-lookup"><span data-stu-id="c2e35-244">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="c2e35-245">C#</span><span class="sxs-lookup"><span data-stu-id="c2e35-245">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = IntegratedWindowsAuthenticationProvider.CreateClientApplication(clientId);
IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2e35-246">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2e35-246">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c2e35-247">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-247">Not applicable.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="c2e35-248">Java</span><span class="sxs-lookup"><span data-stu-id="c2e35-248">Java</span></span>](#tab/Java)

<span data-ttu-id="c2e35-249">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-249">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="c2e35-250">Android</span><span class="sxs-lookup"><span data-stu-id="c2e35-250">Android</span></span>](#tab/Android)

<span data-ttu-id="c2e35-251">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-251">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2e35-252">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2e35-252">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c2e35-253">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-253">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="c2e35-254">PHP</span><span class="sxs-lookup"><span data-stu-id="c2e35-254">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c2e35-255">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-255">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="c2e35-256">Ruby</span><span class="sxs-lookup"><span data-stu-id="c2e35-256">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c2e35-257">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-257">Not applicable.</span></span>

---

##  <a name="a-nameinteractiveproviderinteractive-provider"></a><span data-ttu-id="c2e35-258"><a name="InteractiveProvider"/>Provedor interativo</span><span class="sxs-lookup"><span data-stu-id="c2e35-258"><a name="InteractiveProvider"/>Interactive provider</span></span>

<span data-ttu-id="c2e35-259">O fluxo interativo é usado por aplicativos móveis (Xamarin e UWP) e aplicativos de área de trabalho para chamar o Microsoft Graph no nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c2e35-259">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="c2e35-260">Para obter detalhes, [](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)consulte adquirindo tokens interativamente.</span><span class="sxs-lookup"><span data-stu-id="c2e35-260">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="c2e35-261">C#</span><span class="sxs-lookup"><span data-stu-id="c2e35-261">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = InteractiveAuthenticationProvider.CreateClientApplication(clientId);
InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2e35-262">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2e35-262">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c2e35-263">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-263">Not yet available.</span></span> <span data-ttu-id="c2e35-264">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-264">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="c2e35-265">Java</span><span class="sxs-lookup"><span data-stu-id="c2e35-265">Java</span></span>](#tab/Java)

<span data-ttu-id="c2e35-266">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-266">Not yet available.</span></span> <span data-ttu-id="c2e35-267">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-267">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="c2e35-268">Android</span><span class="sxs-lookup"><span data-stu-id="c2e35-268">Android</span></span>](#tab/Android)

```java
PublicClientApplication publicClientApplication = new PublicClientApplication(getApplicationContext(), "CLIENT_ID_OF_YOUR_APPLICATION");
MSALAuthenticationProvider msalAuthenticationProvider = new MSALAuthenticationProvider(
    getActivity(),
    getApplication(),
    publicClientApplication,
    scopes);

IGraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(msalAuthenticationProvider)
    .buildClient();
```

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2e35-269">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2e35-269">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[<span data-ttu-id="c2e35-270">PHP</span><span class="sxs-lookup"><span data-stu-id="c2e35-270">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c2e35-271">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-271">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="c2e35-272">Ruby</span><span class="sxs-lookup"><span data-stu-id="c2e35-272">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c2e35-273">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-273">Not applicable.</span></span>

---

##  <a name="a-nameusernamepasswordproviderusernamepassword-provider"></a><span data-ttu-id="c2e35-274"><a name="UsernamePasswordProvider"/>Provedor de nome de usuário/senha</span><span class="sxs-lookup"><span data-stu-id="c2e35-274"><a name="UsernamePasswordProvider"/>Username/password provider</span></span>

<span data-ttu-id="c2e35-275">O provedor de nome de usuário/senha permite que um aplicativo entre em um usuário usando seu nome de usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="c2e35-275">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="c2e35-276">Use este fluxo somente quando não for possível usar qualquer um dos outros fluxos OAuth.</span><span class="sxs-lookup"><span data-stu-id="c2e35-276">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="c2e35-277">Para obter mais informações, consulte [plataforma de identidade da Microsoft e a credencial de senha de proprietário do recurso OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="c2e35-277">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="ctabcs"></a>[<span data-ttu-id="c2e35-278">C#</span><span class="sxs-lookup"><span data-stu-id="c2e35-278">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = UsernamePasswordProvider.CreateClientApplication(clientId);
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2e35-279">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2e35-279">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="c2e35-280">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-280">Not yet available.</span></span> <span data-ttu-id="c2e35-281">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-281">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="c2e35-282">Java</span><span class="sxs-lookup"><span data-stu-id="c2e35-282">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="c2e35-283">Android</span><span class="sxs-lookup"><span data-stu-id="c2e35-283">Android</span></span>](#tab/Android)

<span data-ttu-id="c2e35-284">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-284">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2e35-285">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2e35-285">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c2e35-286">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c2e35-286">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="c2e35-287">PHP</span><span class="sxs-lookup"><span data-stu-id="c2e35-287">PHP</span></span>](#tab/PHP)

<span data-ttu-id="c2e35-288">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-288">Not yet available.</span></span> <span data-ttu-id="c2e35-289">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="c2e35-290">Ruby</span><span class="sxs-lookup"><span data-stu-id="c2e35-290">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="c2e35-291">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="c2e35-291">Not yet available.</span></span> <span data-ttu-id="c2e35-292">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="c2e35-292">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="c2e35-293">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="c2e35-293">Next steps</span></span>

* <span data-ttu-id="c2e35-294">Os provedores de autenticação exigem uma ID de cliente.</span><span class="sxs-lookup"><span data-stu-id="c2e35-294">Authentication providers require an client ID.</span></span> <span data-ttu-id="c2e35-295">Você deve [registrar seu aplicativo](https://portal.azure.com/) depois de configurar seu provedor de autenticação.</span><span class="sxs-lookup"><span data-stu-id="c2e35-295">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="c2e35-296">Deixe-nos saber se um fluxo OAuth necessário atualmente não é suportado pela votação ou pela abertura de uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span><span class="sxs-lookup"><span data-stu-id="c2e35-296">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
