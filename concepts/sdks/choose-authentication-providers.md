---
title: Escolher um provedor de autenticação do Microsoft Graph
description: Saiba como escolher provedores de autenticação específicos do cenário para seu aplicativo.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 7975a2049ee16d89cfc9668babde091db7dd140e
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778296"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="de6bf-103">Escolher um provedor de autenticação do Microsoft Graph com base no cenário</span><span class="sxs-lookup"><span data-stu-id="de6bf-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="de6bf-104">Os provedores de autenticação implementam o código necessário para adquirir um token usando a biblioteca de autenticação da Microsoft (MSAL); gerenciar vários erros potenciais para casos como o consentimento incremental, senhas expiradas e acesso condicional; e, em seguida, defina o cabeçalho de autorização da solicitação HTTP.</span><span class="sxs-lookup"><span data-stu-id="de6bf-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="de6bf-105">A tabela a seguir lista o conjunto de provedores que correspondem aos cenários para diferentes [tipos de aplicativos](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types).</span><span class="sxs-lookup"><span data-stu-id="de6bf-105">The following table lists the set of providers that match the scenarios for different [application types](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="de6bf-106">Cenário</span><span class="sxs-lookup"><span data-stu-id="de6bf-106">Scenario</span></span> | <span data-ttu-id="de6bf-107">Fluxo/concessão</span><span class="sxs-lookup"><span data-stu-id="de6bf-107">Flow/Grant</span></span> | <span data-ttu-id="de6bf-108">Público-alvo</span><span class="sxs-lookup"><span data-stu-id="de6bf-108">Audience</span></span> | <span data-ttu-id="de6bf-109">Provedor</span><span class="sxs-lookup"><span data-stu-id="de6bf-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="de6bf-110">Aplicativo de página única</span><span class="sxs-lookup"><span data-stu-id="de6bf-110">Single Page App</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="de6bf-111">Implícito</span><span class="sxs-lookup"><span data-stu-id="de6bf-111">Implicit</span></span> | <span data-ttu-id="de6bf-112">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="de6bf-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="de6bf-113">Provedor implícito</span><span class="sxs-lookup"><span data-stu-id="de6bf-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="de6bf-114">Aplicativo Web que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="de6bf-114">Web App that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="de6bf-115">Código de Autorização</span><span class="sxs-lookup"><span data-stu-id="de6bf-115">Authorization Code</span></span> | <span data-ttu-id="de6bf-116">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="de6bf-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="de6bf-117">Provedor de código de autorização</span><span class="sxs-lookup"><span data-stu-id="de6bf-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="de6bf-118">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="de6bf-118">Client Credentials</span></span>  | <span data-ttu-id="de6bf-119">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="de6bf-119">App Only</span></span> | [<span data-ttu-id="de6bf-120">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="de6bf-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="de6bf-121">API Web que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="de6bf-121">Web API that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="de6bf-122">Em nome de</span><span class="sxs-lookup"><span data-stu-id="de6bf-122">On Behalf Of</span></span> | <span data-ttu-id="de6bf-123">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="de6bf-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="de6bf-124">Em nome do provedor</span><span class="sxs-lookup"><span data-stu-id="de6bf-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="de6bf-125">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="de6bf-125">Client Credentials</span></span>  | <span data-ttu-id="de6bf-126">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="de6bf-126">App Only</span></span> | [<span data-ttu-id="de6bf-127">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="de6bf-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="de6bf-128">Aplicativo de área de trabalho que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="de6bf-128">Desktop app that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="de6bf-129">Interativo</span><span class="sxs-lookup"><span data-stu-id="de6bf-129">Interactive</span></span> | <span data-ttu-id="de6bf-130">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="de6bf-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="de6bf-131">Provedor interativo</span><span class="sxs-lookup"><span data-stu-id="de6bf-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="de6bf-132">Integrada do Windows</span><span class="sxs-lookup"><span data-stu-id="de6bf-132">Integrated Windows</span></span> | <span data-ttu-id="de6bf-133">Organização delegada</span><span class="sxs-lookup"><span data-stu-id="de6bf-133">Delegated Org</span></span> | [<span data-ttu-id="de6bf-134">Provedor integrado do Windows</span><span class="sxs-lookup"><span data-stu-id="de6bf-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="de6bf-135">Proprietário do recurso</span><span class="sxs-lookup"><span data-stu-id="de6bf-135">Resource Owner</span></span>  | <span data-ttu-id="de6bf-136">Organização delegada</span><span class="sxs-lookup"><span data-stu-id="de6bf-136">Delegated Org</span></span> | [<span data-ttu-id="de6bf-137">Provedor de nome de usuário/senha</span><span class="sxs-lookup"><span data-stu-id="de6bf-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="de6bf-138">Código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="de6bf-138">Device Code</span></span>  | <span data-ttu-id="de6bf-139">Organização delegada</span><span class="sxs-lookup"><span data-stu-id="de6bf-139">Delegated Org</span></span> | [<span data-ttu-id="de6bf-140">Provedor de código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="de6bf-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="de6bf-141">Aplicativo daemon</span><span class="sxs-lookup"><span data-stu-id="de6bf-141">Daemon app</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="de6bf-142">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="de6bf-142">Client Credentials</span></span>  | <span data-ttu-id="de6bf-143">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="de6bf-143">App Only</span></span> | [<span data-ttu-id="de6bf-144">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="de6bf-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="de6bf-145">Aplicativo móvel que chama as APIs Web</span><span class="sxs-lookup"><span data-stu-id="de6bf-145">Mobile app that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="de6bf-146">Interativo</span><span class="sxs-lookup"><span data-stu-id="de6bf-146">Interactive</span></span> | <span data-ttu-id="de6bf-147">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="de6bf-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="de6bf-148">Provedor interativo</span><span class="sxs-lookup"><span data-stu-id="de6bf-148">Interactive Provider</span></span>](#InteractiveProvider) |


## <a name="a-nameauthcodeproviderauthorization-code-provider"></a><span data-ttu-id="de6bf-149"><a name="AuthCodeProvider"/>Provedor de código de autorização</span><span class="sxs-lookup"><span data-stu-id="de6bf-149"><a name="AuthCodeProvider"/>Authorization code provider</span></span>

<span data-ttu-id="de6bf-150">O fluxo de código de autorização permite que aplicativos nativos e Web obtenham tokens com segurança no nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="de6bf-150">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="de6bf-151">Para saber mais, confira [Microsoft Identity Platform and OAuth 2,0 Authorization Code Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span><span class="sxs-lookup"><span data-stu-id="de6bf-151">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="de6bf-152">C#</span><span class="sxs-lookup"><span data-stu-id="de6bf-152">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);  
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6bf-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="de6bf-153">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="de6bf-154">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="de6bf-154">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="de6bf-155">Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="de6bf-155">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="de6bf-156">Java</span><span class="sxs-lookup"><span data-stu-id="de6bf-156">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="de6bf-157">Android</span><span class="sxs-lookup"><span data-stu-id="de6bf-157">Android</span></span>](#tab/Android)

<span data-ttu-id="de6bf-158">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-158">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de6bf-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de6bf-159">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="de6bf-160">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-160">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="de6bf-161">PHP</span><span class="sxs-lookup"><span data-stu-id="de6bf-161">PHP</span></span>](#tab/PHP)

<span data-ttu-id="de6bf-162">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-162">Not yet available.</span></span> <span data-ttu-id="de6bf-163">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-163">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="de6bf-164">Ruby</span><span class="sxs-lookup"><span data-stu-id="de6bf-164">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="de6bf-165">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="de6bf-165">Not available, yet.</span></span> <span data-ttu-id="de6bf-166">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-166">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameclientcredentialsproviderclient-credentials-provider"></a><span data-ttu-id="de6bf-167"><a name="ClientCredentialsProvider"/>Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="de6bf-167"><a name="ClientCredentialsProvider"/>Client credentials provider</span></span>

<span data-ttu-id="de6bf-168">O fluxo de credenciais do cliente permite que aplicativos de serviço sejam executados sem interação do usuário.</span><span class="sxs-lookup"><span data-stu-id="de6bf-168">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="de6bf-169">O acesso baseia-se na identidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de6bf-169">Access is based on the identity of the application.</span></span> <span data-ttu-id="de6bf-170">Para obter mais informações, consulte [Microsoft Identity Platform e The OAuth 2,0 Client Credentials Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="de6bf-170">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="de6bf-171">C#</span><span class="sxs-lookup"><span data-stu-id="de6bf-171">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6bf-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="de6bf-172">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="de6bf-173">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="de6bf-173">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="de6bf-174">Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="de6bf-174">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="de6bf-175">Java</span><span class="sxs-lookup"><span data-stu-id="de6bf-175">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="de6bf-176">Android</span><span class="sxs-lookup"><span data-stu-id="de6bf-176">Android</span></span>](#tab/Android)

<span data-ttu-id="de6bf-177">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-177">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de6bf-178">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de6bf-178">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="de6bf-179">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-179">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="de6bf-180">PHP</span><span class="sxs-lookup"><span data-stu-id="de6bf-180">PHP</span></span>](#tab/PHP)

<span data-ttu-id="de6bf-181">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="de6bf-181">Not available, yet.</span></span> <span data-ttu-id="de6bf-182">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-182">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="de6bf-183">Ruby</span><span class="sxs-lookup"><span data-stu-id="de6bf-183">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="de6bf-184">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="de6bf-184">Not available, yet.</span></span> <span data-ttu-id="de6bf-185">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-185">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameonbehalfofprovideron-behalf-of-provider"></a><span data-ttu-id="de6bf-186"><a name="OnBehalfOfProvider"/>Provedor em nome de</span><span class="sxs-lookup"><span data-stu-id="de6bf-186"><a name="OnBehalfOfProvider"/>On-behalf-of provider</span></span>

<span data-ttu-id="de6bf-187">O fluxo em nome de é aplicável quando o aplicativo chama uma API de serviço/Web que, em seguida, chama a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="de6bf-187">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="de6bf-188">Saiba mais lendo a [plataforma de identidade da Microsoft e o fluxo em nome de do OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="de6bf-188">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="de6bf-189">C#</span><span class="sxs-lookup"><span data-stu-id="de6bf-189">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6bf-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="de6bf-190">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="de6bf-191">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="de6bf-191">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="de6bf-192">Leia [usando provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="de6bf-192">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="de6bf-193">Java</span><span class="sxs-lookup"><span data-stu-id="de6bf-193">Java</span></span>](#tab/Java)

<span data-ttu-id="de6bf-194">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-194">Not yet available.</span></span> <span data-ttu-id="de6bf-195">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-195">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="de6bf-196">Android</span><span class="sxs-lookup"><span data-stu-id="de6bf-196">Android</span></span>](#tab/Android)

<span data-ttu-id="de6bf-197">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-197">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de6bf-198">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de6bf-198">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="de6bf-199">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-199">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="de6bf-200">PHP</span><span class="sxs-lookup"><span data-stu-id="de6bf-200">PHP</span></span>](#tab/PHP)

<span data-ttu-id="de6bf-201">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-201">Not yet available.</span></span> <span data-ttu-id="de6bf-202">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-202">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="de6bf-203">Ruby</span><span class="sxs-lookup"><span data-stu-id="de6bf-203">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="de6bf-204">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-204">Not yet available.</span></span> <span data-ttu-id="de6bf-205">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-205">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="a-nameimplicitproviderimplicit-provider"></a><span data-ttu-id="de6bf-206"><a name="ImplicitProvider"/>Provedor implícito</span><span class="sxs-lookup"><span data-stu-id="de6bf-206"><a name="ImplicitProvider"/>Implicit provider</span></span>

<span data-ttu-id="de6bf-207">O fluxo de concessão implícito é usado em aplicativos baseados em navegador.</span><span class="sxs-lookup"><span data-stu-id="de6bf-207">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="de6bf-208">Para obter mais informações, consulte [Microsoft Identity Platform and implícito Grant Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="de6bf-208">For more information, see [Microsoft identity platform and Implicit grant flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="de6bf-209">C#</span><span class="sxs-lookup"><span data-stu-id="de6bf-209">C#</span></span>](#tab/CS)

<span data-ttu-id="de6bf-210">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-210">Not applicable.</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6bf-211">Javascript</span><span class="sxs-lookup"><span data-stu-id="de6bf-211">Javascript</span></span>](#tab/Javascript)

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

# <a name="javatabjava"></a>[<span data-ttu-id="de6bf-212">Java</span><span class="sxs-lookup"><span data-stu-id="de6bf-212">Java</span></span>](#tab/Java)

<span data-ttu-id="de6bf-213">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-213">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="de6bf-214">Android</span><span class="sxs-lookup"><span data-stu-id="de6bf-214">Android</span></span>](#tab/Android)

<span data-ttu-id="de6bf-215">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-215">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de6bf-216">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de6bf-216">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="de6bf-217">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-217">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="de6bf-218">PHP</span><span class="sxs-lookup"><span data-stu-id="de6bf-218">PHP</span></span>](#tab/PHP)

<span data-ttu-id="de6bf-219">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-219">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="de6bf-220">Ruby</span><span class="sxs-lookup"><span data-stu-id="de6bf-220">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="de6bf-221">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-221">Not applicable.</span></span>

---

##  <a name="a-namedevicecodeproviderdevice-code-provider"></a><span data-ttu-id="de6bf-222"><a name="DeviceCodeProvider"/>Provedor de código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="de6bf-222"><a name="DeviceCodeProvider"/>Device code provider</span></span>

<span data-ttu-id="de6bf-223">O fluxo de código de dispositivo permite entrar em dispositivos por meio de outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de6bf-223">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="de6bf-224">Para obter detalhes, consulte [plataforma de identidade da Microsoft e o fluxo de código de dispositivo OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span><span class="sxs-lookup"><span data-stu-id="de6bf-224">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="de6bf-225">C#</span><span class="sxs-lookup"><span data-stu-id="de6bf-225">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6bf-226">Javascript</span><span class="sxs-lookup"><span data-stu-id="de6bf-226">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="de6bf-227">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-227">Not yet available.</span></span> <span data-ttu-id="de6bf-228">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-228">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="de6bf-229">Java</span><span class="sxs-lookup"><span data-stu-id="de6bf-229">Java</span></span>](#tab/Java)

<span data-ttu-id="de6bf-230">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="de6bf-230">Not available, yet.</span></span> <span data-ttu-id="de6bf-231">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-231">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="de6bf-232">Android</span><span class="sxs-lookup"><span data-stu-id="de6bf-232">Android</span></span>](#tab/Android)

<span data-ttu-id="de6bf-233">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-233">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de6bf-234">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de6bf-234">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="de6bf-235">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-235">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="de6bf-236">PHP</span><span class="sxs-lookup"><span data-stu-id="de6bf-236">PHP</span></span>](#tab/PHP)

<span data-ttu-id="de6bf-237">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-237">Not yet available.</span></span> <span data-ttu-id="de6bf-238">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-238">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="de6bf-239">Ruby</span><span class="sxs-lookup"><span data-stu-id="de6bf-239">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="de6bf-240">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-240">Not yet available.</span></span> <span data-ttu-id="de6bf-241">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameintegratedwindowsproviderintegrated-windows-provider"></a><span data-ttu-id="de6bf-242"><a name="IntegratedWindowsProvider"/>Provedor integrado do Windows</span><span class="sxs-lookup"><span data-stu-id="de6bf-242"><a name="IntegratedWindowsProvider"/>Integrated Windows provider</span></span>

<span data-ttu-id="de6bf-243">O fluxo integrado do Windows oferece uma maneira para que os computadores com Windows adquiram um token de acesso de forma silenciosa quando são associados ao domínio.</span><span class="sxs-lookup"><span data-stu-id="de6bf-243">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="de6bf-244">Para obter detalhes, consulte [autenticação integrada do Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span><span class="sxs-lookup"><span data-stu-id="de6bf-244">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="de6bf-245">C#</span><span class="sxs-lookup"><span data-stu-id="de6bf-245">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6bf-246">Javascript</span><span class="sxs-lookup"><span data-stu-id="de6bf-246">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="de6bf-247">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-247">Not applicable.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="de6bf-248">Java</span><span class="sxs-lookup"><span data-stu-id="de6bf-248">Java</span></span>](#tab/Java)

<span data-ttu-id="de6bf-249">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-249">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="de6bf-250">Android</span><span class="sxs-lookup"><span data-stu-id="de6bf-250">Android</span></span>](#tab/Android)

<span data-ttu-id="de6bf-251">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-251">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de6bf-252">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de6bf-252">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="de6bf-253">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-253">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="de6bf-254">PHP</span><span class="sxs-lookup"><span data-stu-id="de6bf-254">PHP</span></span>](#tab/PHP)

<span data-ttu-id="de6bf-255">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-255">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="de6bf-256">Ruby</span><span class="sxs-lookup"><span data-stu-id="de6bf-256">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="de6bf-257">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-257">Not applicable.</span></span>

---

##  <a name="a-nameinteractiveproviderinteractive-provider"></a><span data-ttu-id="de6bf-258"><a name="InteractiveProvider"/>Provedor interativo</span><span class="sxs-lookup"><span data-stu-id="de6bf-258"><a name="InteractiveProvider"/>Interactive provider</span></span>

<span data-ttu-id="de6bf-259">O fluxo interativo é usado por aplicativos móveis (Xamarin e UWP) e aplicativos de área de trabalho para chamar o Microsoft Graph no nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="de6bf-259">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="de6bf-260">Para obter detalhes, [](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)consulte adquirindo tokens interativamente.</span><span class="sxs-lookup"><span data-stu-id="de6bf-260">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="de6bf-261">C#</span><span class="sxs-lookup"><span data-stu-id="de6bf-261">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6bf-262">Javascript</span><span class="sxs-lookup"><span data-stu-id="de6bf-262">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="de6bf-263">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-263">Not yet available.</span></span> <span data-ttu-id="de6bf-264">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-264">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="de6bf-265">Java</span><span class="sxs-lookup"><span data-stu-id="de6bf-265">Java</span></span>](#tab/Java)

<span data-ttu-id="de6bf-266">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-266">Not yet available.</span></span> <span data-ttu-id="de6bf-267">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-267">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="de6bf-268">Android</span><span class="sxs-lookup"><span data-stu-id="de6bf-268">Android</span></span>](#tab/Android)

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

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de6bf-269">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de6bf-269">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[<span data-ttu-id="de6bf-270">PHP</span><span class="sxs-lookup"><span data-stu-id="de6bf-270">PHP</span></span>](#tab/PHP)

<span data-ttu-id="de6bf-271">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-271">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="de6bf-272">Ruby</span><span class="sxs-lookup"><span data-stu-id="de6bf-272">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="de6bf-273">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-273">Not applicable.</span></span>

---

##  <a name="a-nameusernamepasswordproviderusernamepassword-provider"></a><span data-ttu-id="de6bf-274"><a name="UsernamePasswordProvider"/>Provedor de nome de usuário/senha</span><span class="sxs-lookup"><span data-stu-id="de6bf-274"><a name="UsernamePasswordProvider"/>Username/password provider</span></span>

<span data-ttu-id="de6bf-275">O provedor de nome de usuário/senha permite que um aplicativo entre em um usuário usando seu nome de usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="de6bf-275">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="de6bf-276">Use este fluxo somente quando não for possível usar qualquer um dos outros fluxos OAuth.</span><span class="sxs-lookup"><span data-stu-id="de6bf-276">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="de6bf-277">Para obter mais informações, consulte [plataforma de identidade da Microsoft e a credencial de senha de proprietário do recurso OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="de6bf-277">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="ctabcs"></a>[<span data-ttu-id="de6bf-278">C#</span><span class="sxs-lookup"><span data-stu-id="de6bf-278">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

UsernamePasswordProvider authProvider = new UsernamePasswordProvider(publicClientApplication, scopes);

GraphServiceClient graphClient = new GraphServiceClient(authProvider);

User me = await graphClient.Me.Request()
                .WithUsernamePassword(email, password)
                .GetAsync();
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6bf-279">Javascript</span><span class="sxs-lookup"><span data-stu-id="de6bf-279">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="de6bf-280">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-280">Not yet available.</span></span> <span data-ttu-id="de6bf-281">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-281">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="de6bf-282">Java</span><span class="sxs-lookup"><span data-stu-id="de6bf-282">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="de6bf-283">Android</span><span class="sxs-lookup"><span data-stu-id="de6bf-283">Android</span></span>](#tab/Android)

<span data-ttu-id="de6bf-284">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-284">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de6bf-285">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de6bf-285">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="de6bf-286">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="de6bf-286">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="de6bf-287">PHP</span><span class="sxs-lookup"><span data-stu-id="de6bf-287">PHP</span></span>](#tab/PHP)

<span data-ttu-id="de6bf-288">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-288">Not yet available.</span></span> <span data-ttu-id="de6bf-289">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="de6bf-290">Ruby</span><span class="sxs-lookup"><span data-stu-id="de6bf-290">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="de6bf-291">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="de6bf-291">Not yet available.</span></span> <span data-ttu-id="de6bf-292">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="de6bf-292">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="de6bf-293">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="de6bf-293">Next steps</span></span>

* <span data-ttu-id="de6bf-294">Os provedores de autenticação exigem uma ID de cliente.</span><span class="sxs-lookup"><span data-stu-id="de6bf-294">Authentication providers require an client ID.</span></span> <span data-ttu-id="de6bf-295">Você deve [registrar seu aplicativo](https://portal.azure.com/) depois de configurar seu provedor de autenticação.</span><span class="sxs-lookup"><span data-stu-id="de6bf-295">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="de6bf-296">Deixe-nos saber se um fluxo OAuth necessário atualmente não é suportado pela votação ou pela abertura de uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span><span class="sxs-lookup"><span data-stu-id="de6bf-296">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
