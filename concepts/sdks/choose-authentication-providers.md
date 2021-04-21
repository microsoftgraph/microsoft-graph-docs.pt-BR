---
title: Escolher um provedor de autenticação do Microsoft Graph
description: Saiba como escolher provedores de autenticação específicos de cenário para seu aplicativo.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 726fbf1334a99ab6a854bd4627052d154187105c
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921123"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="ebc39-103">Escolha um provedor de autenticação do Microsoft Graph com base no cenário</span><span class="sxs-lookup"><span data-stu-id="ebc39-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="ebc39-104">Os provedores de autenticação implementam o código necessário para adquirir um token usando a Biblioteca de Autenticação da Microsoft (MSAL); lidar com vários erros potenciais para casos como consentimento incremental, senhas expiradas e acesso condicional; e, em seguida, de definir o cabeçalho de autorização de solicitação HTTP.</span><span class="sxs-lookup"><span data-stu-id="ebc39-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="ebc39-105">A tabela a seguir lista o conjunto de provedores que combinam com os cenários de diferentes tipos [de aplicativo.](/azure/active-directory/develop/v2-app-types)</span><span class="sxs-lookup"><span data-stu-id="ebc39-105">The following table lists the set of providers that match the scenarios for different [application types](/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="ebc39-106">Cenário</span><span class="sxs-lookup"><span data-stu-id="ebc39-106">Scenario</span></span> | <span data-ttu-id="ebc39-107">Fluxo/Concessão</span><span class="sxs-lookup"><span data-stu-id="ebc39-107">Flow/Grant</span></span> | <span data-ttu-id="ebc39-108">Espectadores</span><span class="sxs-lookup"><span data-stu-id="ebc39-108">Audience</span></span> | <span data-ttu-id="ebc39-109">Provedor</span><span class="sxs-lookup"><span data-stu-id="ebc39-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="ebc39-110">Aplicativo de Página Única</span><span class="sxs-lookup"><span data-stu-id="ebc39-110">Single Page App</span></span>](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="ebc39-111">Implícito</span><span class="sxs-lookup"><span data-stu-id="ebc39-111">Implicit</span></span> | <span data-ttu-id="ebc39-112">Consumidor Delegado/Org</span><span class="sxs-lookup"><span data-stu-id="ebc39-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="ebc39-113">Provedor Implícito</span><span class="sxs-lookup"><span data-stu-id="ebc39-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="ebc39-114">Aplicativo Web que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="ebc39-114">Web App that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="ebc39-115">Código de Autorização</span><span class="sxs-lookup"><span data-stu-id="ebc39-115">Authorization Code</span></span> | <span data-ttu-id="ebc39-116">Consumidor Delegado/Org</span><span class="sxs-lookup"><span data-stu-id="ebc39-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="ebc39-117">Provedor de Código de Autorização</span><span class="sxs-lookup"><span data-stu-id="ebc39-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="ebc39-118">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="ebc39-118">Client Credentials</span></span>  | <span data-ttu-id="ebc39-119">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebc39-119">App Only</span></span> | [<span data-ttu-id="ebc39-120">Provedor de Credenciais do Cliente</span><span class="sxs-lookup"><span data-stu-id="ebc39-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="ebc39-121">API Web que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="ebc39-121">Web API that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="ebc39-122">Em nome de</span><span class="sxs-lookup"><span data-stu-id="ebc39-122">On Behalf Of</span></span> | <span data-ttu-id="ebc39-123">Consumidor Delegado/Org</span><span class="sxs-lookup"><span data-stu-id="ebc39-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="ebc39-124">Em nome do provedor</span><span class="sxs-lookup"><span data-stu-id="ebc39-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="ebc39-125">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="ebc39-125">Client Credentials</span></span>  | <span data-ttu-id="ebc39-126">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebc39-126">App Only</span></span> | [<span data-ttu-id="ebc39-127">Provedor de Credenciais do Cliente</span><span class="sxs-lookup"><span data-stu-id="ebc39-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="ebc39-128">Aplicativo de área de trabalho que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="ebc39-128">Desktop app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="ebc39-129">Interativo</span><span class="sxs-lookup"><span data-stu-id="ebc39-129">Interactive</span></span> | <span data-ttu-id="ebc39-130">Consumidor Delegado/Org</span><span class="sxs-lookup"><span data-stu-id="ebc39-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="ebc39-131">Provedor Interativo</span><span class="sxs-lookup"><span data-stu-id="ebc39-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="ebc39-132">Windows integrado</span><span class="sxs-lookup"><span data-stu-id="ebc39-132">Integrated Windows</span></span> | <span data-ttu-id="ebc39-133">Organização Delegada</span><span class="sxs-lookup"><span data-stu-id="ebc39-133">Delegated Org</span></span> | [<span data-ttu-id="ebc39-134">Provedor Integrado do Windows</span><span class="sxs-lookup"><span data-stu-id="ebc39-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="ebc39-135">Proprietário do Recurso</span><span class="sxs-lookup"><span data-stu-id="ebc39-135">Resource Owner</span></span>  | <span data-ttu-id="ebc39-136">Organização Delegada</span><span class="sxs-lookup"><span data-stu-id="ebc39-136">Delegated Org</span></span> | [<span data-ttu-id="ebc39-137">Username /Password Provider</span><span class="sxs-lookup"><span data-stu-id="ebc39-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="ebc39-138">Código do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ebc39-138">Device Code</span></span>  | <span data-ttu-id="ebc39-139">Organização Delegada</span><span class="sxs-lookup"><span data-stu-id="ebc39-139">Delegated Org</span></span> | [<span data-ttu-id="ebc39-140">Provedor de Código de Dispositivo</span><span class="sxs-lookup"><span data-stu-id="ebc39-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="ebc39-141">Aplicativo Daemon</span><span class="sxs-lookup"><span data-stu-id="ebc39-141">Daemon app</span></span>](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="ebc39-142">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="ebc39-142">Client Credentials</span></span>  | <span data-ttu-id="ebc39-143">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebc39-143">App Only</span></span> | [<span data-ttu-id="ebc39-144">Provedor de Credenciais do Cliente</span><span class="sxs-lookup"><span data-stu-id="ebc39-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="ebc39-145">Aplicativo móvel que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="ebc39-145">Mobile app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="ebc39-146">Interativo</span><span class="sxs-lookup"><span data-stu-id="ebc39-146">Interactive</span></span> | <span data-ttu-id="ebc39-147">Consumidor Delegado/Org</span><span class="sxs-lookup"><span data-stu-id="ebc39-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="ebc39-148">Provedor Interativo</span><span class="sxs-lookup"><span data-stu-id="ebc39-148">Interactive Provider</span></span>](#InteractiveProvider) |

> <span data-ttu-id="ebc39-149">Observação: Java desenvolvedores android precisam adicionar a biblioteca [do azure-identity](/java/api/overview/azure/identity-readme?view=azure-java-stable) para obter acesso aos diferentes tipos de credenciais.</span><span class="sxs-lookup"><span data-stu-id="ebc39-149">Note: Java and android developers need to add the [azure-identity](/java/api/overview/azure/identity-readme?view=azure-java-stable) library in order to get access to the different credentials types.</span></span>

## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a><span data-ttu-id="ebc39-150">Provedor de código de autorização</span><span class="sxs-lookup"><span data-stu-id="ebc39-150">Authorization code provider</span></span>

<span data-ttu-id="ebc39-151">O fluxo de código de autorização permite que aplicativos nativos e web obtenham tokens com segurança no nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="ebc39-151">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="ebc39-152">Para saber mais, confira [Microsoft identity platform and OAuth 2.0 authorization code flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span><span class="sxs-lookup"><span data-stu-id="ebc39-152">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="ebc39-153">C#</span><span class="sxs-lookup"><span data-stu-id="ebc39-153">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="ebc39-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="ebc39-154">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ebc39-155">O código de autorização, a credencial do cliente e os fluxos em nome do OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="ebc39-155">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="ebc39-156">Para obter mais informações, consulte [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="ebc39-156">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="ebc39-157">Java</span><span class="sxs-lookup"><span data-stu-id="ebc39-157">Java</span></span>](#tab/Java)

```java
final AuthorizationCodeCredential authCodeCredential = new AuthorizationCodeCredentialBuilder()
        .clientId(clientId)
        .clientSecret(clientSecret) //required for web apps, do not set for native apps
        .authorizationCode(authorizationCode)
        .redirectUrl(redirectUri)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, authCodeCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="ebc39-158">Android</span><span class="sxs-lookup"><span data-stu-id="ebc39-158">Android</span></span>](#tab/Android)

<span data-ttu-id="ebc39-159">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-159">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ebc39-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebc39-160">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ebc39-161">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-161">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ebc39-162">PHP</span><span class="sxs-lookup"><span data-stu-id="ebc39-162">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ebc39-163">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-163">Not yet available.</span></span> <span data-ttu-id="ebc39-164">Dê suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-164">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ebc39-165">Ruby</span><span class="sxs-lookup"><span data-stu-id="ebc39-165">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ebc39-166">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-166">Not available, yet.</span></span> <span data-ttu-id="ebc39-167">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-167">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a><span data-ttu-id="ebc39-168">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="ebc39-168">Client credentials provider</span></span>

<span data-ttu-id="ebc39-169">O fluxo de credenciais do cliente permite que aplicativos de serviço executem sem interação do usuário.</span><span class="sxs-lookup"><span data-stu-id="ebc39-169">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="ebc39-170">O Access baseia-se na identidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ebc39-170">Access is based on the identity of the application.</span></span> <span data-ttu-id="ebc39-171">Para obter mais informações, [consulte Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="ebc39-171">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="ebc39-172">C#</span><span class="sxs-lookup"><span data-stu-id="ebc39-172">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[<span data-ttu-id="ebc39-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="ebc39-173">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ebc39-174">O código de autorização, a credencial do cliente e os fluxos em nome do OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="ebc39-174">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="ebc39-175">Para obter mais informações, consulte [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="ebc39-175">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="ebc39-176">Java</span><span class="sxs-lookup"><span data-stu-id="ebc39-176">Java</span></span>](#tab/Java)

```java
final ClientSecretCredential clientSecretCredential = new ClientSecretCredentialBuilder()
        .clientId(clientId)
        .clientSecret(clientSecret)
        .tenantId(tenant)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, clientSecretCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="ebc39-177">Android</span><span class="sxs-lookup"><span data-stu-id="ebc39-177">Android</span></span>](#tab/Android)

<span data-ttu-id="ebc39-178">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-178">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ebc39-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebc39-179">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ebc39-180">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-180">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ebc39-181">PHP</span><span class="sxs-lookup"><span data-stu-id="ebc39-181">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ebc39-182">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-182">Not available, yet.</span></span> <span data-ttu-id="ebc39-183">Dê suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-183">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ebc39-184">Ruby</span><span class="sxs-lookup"><span data-stu-id="ebc39-184">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ebc39-185">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-185">Not available, yet.</span></span> <span data-ttu-id="ebc39-186">Dê suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-186">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a><span data-ttu-id="ebc39-187">Provedor on-behalf-of</span><span class="sxs-lookup"><span data-stu-id="ebc39-187">On-behalf-of provider</span></span>

<span data-ttu-id="ebc39-188">O fluxo em nome do fluxo é aplicável quando seu aplicativo chama uma API de serviço/Web que, por sua vez, chama a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ebc39-188">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="ebc39-189">Saiba mais lendo a plataforma de identidade da Microsoft e o [fluxo OAuth 2.0 On-Behalf-Of](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="ebc39-189">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="c"></a>[<span data-ttu-id="ebc39-190">C#</span><span class="sxs-lookup"><span data-stu-id="ebc39-190">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="ebc39-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="ebc39-191">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ebc39-192">O código de autorização, a credencial do cliente e os fluxos em nome do OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="ebc39-192">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="ebc39-193">Leia [Usando o Provedor de Autenticação Personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="ebc39-193">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="java"></a>[<span data-ttu-id="ebc39-194">Java</span><span class="sxs-lookup"><span data-stu-id="ebc39-194">Java</span></span>](#tab/Java)

<span data-ttu-id="ebc39-195">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-195">Not yet available.</span></span> <span data-ttu-id="ebc39-196">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-196">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="ebc39-197">Android</span><span class="sxs-lookup"><span data-stu-id="ebc39-197">Android</span></span>](#tab/Android)

<span data-ttu-id="ebc39-198">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-198">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ebc39-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebc39-199">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ebc39-200">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-200">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ebc39-201">PHP</span><span class="sxs-lookup"><span data-stu-id="ebc39-201">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ebc39-202">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-202">Not yet available.</span></span> <span data-ttu-id="ebc39-203">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-203">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ebc39-204">Ruby</span><span class="sxs-lookup"><span data-stu-id="ebc39-204">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ebc39-205">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-205">Not yet available.</span></span> <span data-ttu-id="ebc39-206">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-206">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a><span data-ttu-id="ebc39-207">Provedor implícito</span><span class="sxs-lookup"><span data-stu-id="ebc39-207">Implicit provider</span></span>

<span data-ttu-id="ebc39-208">O fluxo de concessão implícito é usado em aplicativos baseados em navegador.</span><span class="sxs-lookup"><span data-stu-id="ebc39-208">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="ebc39-209">Para obter mais informações, consulte [Plataforma de identidade da Microsoft e Fluxo de concessão implícito.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)</span><span class="sxs-lookup"><span data-stu-id="ebc39-209">For more information, see [Microsoft identity platform and Implicit grant flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="ebc39-210">C#</span><span class="sxs-lookup"><span data-stu-id="ebc39-210">C#</span></span>](#tab/CS)

<span data-ttu-id="ebc39-211">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-211">Not applicable.</span></span>

# <a name="javascript"></a>[<span data-ttu-id="ebc39-212">Javascript</span><span class="sxs-lookup"><span data-stu-id="ebc39-212">Javascript</span></span>](#tab/Javascript)

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

# <a name="java"></a>[<span data-ttu-id="ebc39-213">Java</span><span class="sxs-lookup"><span data-stu-id="ebc39-213">Java</span></span>](#tab/Java)

<span data-ttu-id="ebc39-214">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-214">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="ebc39-215">Android</span><span class="sxs-lookup"><span data-stu-id="ebc39-215">Android</span></span>](#tab/Android)

<span data-ttu-id="ebc39-216">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-216">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ebc39-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebc39-217">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ebc39-218">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-218">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ebc39-219">PHP</span><span class="sxs-lookup"><span data-stu-id="ebc39-219">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ebc39-220">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-220">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ebc39-221">Ruby</span><span class="sxs-lookup"><span data-stu-id="ebc39-221">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ebc39-222">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-222">Not applicable.</span></span>

---

##  <a name="device-code-provider"></a><a name="DeviceCodeProvider"></a><span data-ttu-id="ebc39-223">Provedor de código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="ebc39-223">Device code provider</span></span>

<span data-ttu-id="ebc39-224">O fluxo de código do dispositivo permite entrar em dispositivos por meio de outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebc39-224">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="ebc39-225">Para obter detalhes, [consulte Microsoft identity platform and the OAuth 2.0 device code flow](/azure/active-directory/develop/v2-oauth2-device-code).</span><span class="sxs-lookup"><span data-stu-id="ebc39-225">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="c"></a>[<span data-ttu-id="ebc39-226">C#</span><span class="sxs-lookup"><span data-stu-id="ebc39-226">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[<span data-ttu-id="ebc39-227">Javascript</span><span class="sxs-lookup"><span data-stu-id="ebc39-227">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ebc39-228">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-228">Not yet available.</span></span> <span data-ttu-id="ebc39-229">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-229">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="ebc39-230">Java</span><span class="sxs-lookup"><span data-stu-id="ebc39-230">Java</span></span>](#tab/Java)

```java
final DeviceCodeCredential deviceCodeCredential = new DeviceCodeCredentialBuilder()
                    .clientId(clientId)
                    .challengeConsumer(challenge -> {
                        // lets user know of the challenge
                        System.out.println(challenge.getMessage());
                    })
                    .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, deviceCodeCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="ebc39-231">Android</span><span class="sxs-lookup"><span data-stu-id="ebc39-231">Android</span></span>](#tab/Android)

<span data-ttu-id="ebc39-232">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-232">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ebc39-233">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebc39-233">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ebc39-234">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-234">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ebc39-235">PHP</span><span class="sxs-lookup"><span data-stu-id="ebc39-235">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ebc39-236">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-236">Not yet available.</span></span> <span data-ttu-id="ebc39-237">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-237">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ebc39-238">Ruby</span><span class="sxs-lookup"><span data-stu-id="ebc39-238">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ebc39-239">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-239">Not yet available.</span></span> <span data-ttu-id="ebc39-240">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-240">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a><span data-ttu-id="ebc39-241">Provedor integrado do Windows</span><span class="sxs-lookup"><span data-stu-id="ebc39-241">Integrated Windows provider</span></span>

<span data-ttu-id="ebc39-242">O fluxo integrado do Windows fornece uma maneira para os computadores Windows adquirirem silenciosamente um token de acesso quando eles estão ingressados no domínio.</span><span class="sxs-lookup"><span data-stu-id="ebc39-242">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="ebc39-243">Para obter detalhes, consulte [Autenticação integrada do Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span><span class="sxs-lookup"><span data-stu-id="ebc39-243">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="c"></a>[<span data-ttu-id="ebc39-244">C#</span><span class="sxs-lookup"><span data-stu-id="ebc39-244">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="ebc39-245">Javascript</span><span class="sxs-lookup"><span data-stu-id="ebc39-245">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ebc39-246">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-246">Not applicable.</span></span>

# <a name="java"></a>[<span data-ttu-id="ebc39-247">Java</span><span class="sxs-lookup"><span data-stu-id="ebc39-247">Java</span></span>](#tab/Java)

<span data-ttu-id="ebc39-248">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-248">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="ebc39-249">Android</span><span class="sxs-lookup"><span data-stu-id="ebc39-249">Android</span></span>](#tab/Android)

<span data-ttu-id="ebc39-250">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-250">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ebc39-251">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebc39-251">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ebc39-252">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-252">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ebc39-253">PHP</span><span class="sxs-lookup"><span data-stu-id="ebc39-253">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ebc39-254">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-254">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ebc39-255">Ruby</span><span class="sxs-lookup"><span data-stu-id="ebc39-255">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ebc39-256">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-256">Not applicable.</span></span>

---

##  <a name="interactive-provider"></a><a name="InteractiveProvider"></a><span data-ttu-id="ebc39-257">Provedor interativo</span><span class="sxs-lookup"><span data-stu-id="ebc39-257">Interactive provider</span></span>

<span data-ttu-id="ebc39-258">O fluxo interativo é usado por aplicativos móveis (Xamarin e UWP) e aplicativos de área de trabalho para chamar o Microsoft Graph em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ebc39-258">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="ebc39-259">Para obter detalhes, consulte [Adquirindo tokens interativamente](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span><span class="sxs-lookup"><span data-stu-id="ebc39-259">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="c"></a>[<span data-ttu-id="ebc39-260">C#</span><span class="sxs-lookup"><span data-stu-id="ebc39-260">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="ebc39-261">Javascript</span><span class="sxs-lookup"><span data-stu-id="ebc39-261">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ebc39-262">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-262">Not yet available.</span></span> <span data-ttu-id="ebc39-263">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-263">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="ebc39-264">Java</span><span class="sxs-lookup"><span data-stu-id="ebc39-264">Java</span></span>](#tab/Java)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(clientId)
                .redirectUrl("http://localhost:8765")
                .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, interactiveBrowserCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="ebc39-265">Android</span><span class="sxs-lookup"><span data-stu-id="ebc39-265">Android</span></span>](#tab/Android)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(clientId)
                .redirectUrl("http://localhost:8765")
                .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, interactiveBrowserCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="objective-c"></a>[<span data-ttu-id="ebc39-266">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebc39-266">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[<span data-ttu-id="ebc39-267">PHP</span><span class="sxs-lookup"><span data-stu-id="ebc39-267">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ebc39-268">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-268">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ebc39-269">Ruby</span><span class="sxs-lookup"><span data-stu-id="ebc39-269">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ebc39-270">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-270">Not applicable.</span></span>

---

##  <a name="usernamepassword-provider"></a><a name="UsernamePasswordProvider"></a><span data-ttu-id="ebc39-271">Provedor de nome de usuário/senha</span><span class="sxs-lookup"><span data-stu-id="ebc39-271">Username/password provider</span></span>

<span data-ttu-id="ebc39-272">O provedor de nome de usuário/senha permite que um aplicativo entre em um usuário usando seu nome de usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="ebc39-272">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="ebc39-273">Use esse fluxo somente quando você não puder usar nenhum dos outros fluxos OAuth.</span><span class="sxs-lookup"><span data-stu-id="ebc39-273">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="ebc39-274">Para obter mais informações, [consulte Microsoft identity platform and the OAuth 2.0 resource owner password credential](/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="ebc39-274">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="c"></a>[<span data-ttu-id="ebc39-275">C#</span><span class="sxs-lookup"><span data-stu-id="ebc39-275">C#</span></span>](#tab/CS)

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

# <a name="javascript"></a>[<span data-ttu-id="ebc39-276">Javascript</span><span class="sxs-lookup"><span data-stu-id="ebc39-276">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="ebc39-277">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-277">Not yet available.</span></span> <span data-ttu-id="ebc39-278">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-278">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="ebc39-279">Java</span><span class="sxs-lookup"><span data-stu-id="ebc39-279">Java</span></span>](#tab/Java)

```java
final UsernamePasswordCredential usernamePasswordCredential = new UsernamePasswordCredentialBuilder()
        .clientId(clientId)
        .username(username)
        .password(password)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, usernamePasswordCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[<span data-ttu-id="ebc39-280">Android</span><span class="sxs-lookup"><span data-stu-id="ebc39-280">Android</span></span>](#tab/Android)

<span data-ttu-id="ebc39-281">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-281">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="ebc39-282">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebc39-282">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="ebc39-283">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="ebc39-283">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="ebc39-284">PHP</span><span class="sxs-lookup"><span data-stu-id="ebc39-284">PHP</span></span>](#tab/PHP)

<span data-ttu-id="ebc39-285">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-285">Not yet available.</span></span> <span data-ttu-id="ebc39-286">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-286">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="ebc39-287">Ruby</span><span class="sxs-lookup"><span data-stu-id="ebc39-287">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="ebc39-288">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="ebc39-288">Not yet available.</span></span> <span data-ttu-id="ebc39-289">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="ebc39-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="ebc39-290">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ebc39-290">Next steps</span></span>

* <span data-ttu-id="ebc39-291">Os provedores de autenticação exigem uma ID do cliente.</span><span class="sxs-lookup"><span data-stu-id="ebc39-291">Authentication providers require an client ID.</span></span> <span data-ttu-id="ebc39-292">Você vai querer registrar [seu aplicativo depois](https://portal.azure.com/) de configurar seu provedor de autenticação.</span><span class="sxs-lookup"><span data-stu-id="ebc39-292">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="ebc39-293">Deixe-nos saber se um fluxo OAuth necessário não tem suporte no momento votando ou abrindo uma solicitação de recurso [do Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)</span><span class="sxs-lookup"><span data-stu-id="ebc39-293">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>