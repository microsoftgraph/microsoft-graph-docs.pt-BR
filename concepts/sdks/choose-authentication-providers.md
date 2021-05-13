---
title: Escolha um provedor de autenticação Graph microsoft
description: Saiba como escolher provedores de autenticação específicos de cenário para seu aplicativo.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 0cdc407187ea0b5befc3704f877b1df11aeda545
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475532"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="a98c3-103">Escolha um provedor Graph de autenticação da Microsoft com base no cenário</span><span class="sxs-lookup"><span data-stu-id="a98c3-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="a98c3-104">Os provedores de autenticação implementam o código necessário para adquirir um token usando a Biblioteca de Autenticação da Microsoft (MSAL); lidar com vários erros potenciais para casos como consentimento incremental, senhas expiradas e acesso condicional; e, em seguida, de definir o cabeçalho de autorização de solicitação HTTP.</span><span class="sxs-lookup"><span data-stu-id="a98c3-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="a98c3-105">A tabela a seguir lista o conjunto de provedores que combinam com os cenários de diferentes tipos [de aplicativo.](/azure/active-directory/develop/v2-app-types)</span><span class="sxs-lookup"><span data-stu-id="a98c3-105">The following table lists the set of providers that match the scenarios for different [application types](/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="a98c3-106">Cenário</span><span class="sxs-lookup"><span data-stu-id="a98c3-106">Scenario</span></span> | <span data-ttu-id="a98c3-107">Flow/Grant</span><span class="sxs-lookup"><span data-stu-id="a98c3-107">Flow/Grant</span></span> | <span data-ttu-id="a98c3-108">Espectadores</span><span class="sxs-lookup"><span data-stu-id="a98c3-108">Audience</span></span> | <span data-ttu-id="a98c3-109">Provedor</span><span class="sxs-lookup"><span data-stu-id="a98c3-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="a98c3-110">Aplicativo de Página Única</span><span class="sxs-lookup"><span data-stu-id="a98c3-110">Single Page App</span></span>](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="a98c3-111">Implícito</span><span class="sxs-lookup"><span data-stu-id="a98c3-111">Implicit</span></span> | <span data-ttu-id="a98c3-112">Consumidor Delegado/Org</span><span class="sxs-lookup"><span data-stu-id="a98c3-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="a98c3-113">Provedor Implícito</span><span class="sxs-lookup"><span data-stu-id="a98c3-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="a98c3-114">Aplicativo Web que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="a98c3-114">Web App that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="a98c3-115">Código de Autorização</span><span class="sxs-lookup"><span data-stu-id="a98c3-115">Authorization Code</span></span> | <span data-ttu-id="a98c3-116">Consumidor Delegado/Org</span><span class="sxs-lookup"><span data-stu-id="a98c3-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="a98c3-117">Provedor de Código de Autorização</span><span class="sxs-lookup"><span data-stu-id="a98c3-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="a98c3-118">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="a98c3-118">Client Credentials</span></span>  | <span data-ttu-id="a98c3-119">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="a98c3-119">App Only</span></span> | [<span data-ttu-id="a98c3-120">Provedor de Credenciais do Cliente</span><span class="sxs-lookup"><span data-stu-id="a98c3-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="a98c3-121">API Web que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="a98c3-121">Web API that calls web APIs</span></span>](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="a98c3-122">Em nome de</span><span class="sxs-lookup"><span data-stu-id="a98c3-122">On Behalf Of</span></span> | <span data-ttu-id="a98c3-123">Consumidor Delegado/Org</span><span class="sxs-lookup"><span data-stu-id="a98c3-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="a98c3-124">Em nome do provedor</span><span class="sxs-lookup"><span data-stu-id="a98c3-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="a98c3-125">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="a98c3-125">Client Credentials</span></span>  | <span data-ttu-id="a98c3-126">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="a98c3-126">App Only</span></span> | [<span data-ttu-id="a98c3-127">Provedor de Credenciais do Cliente</span><span class="sxs-lookup"><span data-stu-id="a98c3-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="a98c3-128">Aplicativo de área de trabalho que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="a98c3-128">Desktop app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="a98c3-129">Interativo</span><span class="sxs-lookup"><span data-stu-id="a98c3-129">Interactive</span></span> | <span data-ttu-id="a98c3-130">Consumidor Delegado/Org</span><span class="sxs-lookup"><span data-stu-id="a98c3-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="a98c3-131">Provedor Interativo</span><span class="sxs-lookup"><span data-stu-id="a98c3-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="a98c3-132">Integração Windows</span><span class="sxs-lookup"><span data-stu-id="a98c3-132">Integrated Windows</span></span> | <span data-ttu-id="a98c3-133">Organização Delegada</span><span class="sxs-lookup"><span data-stu-id="a98c3-133">Delegated Org</span></span> | [<span data-ttu-id="a98c3-134">Provedor Windows integrado</span><span class="sxs-lookup"><span data-stu-id="a98c3-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="a98c3-135">Proprietário do Recurso</span><span class="sxs-lookup"><span data-stu-id="a98c3-135">Resource Owner</span></span>  | <span data-ttu-id="a98c3-136">Organização Delegada</span><span class="sxs-lookup"><span data-stu-id="a98c3-136">Delegated Org</span></span> | [<span data-ttu-id="a98c3-137">Username /Password Provider</span><span class="sxs-lookup"><span data-stu-id="a98c3-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="a98c3-138">Código do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a98c3-138">Device Code</span></span>  | <span data-ttu-id="a98c3-139">Organização Delegada</span><span class="sxs-lookup"><span data-stu-id="a98c3-139">Delegated Org</span></span> | [<span data-ttu-id="a98c3-140">Provedor de Código de Dispositivo</span><span class="sxs-lookup"><span data-stu-id="a98c3-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="a98c3-141">Aplicativo Daemon</span><span class="sxs-lookup"><span data-stu-id="a98c3-141">Daemon app</span></span>](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="a98c3-142">Credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="a98c3-142">Client Credentials</span></span>  | <span data-ttu-id="a98c3-143">Somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="a98c3-143">App Only</span></span> | [<span data-ttu-id="a98c3-144">Provedor de Credenciais do Cliente</span><span class="sxs-lookup"><span data-stu-id="a98c3-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="a98c3-145">Aplicativo móvel que chama APIs da Web</span><span class="sxs-lookup"><span data-stu-id="a98c3-145">Mobile app that calls web APIs</span></span>](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="a98c3-146">Interativo</span><span class="sxs-lookup"><span data-stu-id="a98c3-146">Interactive</span></span> | <span data-ttu-id="a98c3-147">Consumidor Delegado/Org</span><span class="sxs-lookup"><span data-stu-id="a98c3-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="a98c3-148">Provedor Interativo</span><span class="sxs-lookup"><span data-stu-id="a98c3-148">Interactive Provider</span></span>](#InteractiveProvider) |

> <span data-ttu-id="a98c3-149">Observação: Java desenvolvedores android precisam adicionar a biblioteca [do azure-identity](/java/api/overview/azure/identity-readme?view=azure-java-stable) para obter acesso aos diferentes tipos de credenciais.</span><span class="sxs-lookup"><span data-stu-id="a98c3-149">Note: Java and android developers need to add the [azure-identity](/java/api/overview/azure/identity-readme?view=azure-java-stable) library in order to get access to the different credentials types.</span></span>

## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a><span data-ttu-id="a98c3-150">Provedor de código de autorização</span><span class="sxs-lookup"><span data-stu-id="a98c3-150">Authorization code provider</span></span>

<span data-ttu-id="a98c3-151">O fluxo de código de autorização permite que aplicativos nativos e web obtenham tokens com segurança no nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="a98c3-151">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="a98c3-152">Para saber mais, confira plataforma de identidade da Microsoft fluxo de código de autorização [do OAuth 2.0](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span><span class="sxs-lookup"><span data-stu-id="a98c3-152">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="a98c3-153">C#</span><span class="sxs-lookup"><span data-stu-id="a98c3-153">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="a98c3-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="a98c3-154">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a98c3-155">O código de autorização, a credencial do cliente e os fluxos em nome do OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="a98c3-155">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="a98c3-156">Para obter mais informações, consulte [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="a98c3-156">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="a98c3-157">Java</span><span class="sxs-lookup"><span data-stu-id="a98c3-157">Java</span></span>](#tab/Java)

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

# <a name="android"></a>[<span data-ttu-id="a98c3-158">Android</span><span class="sxs-lookup"><span data-stu-id="a98c3-158">Android</span></span>](#tab/Android)

<span data-ttu-id="a98c3-159">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-159">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="a98c3-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a98c3-160">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a98c3-161">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-161">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="a98c3-162">PHP</span><span class="sxs-lookup"><span data-stu-id="a98c3-162">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a98c3-163">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-163">Not yet available.</span></span> <span data-ttu-id="a98c3-164">Dê suporte ou abra uma solicitação [de recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-164">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="a98c3-165">Ruby</span><span class="sxs-lookup"><span data-stu-id="a98c3-165">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a98c3-166">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-166">Not available, yet.</span></span> <span data-ttu-id="a98c3-167">Vote ou abra uma solicitação de [recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-167">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a><span data-ttu-id="a98c3-168">Provedor de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="a98c3-168">Client credentials provider</span></span>

<span data-ttu-id="a98c3-169">O fluxo de credenciais do cliente permite que aplicativos de serviço executem sem interação do usuário.</span><span class="sxs-lookup"><span data-stu-id="a98c3-169">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="a98c3-170">O Access baseia-se na identidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a98c3-170">Access is based on the identity of the application.</span></span> <span data-ttu-id="a98c3-171">Para obter mais informações, consulte plataforma de identidade da Microsoft e o fluxo de credenciais do cliente [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)</span><span class="sxs-lookup"><span data-stu-id="a98c3-171">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="a98c3-172">C#</span><span class="sxs-lookup"><span data-stu-id="a98c3-172">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[<span data-ttu-id="a98c3-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="a98c3-173">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a98c3-174">O código de autorização, a credencial do cliente e os fluxos em nome do OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="a98c3-174">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="a98c3-175">Para obter mais informações, consulte [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="a98c3-175">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="java"></a>[<span data-ttu-id="a98c3-176">Java</span><span class="sxs-lookup"><span data-stu-id="a98c3-176">Java</span></span>](#tab/Java)

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

# <a name="android"></a>[<span data-ttu-id="a98c3-177">Android</span><span class="sxs-lookup"><span data-stu-id="a98c3-177">Android</span></span>](#tab/Android)

<span data-ttu-id="a98c3-178">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-178">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="a98c3-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a98c3-179">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a98c3-180">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-180">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="a98c3-181">PHP</span><span class="sxs-lookup"><span data-stu-id="a98c3-181">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a98c3-182">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-182">Not available, yet.</span></span> <span data-ttu-id="a98c3-183">Dê suporte ou abra uma solicitação [de recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-183">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="a98c3-184">Ruby</span><span class="sxs-lookup"><span data-stu-id="a98c3-184">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a98c3-185">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-185">Not available, yet.</span></span> <span data-ttu-id="a98c3-186">Dê suporte ou abra uma solicitação [de recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-186">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a><span data-ttu-id="a98c3-187">Provedor on-behalf-of</span><span class="sxs-lookup"><span data-stu-id="a98c3-187">On-behalf-of provider</span></span>

<span data-ttu-id="a98c3-188">O fluxo em nome do fluxo é aplicável quando seu aplicativo chama uma API de serviço/web que, por sua vez, chama a API Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a98c3-188">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="a98c3-189">Saiba mais lendo [o plataforma de identidade da Microsoft e o fluxo OAuth 2.0 On-Behalf-Of](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="a98c3-189">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="c"></a>[<span data-ttu-id="a98c3-190">C#</span><span class="sxs-lookup"><span data-stu-id="a98c3-190">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="a98c3-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="a98c3-191">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a98c3-192">O código de autorização, a credencial do cliente e os fluxos em nome do OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="a98c3-192">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="a98c3-193">Leia [Usando o Provedor de Autenticação Personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="a98c3-193">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="java"></a>[<span data-ttu-id="a98c3-194">Java</span><span class="sxs-lookup"><span data-stu-id="a98c3-194">Java</span></span>](#tab/Java)

<span data-ttu-id="a98c3-195">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-195">Not yet available.</span></span> <span data-ttu-id="a98c3-196">Vote ou abra uma solicitação de [recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-196">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="android"></a>[<span data-ttu-id="a98c3-197">Android</span><span class="sxs-lookup"><span data-stu-id="a98c3-197">Android</span></span>](#tab/Android)

<span data-ttu-id="a98c3-198">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-198">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="a98c3-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a98c3-199">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a98c3-200">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-200">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="a98c3-201">PHP</span><span class="sxs-lookup"><span data-stu-id="a98c3-201">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a98c3-202">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-202">Not yet available.</span></span> <span data-ttu-id="a98c3-203">Vote ou abra uma solicitação de [recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-203">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="a98c3-204">Ruby</span><span class="sxs-lookup"><span data-stu-id="a98c3-204">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a98c3-205">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-205">Not yet available.</span></span> <span data-ttu-id="a98c3-206">Vote ou abra uma solicitação de [recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-206">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a><span data-ttu-id="a98c3-207">Provedor implícito</span><span class="sxs-lookup"><span data-stu-id="a98c3-207">Implicit provider</span></span>

<span data-ttu-id="a98c3-208">O fluxo de concessão implícito é usado em aplicativos baseados em navegador.</span><span class="sxs-lookup"><span data-stu-id="a98c3-208">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="a98c3-209">Para obter mais informações, [consulte plataforma de identidade da Microsoft fluxo de concessão implícito.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)</span><span class="sxs-lookup"><span data-stu-id="a98c3-209">For more information, see [Microsoft identity platform and Implicit grant flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="c"></a>[<span data-ttu-id="a98c3-210">C#</span><span class="sxs-lookup"><span data-stu-id="a98c3-210">C#</span></span>](#tab/CS)

<span data-ttu-id="a98c3-211">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-211">Not applicable.</span></span>

# <a name="javascript"></a>[<span data-ttu-id="a98c3-212">Javascript</span><span class="sxs-lookup"><span data-stu-id="a98c3-212">Javascript</span></span>](#tab/Javascript)

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

# <a name="java"></a>[<span data-ttu-id="a98c3-213">Java</span><span class="sxs-lookup"><span data-stu-id="a98c3-213">Java</span></span>](#tab/Java)

<span data-ttu-id="a98c3-214">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-214">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="a98c3-215">Android</span><span class="sxs-lookup"><span data-stu-id="a98c3-215">Android</span></span>](#tab/Android)

<span data-ttu-id="a98c3-216">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-216">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="a98c3-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a98c3-217">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a98c3-218">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-218">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="a98c3-219">PHP</span><span class="sxs-lookup"><span data-stu-id="a98c3-219">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a98c3-220">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-220">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="a98c3-221">Ruby</span><span class="sxs-lookup"><span data-stu-id="a98c3-221">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a98c3-222">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-222">Not applicable.</span></span>

---

##  <a name="device-code-provider"></a><a name="DeviceCodeProvider"></a><span data-ttu-id="a98c3-223">Provedor de código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="a98c3-223">Device code provider</span></span>

<span data-ttu-id="a98c3-224">O fluxo de código do dispositivo permite entrar em dispositivos por meio de outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a98c3-224">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="a98c3-225">Para obter detalhes, consulte plataforma de identidade da Microsoft e o fluxo de código do dispositivo [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-device-code)</span><span class="sxs-lookup"><span data-stu-id="a98c3-225">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="c"></a>[<span data-ttu-id="a98c3-226">C#</span><span class="sxs-lookup"><span data-stu-id="a98c3-226">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[<span data-ttu-id="a98c3-227">Javascript</span><span class="sxs-lookup"><span data-stu-id="a98c3-227">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a98c3-228">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-228">Not yet available.</span></span> <span data-ttu-id="a98c3-229">Vote ou abra uma solicitação de [recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-229">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="a98c3-230">Java</span><span class="sxs-lookup"><span data-stu-id="a98c3-230">Java</span></span>](#tab/Java)

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

# <a name="android"></a>[<span data-ttu-id="a98c3-231">Android</span><span class="sxs-lookup"><span data-stu-id="a98c3-231">Android</span></span>](#tab/Android)

<span data-ttu-id="a98c3-232">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-232">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="a98c3-233">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a98c3-233">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a98c3-234">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-234">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="a98c3-235">PHP</span><span class="sxs-lookup"><span data-stu-id="a98c3-235">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a98c3-236">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-236">Not yet available.</span></span> <span data-ttu-id="a98c3-237">Vote ou abra uma solicitação de [recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-237">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="a98c3-238">Ruby</span><span class="sxs-lookup"><span data-stu-id="a98c3-238">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a98c3-239">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-239">Not yet available.</span></span> <span data-ttu-id="a98c3-240">Vote ou abra uma solicitação de [recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-240">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a><span data-ttu-id="a98c3-241">Provedor Windows integrado</span><span class="sxs-lookup"><span data-stu-id="a98c3-241">Integrated Windows provider</span></span>

<span data-ttu-id="a98c3-242">O fluxo Windows integrado fornece uma maneira de Windows computadores adquirirem silenciosamente um token de acesso quando eles estão ingressados no domínio.</span><span class="sxs-lookup"><span data-stu-id="a98c3-242">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="a98c3-243">Para obter detalhes, consulte [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span><span class="sxs-lookup"><span data-stu-id="a98c3-243">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="c"></a>[<span data-ttu-id="a98c3-244">C#</span><span class="sxs-lookup"><span data-stu-id="a98c3-244">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="a98c3-245">Javascript</span><span class="sxs-lookup"><span data-stu-id="a98c3-245">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a98c3-246">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-246">Not applicable.</span></span>

# <a name="java"></a>[<span data-ttu-id="a98c3-247">Java</span><span class="sxs-lookup"><span data-stu-id="a98c3-247">Java</span></span>](#tab/Java)

<span data-ttu-id="a98c3-248">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-248">Not applicable.</span></span>

# <a name="android"></a>[<span data-ttu-id="a98c3-249">Android</span><span class="sxs-lookup"><span data-stu-id="a98c3-249">Android</span></span>](#tab/Android)

<span data-ttu-id="a98c3-250">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-250">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="a98c3-251">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a98c3-251">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a98c3-252">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-252">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="a98c3-253">PHP</span><span class="sxs-lookup"><span data-stu-id="a98c3-253">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a98c3-254">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-254">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="a98c3-255">Ruby</span><span class="sxs-lookup"><span data-stu-id="a98c3-255">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a98c3-256">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-256">Not applicable.</span></span>

---

##  <a name="interactive-provider"></a><a name="InteractiveProvider"></a><span data-ttu-id="a98c3-257">Provedor interativo</span><span class="sxs-lookup"><span data-stu-id="a98c3-257">Interactive provider</span></span>

<span data-ttu-id="a98c3-258">O fluxo interativo é usado por aplicativos móveis (Xamarin e UWP) e aplicativos de área de trabalho para chamar a Microsoft Graph em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a98c3-258">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="a98c3-259">Para obter detalhes, consulte [Adquirindo tokens interativamente](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span><span class="sxs-lookup"><span data-stu-id="a98c3-259">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="c"></a>[<span data-ttu-id="a98c3-260">C#</span><span class="sxs-lookup"><span data-stu-id="a98c3-260">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[<span data-ttu-id="a98c3-261">Javascript</span><span class="sxs-lookup"><span data-stu-id="a98c3-261">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a98c3-262">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-262">Not yet available.</span></span> <span data-ttu-id="a98c3-263">Vote ou abra uma solicitação de [recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-263">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="a98c3-264">Java</span><span class="sxs-lookup"><span data-stu-id="a98c3-264">Java</span></span>](#tab/Java)

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

# <a name="android"></a>[<span data-ttu-id="a98c3-265">Android</span><span class="sxs-lookup"><span data-stu-id="a98c3-265">Android</span></span>](#tab/Android)

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

# <a name="objective-c"></a>[<span data-ttu-id="a98c3-266">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a98c3-266">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[<span data-ttu-id="a98c3-267">PHP</span><span class="sxs-lookup"><span data-stu-id="a98c3-267">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a98c3-268">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-268">Not applicable.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="a98c3-269">Ruby</span><span class="sxs-lookup"><span data-stu-id="a98c3-269">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a98c3-270">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-270">Not applicable.</span></span>

---

##  <a name="usernamepassword-provider"></a><a name="UsernamePasswordProvider"></a><span data-ttu-id="a98c3-271">Provedor de nome de usuário/senha</span><span class="sxs-lookup"><span data-stu-id="a98c3-271">Username/password provider</span></span>

<span data-ttu-id="a98c3-272">O provedor de nome de usuário/senha permite que um aplicativo entre em um usuário usando seu nome de usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="a98c3-272">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="a98c3-273">Use esse fluxo somente quando você não puder usar nenhum dos outros fluxos OAuth.</span><span class="sxs-lookup"><span data-stu-id="a98c3-273">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="a98c3-274">Para obter mais informações, consulte plataforma de identidade da Microsoft e a credencial de senha do proprietário do recurso [OAuth 2.0](/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="a98c3-274">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="c"></a>[<span data-ttu-id="a98c3-275">C#</span><span class="sxs-lookup"><span data-stu-id="a98c3-275">C#</span></span>](#tab/CS)

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

# <a name="javascript"></a>[<span data-ttu-id="a98c3-276">Javascript</span><span class="sxs-lookup"><span data-stu-id="a98c3-276">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a98c3-277">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-277">Not yet available.</span></span> <span data-ttu-id="a98c3-278">Vote ou abra uma solicitação de [recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-278">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="java"></a>[<span data-ttu-id="a98c3-279">Java</span><span class="sxs-lookup"><span data-stu-id="a98c3-279">Java</span></span>](#tab/Java)

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

# <a name="android"></a>[<span data-ttu-id="a98c3-280">Android</span><span class="sxs-lookup"><span data-stu-id="a98c3-280">Android</span></span>](#tab/Android)

<span data-ttu-id="a98c3-281">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-281">Not applicable.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="a98c3-282">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a98c3-282">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a98c3-283">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a98c3-283">Not applicable.</span></span>

# <a name="php"></a>[<span data-ttu-id="a98c3-284">PHP</span><span class="sxs-lookup"><span data-stu-id="a98c3-284">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a98c3-285">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-285">Not yet available.</span></span> <span data-ttu-id="a98c3-286">Vote ou abra uma solicitação de [recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-286">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="ruby"></a>[<span data-ttu-id="a98c3-287">Ruby</span><span class="sxs-lookup"><span data-stu-id="a98c3-287">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a98c3-288">Ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="a98c3-288">Not yet available.</span></span> <span data-ttu-id="a98c3-289">Vote ou abra uma solicitação de [recurso Graph microsoft](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a98c3-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="a98c3-290">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a98c3-290">Next steps</span></span>

* <span data-ttu-id="a98c3-291">Para obter exemplos de código que mostram como usar o plataforma de identidade da Microsoft para proteger diferentes tipos de aplicativos, consulte plataforma de identidade da Microsoft exemplos de código (ponto de extremidade [v2.0)](/azure/active-directory/develop/sample-v2-code).</span><span class="sxs-lookup"><span data-stu-id="a98c3-291">For code samples that show you how to use the Microsoft identity platform to secure different application types, see [Microsoft identity platform code samples (v2.0 endpoint)](/azure/active-directory/develop/sample-v2-code).</span></span>
* <span data-ttu-id="a98c3-292">Os provedores de autenticação exigem uma ID do cliente.</span><span class="sxs-lookup"><span data-stu-id="a98c3-292">Authentication providers require an client ID.</span></span> <span data-ttu-id="a98c3-293">Você vai querer registrar [seu aplicativo depois](https://portal.azure.com/) de configurar seu provedor de autenticação.</span><span class="sxs-lookup"><span data-stu-id="a98c3-293">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="a98c3-294">Deixe-nos saber se um fluxo OAuth necessário não tem suporte no momento votando ou abrindo uma solicitação de recurso do [Microsoft Graph](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span><span class="sxs-lookup"><span data-stu-id="a98c3-294">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span></span>
