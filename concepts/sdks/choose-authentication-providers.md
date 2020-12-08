---
title: Escolher um provedor de autenticação do Microsoft Graph
description: Saiba como escolher provedores de autenticação específicos do cenário para seu aplicativo.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 29f7ea60080ed1f1a2ed6ea02256e03f5b91e6cd
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49580967"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="e6468-103">Escolher um provedor de autenticação do Microsoft Graph com base no cenário</span><span class="sxs-lookup"><span data-stu-id="e6468-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="e6468-104">Os provedores de autenticação implementam o código necessário para adquirir um token usando a biblioteca de autenticação da Microsoft (MSAL); gerenciar vários erros potenciais para casos como o consentimento incremental, senhas expiradas e acesso condicional; e, em seguida, defina o cabeçalho de autorização da solicitação HTTP.</span><span class="sxs-lookup"><span data-stu-id="e6468-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="e6468-105">A tabela a seguir lista o conjunto de provedores que correspondem aos cenários para diferentes [tipos de aplicativos](/azure/active-directory/develop/v2-app-types).</span><span class="sxs-lookup"><span data-stu-id="e6468-105">The following table lists the set of providers that match the scenarios for different [application types](/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="e6468-106">Cenário</span><span class="sxs-lookup"><span data-stu-id="e6468-106">Scenario</span></span> | <span data-ttu-id="e6468-107">Fluxo/concessão</span><span class="sxs-lookup"><span data-stu-id="e6468-107">Flow/Grant</span></span> | <span data-ttu-id="e6468-108">Espectadores</span><span class="sxs-lookup"><span data-stu-id="e6468-108">Audience</span></span> | <span data-ttu-id="e6468-109">Provedor</span><span class="sxs-lookup"><span data-stu-id="e6468-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="e6468-110">Aplicativo de página única</span><span class="sxs-lookup"><span data-stu-id="e6468-110">Single Page App</span></span>](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="e6468-111">Implícito</span><span class="sxs-lookup"><span data-stu-id="e6468-111">Implicit</span></span> | <span data-ttu-id="e6468-112">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="e6468-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="e6468-113">Provedor implícito</span><span class="sxs-lookup"><span data-stu-id="e6468-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="e6468-114">Aplicativo Web que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="e6468-114">Web App that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="e6468-115">Código de Autorização</span><span class="sxs-lookup"><span data-stu-id="e6468-115">Authorization Code</span></span> | <span data-ttu-id="e6468-116">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="e6468-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="e6468-117">Provedor de código de autorização</span><span class="sxs-lookup"><span data-stu-id="e6468-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="e6468-118">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="e6468-118">Client Credentials</span></span>  | <span data-ttu-id="e6468-119">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6468-119">App Only</span></span> | [<span data-ttu-id="e6468-120">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="e6468-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="e6468-121">API Web que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="e6468-121">Web API that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="e6468-122">Em nome de</span><span class="sxs-lookup"><span data-stu-id="e6468-122">On Behalf Of</span></span> | <span data-ttu-id="e6468-123">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="e6468-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="e6468-124">Em nome do provedor</span><span class="sxs-lookup"><span data-stu-id="e6468-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="e6468-125">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="e6468-125">Client Credentials</span></span>  | <span data-ttu-id="e6468-126">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6468-126">App Only</span></span> | [<span data-ttu-id="e6468-127">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="e6468-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="e6468-128">Aplicativo de área de trabalho que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="e6468-128">Desktop app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="e6468-129">Interativo</span><span class="sxs-lookup"><span data-stu-id="e6468-129">Interactive</span></span> | <span data-ttu-id="e6468-130">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="e6468-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="e6468-131">Provedor interativo</span><span class="sxs-lookup"><span data-stu-id="e6468-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="e6468-132">Integrada do Windows</span><span class="sxs-lookup"><span data-stu-id="e6468-132">Integrated Windows</span></span> | <span data-ttu-id="e6468-133">Organização delegada</span><span class="sxs-lookup"><span data-stu-id="e6468-133">Delegated Org</span></span> | [<span data-ttu-id="e6468-134">Provedor integrado do Windows</span><span class="sxs-lookup"><span data-stu-id="e6468-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="e6468-135">Proprietário do recurso</span><span class="sxs-lookup"><span data-stu-id="e6468-135">Resource Owner</span></span>  | <span data-ttu-id="e6468-136">Organização delegada</span><span class="sxs-lookup"><span data-stu-id="e6468-136">Delegated Org</span></span> | [<span data-ttu-id="e6468-137">Provedor de nome de usuário/senha</span><span class="sxs-lookup"><span data-stu-id="e6468-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="e6468-138">Código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="e6468-138">Device Code</span></span>  | <span data-ttu-id="e6468-139">Organização delegada</span><span class="sxs-lookup"><span data-stu-id="e6468-139">Delegated Org</span></span> | [<span data-ttu-id="e6468-140">Provedor de código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="e6468-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="e6468-141">Aplicativo daemon</span><span class="sxs-lookup"><span data-stu-id="e6468-141">Daemon app</span></span>](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="e6468-142">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="e6468-142">Client Credentials</span></span>  | <span data-ttu-id="e6468-143">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6468-143">App Only</span></span> | [<span data-ttu-id="e6468-144">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="e6468-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="e6468-145">Aplicativo móvel que chama as APIs Web</span><span class="sxs-lookup"><span data-stu-id="e6468-145">Mobile app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="e6468-146">Interativo</span><span class="sxs-lookup"><span data-stu-id="e6468-146">Interactive</span></span> | <span data-ttu-id="e6468-147">Consumidor/org delegada</span><span class="sxs-lookup"><span data-stu-id="e6468-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="e6468-148">Provedor interativo</span><span class="sxs-lookup"><span data-stu-id="e6468-148">Interactive Provider</span></span>](#InteractiveProvider) |


## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a><span data-ttu-id="e6468-149">Provedor de código de autorização</span><span class="sxs-lookup"><span data-stu-id="e6468-149">Authorization code provider</span></span>

<span data-ttu-id="e6468-150">O fluxo de código de autorização permite que aplicativos nativos e Web obtenham tokens com segurança no nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="e6468-150">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="e6468-151">Para saber mais, confira [Microsoft Identity Platform and OAuth 2,0 Authorization Code Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span><span class="sxs-lookup"><span data-stu-id="e6468-151">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="e6468-152">C#</span><span class="sxs-lookup"><span data-stu-id="e6468-152">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="e6468-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6468-153">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="e6468-154">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="e6468-154">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="e6468-155">Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="e6468-155">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="e6468-156">Java</span><span class="sxs-lookup"><span data-stu-id="e6468-156">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="android"></a>[<span data-ttu-id="e6468-157">Android</span><span class="sxs-lookup"><span data-stu-id="e6468-157">Android</span></span>](#tab/Android)

<span data-ttu-id="e6468-158">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-158">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="e6468-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6468-159">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="e6468-160">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-160">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="e6468-161">PHP</span><span class="sxs-lookup"><span data-stu-id="e6468-161">PHP</span></span>](#tab/PHP)

<span data-ttu-id="e6468-162">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-162">Not yet available.</span></span> <span data-ttu-id="e6468-163">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-163">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="e6468-164">Ruby</span><span class="sxs-lookup"><span data-stu-id="e6468-164">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="e6468-165">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="e6468-165">Not available, yet.</span></span> <span data-ttu-id="e6468-166">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-166">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a><span data-ttu-id="e6468-167">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="e6468-167">Client credentials provider</span></span>

<span data-ttu-id="e6468-168">O fluxo de credenciais do cliente permite que aplicativos de serviço sejam executados sem interação do usuário.</span><span class="sxs-lookup"><span data-stu-id="e6468-168">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="e6468-169">O acesso baseia-se na identidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6468-169">Access is based on the identity of the application.</span></span> <span data-ttu-id="e6468-170">Para obter mais informações, consulte [Microsoft Identity Platform e The OAuth 2,0 Client Credentials Flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="e6468-170">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="e6468-171">C#</span><span class="sxs-lookup"><span data-stu-id="e6468-171">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[<span data-ttu-id="e6468-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6468-172">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="e6468-173">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="e6468-173">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="e6468-174">Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="e6468-174">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="e6468-175">Java</span><span class="sxs-lookup"><span data-stu-id="e6468-175">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    NationalCloud.Global);
```

# <a name="android"></a>[<span data-ttu-id="e6468-176">Android</span><span class="sxs-lookup"><span data-stu-id="e6468-176">Android</span></span>](#tab/Android)

<span data-ttu-id="e6468-177">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-177">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="e6468-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6468-178">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="e6468-179">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-179">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="e6468-180">PHP</span><span class="sxs-lookup"><span data-stu-id="e6468-180">PHP</span></span>](#tab/PHP)

<span data-ttu-id="e6468-181">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="e6468-181">Not available, yet.</span></span> <span data-ttu-id="e6468-182">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-182">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="e6468-183">Ruby</span><span class="sxs-lookup"><span data-stu-id="e6468-183">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="e6468-184">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="e6468-184">Not available, yet.</span></span> <span data-ttu-id="e6468-185">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-185">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a><span data-ttu-id="e6468-186">Provedor em nome de</span><span class="sxs-lookup"><span data-stu-id="e6468-186">On-behalf-of provider</span></span>

<span data-ttu-id="e6468-187">O fluxo em nome de é aplicável quando o aplicativo chama uma API de serviço/Web que, em seguida, chama a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e6468-187">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="e6468-188">Saiba mais lendo a [plataforma de identidade da Microsoft e o fluxo em nome de do OAuth 2,0](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="e6468-188">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="c"></a>[<span data-ttu-id="e6468-189">C#</span><span class="sxs-lookup"><span data-stu-id="e6468-189">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="e6468-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6468-190">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="e6468-191">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="e6468-191">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="e6468-192">Leia [usando provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e6468-192">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="java"></a>[<span data-ttu-id="e6468-193">Java</span><span class="sxs-lookup"><span data-stu-id="e6468-193">Java</span></span>](#tab/Java)

<span data-ttu-id="e6468-194">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-194">Not yet available.</span></span> <span data-ttu-id="e6468-195">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-195">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="e6468-196">Android</span><span class="sxs-lookup"><span data-stu-id="e6468-196">Android</span></span>](#tab/Android)

<span data-ttu-id="e6468-197">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-197">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="e6468-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6468-198">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="e6468-199">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-199">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="e6468-200">PHP</span><span class="sxs-lookup"><span data-stu-id="e6468-200">PHP</span></span>](#tab/PHP)

<span data-ttu-id="e6468-201">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-201">Not yet available.</span></span> <span data-ttu-id="e6468-202">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-202">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="e6468-203">Ruby</span><span class="sxs-lookup"><span data-stu-id="e6468-203">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="e6468-204">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-204">Not yet available.</span></span> <span data-ttu-id="e6468-205">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-205">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a><span data-ttu-id="e6468-206">Provedor implícito</span><span class="sxs-lookup"><span data-stu-id="e6468-206">Implicit provider</span></span>

<span data-ttu-id="e6468-207">O fluxo de concessão implícito é usado em aplicativos baseados em navegador.</span><span class="sxs-lookup"><span data-stu-id="e6468-207">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="e6468-208">Para obter mais informações, consulte [Microsoft Identity Platform and implícito Grant Flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="e6468-208">For more information, see [Microsoft identity platform and Implicit grant flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="e6468-209">C#</span><span class="sxs-lookup"><span data-stu-id="e6468-209">C#</span></span>](#tab/CS)

<span data-ttu-id="e6468-210">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-210">Not applicable.</span></span>

# <a name="javascript"></a>[<span data-ttu-id="e6468-211">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6468-211">Javascript</span></span>](#tab/Javascript)

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
const authProvider = new MicrosoftGraph.ImplicitMSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

# <a name="java"></a>[<span data-ttu-id="e6468-212">Java</span><span class="sxs-lookup"><span data-stu-id="e6468-212">Java</span></span>](#tab/Java)

<span data-ttu-id="e6468-213">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-213">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="e6468-214">Android</span><span class="sxs-lookup"><span data-stu-id="e6468-214">Android</span></span>](#tab/Android)

<span data-ttu-id="e6468-215">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-215">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="e6468-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6468-216">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="e6468-217">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-217">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="e6468-218">PHP</span><span class="sxs-lookup"><span data-stu-id="e6468-218">PHP</span></span>](#tab/PHP)

<span data-ttu-id="e6468-219">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-219">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="e6468-220">Ruby</span><span class="sxs-lookup"><span data-stu-id="e6468-220">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="e6468-221">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-221">Not applicable.</span></span>

---

##  <a name="device-code-provider"></a><a name="DeviceCodeProvider"></a><span data-ttu-id="e6468-222">Provedor de código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="e6468-222">Device code provider</span></span>

<span data-ttu-id="e6468-223">O fluxo de código de dispositivo permite entrar em dispositivos por meio de outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e6468-223">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="e6468-224">Para obter detalhes, consulte [plataforma de identidade da Microsoft e o fluxo de código de dispositivo OAuth 2,0](/azure/active-directory/develop/v2-oauth2-device-code).</span><span class="sxs-lookup"><span data-stu-id="e6468-224">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="c"></a>[<span data-ttu-id="e6468-225">C#</span><span class="sxs-lookup"><span data-stu-id="e6468-225">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[<span data-ttu-id="e6468-226">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6468-226">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="e6468-227">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-227">Not yet available.</span></span> <span data-ttu-id="e6468-228">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-228">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="e6468-229">Java</span><span class="sxs-lookup"><span data-stu-id="e6468-229">Java</span></span>](#tab/Java)

<span data-ttu-id="e6468-230">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="e6468-230">Not available, yet.</span></span> <span data-ttu-id="e6468-231">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-231">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="e6468-232">Android</span><span class="sxs-lookup"><span data-stu-id="e6468-232">Android</span></span>](#tab/Android)

<span data-ttu-id="e6468-233">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-233">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="e6468-234">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6468-234">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="e6468-235">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-235">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="e6468-236">PHP</span><span class="sxs-lookup"><span data-stu-id="e6468-236">PHP</span></span>](#tab/PHP)

<span data-ttu-id="e6468-237">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-237">Not yet available.</span></span> <span data-ttu-id="e6468-238">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-238">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="e6468-239">Ruby</span><span class="sxs-lookup"><span data-stu-id="e6468-239">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="e6468-240">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-240">Not yet available.</span></span> <span data-ttu-id="e6468-241">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a><span data-ttu-id="e6468-242">Provedor integrado do Windows</span><span class="sxs-lookup"><span data-stu-id="e6468-242">Integrated Windows provider</span></span>

<span data-ttu-id="e6468-243">O fluxo integrado do Windows oferece uma maneira para que os computadores com Windows adquiram um token de acesso de forma silenciosa quando são associados ao domínio.</span><span class="sxs-lookup"><span data-stu-id="e6468-243">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="e6468-244">Para obter detalhes, consulte [autenticação integrada do Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span><span class="sxs-lookup"><span data-stu-id="e6468-244">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="c"></a>[<span data-ttu-id="e6468-245">C#</span><span class="sxs-lookup"><span data-stu-id="e6468-245">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="e6468-246">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6468-246">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="e6468-247">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-247">Not applicable.</span></span>

# <a name="java"></a>[<span data-ttu-id="e6468-248">Java</span><span class="sxs-lookup"><span data-stu-id="e6468-248">Java</span></span>](#tab/Java)

<span data-ttu-id="e6468-249">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-249">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="e6468-250">Android</span><span class="sxs-lookup"><span data-stu-id="e6468-250">Android</span></span>](#tab/Android)

<span data-ttu-id="e6468-251">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-251">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="e6468-252">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6468-252">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="e6468-253">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-253">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="e6468-254">PHP</span><span class="sxs-lookup"><span data-stu-id="e6468-254">PHP</span></span>](#tab/PHP)

<span data-ttu-id="e6468-255">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-255">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="e6468-256">Ruby</span><span class="sxs-lookup"><span data-stu-id="e6468-256">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="e6468-257">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-257">Not applicable.</span></span>

---

##  <a name="interactive-provider"></a><a name="InteractiveProvider"></a><span data-ttu-id="e6468-258">Provedor interativo</span><span class="sxs-lookup"><span data-stu-id="e6468-258">Interactive provider</span></span>

<span data-ttu-id="e6468-259">O fluxo interativo é usado por aplicativos móveis (Xamarin e UWP) e aplicativos de área de trabalho para chamar o Microsoft Graph no nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e6468-259">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="e6468-260">Para obter detalhes, consulte [adquirindo tokens interativamente](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span><span class="sxs-lookup"><span data-stu-id="e6468-260">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="c"></a>[<span data-ttu-id="e6468-261">C#</span><span class="sxs-lookup"><span data-stu-id="e6468-261">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="e6468-262">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6468-262">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="e6468-263">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-263">Not yet available.</span></span> <span data-ttu-id="e6468-264">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-264">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="e6468-265">Java</span><span class="sxs-lookup"><span data-stu-id="e6468-265">Java</span></span>](#tab/Java)

<span data-ttu-id="e6468-266">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-266">Not yet available.</span></span> <span data-ttu-id="e6468-267">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-267">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="e6468-268">Android</span><span class="sxs-lookup"><span data-stu-id="e6468-268">Android</span></span>](#tab/Android)

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

# <a name="objective-c"></a>[<span data-ttu-id="e6468-269">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6468-269">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[<span data-ttu-id="e6468-270">PHP</span><span class="sxs-lookup"><span data-stu-id="e6468-270">PHP</span></span>](#tab/PHP)

<span data-ttu-id="e6468-271">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-271">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="e6468-272">Ruby</span><span class="sxs-lookup"><span data-stu-id="e6468-272">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="e6468-273">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-273">Not applicable.</span></span>

---

##  <a name="usernamepassword-provider"></a><a name="UsernamePasswordProvider"></a><span data-ttu-id="e6468-274">Provedor de nome de usuário/senha</span><span class="sxs-lookup"><span data-stu-id="e6468-274">Username/password provider</span></span>

<span data-ttu-id="e6468-275">O provedor de nome de usuário/senha permite que um aplicativo entre em um usuário usando seu nome de usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="e6468-275">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="e6468-276">Use este fluxo somente quando não for possível usar qualquer um dos outros fluxos OAuth.</span><span class="sxs-lookup"><span data-stu-id="e6468-276">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="e6468-277">Para obter mais informações, consulte [plataforma de identidade da Microsoft e a credencial de senha de proprietário do recurso OAuth 2,0](/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="e6468-277">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="c"></a>[<span data-ttu-id="e6468-278">C#</span><span class="sxs-lookup"><span data-stu-id="e6468-278">C#</span></span>](#tab/CS)

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

# <a name="javascript"></a>[<span data-ttu-id="e6468-279">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6468-279">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="e6468-280">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-280">Not yet available.</span></span> <span data-ttu-id="e6468-281">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-281">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="e6468-282">Java</span><span class="sxs-lookup"><span data-stu-id="e6468-282">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="android"></a>[<span data-ttu-id="e6468-283">Android</span><span class="sxs-lookup"><span data-stu-id="e6468-283">Android</span></span>](#tab/Android)

<span data-ttu-id="e6468-284">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-284">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="e6468-285">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6468-285">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="e6468-286">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="e6468-286">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="e6468-287">PHP</span><span class="sxs-lookup"><span data-stu-id="e6468-287">PHP</span></span>](#tab/PHP)

<span data-ttu-id="e6468-288">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-288">Not yet available.</span></span> <span data-ttu-id="e6468-289">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="e6468-290">Ruby</span><span class="sxs-lookup"><span data-stu-id="e6468-290">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="e6468-291">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="e6468-291">Not yet available.</span></span> <span data-ttu-id="e6468-292">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="e6468-292">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="e6468-293">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e6468-293">Next steps</span></span>

* <span data-ttu-id="e6468-294">Os provedores de autenticação exigem uma ID de cliente.</span><span class="sxs-lookup"><span data-stu-id="e6468-294">Authentication providers require an client ID.</span></span> <span data-ttu-id="e6468-295">Você deve [registrar seu aplicativo](https://portal.azure.com/) depois de configurar seu provedor de autenticação.</span><span class="sxs-lookup"><span data-stu-id="e6468-295">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="e6468-296">Deixe-nos saber se um fluxo OAuth necessário atualmente não é suportado pela votação ou pela abertura de uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span><span class="sxs-lookup"><span data-stu-id="e6468-296">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
