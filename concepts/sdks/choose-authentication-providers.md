---
title: Escolher um provedor de autenticação do Microsoft Graph
description: Saiba como escolher provedores de autenticação específicos do cenário para seu aplicativo.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 5061b38249f31a6eea959ecec94899337bf57326
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630192"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-oauth-flow"></a><span data-ttu-id="a591b-103">Escolher um provedor de autenticação do Microsoft Graph com base no fluxo OAuth</span><span class="sxs-lookup"><span data-stu-id="a591b-103">Choose a Microsoft Graph authentication provider based on OAuth flow</span></span>

<span data-ttu-id="a591b-104">Os provedores de autenticação simplificam a obter um token de acesso, abstraindo os parâmetros exigidos pelas bibliotecas de clientes de autenticação.</span><span class="sxs-lookup"><span data-stu-id="a591b-104">Authentication providers simplify getting an access token by abstracting the parameters required by the authentication client libraries.</span></span> <span data-ttu-id="a591b-105">Os provedores de autenticação do Microsoft Graph simplificam o uso da biblioteca de autenticação da Microsoft (MSAL) fornecendo adaptadores para cada plataforma.</span><span class="sxs-lookup"><span data-stu-id="a591b-105">The Microsoft Graph authentication providers simplify the use of the Microsoft Authentication Library (MSAL) by providing adapters for each platform.</span></span> <span data-ttu-id="a591b-106">Esses adaptadores tratam da aquisição de token para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a591b-106">These adapters handle token acquisition for your application.</span></span> <span data-ttu-id="a591b-107">Os provedores de autenticação do Microsoft Graph mapeiam para um fluxo de concessão OAuth.</span><span class="sxs-lookup"><span data-stu-id="a591b-107">The Microsoft Graph authentication providers map to an OAuth grant flow.</span></span> <span data-ttu-id="a591b-108">Você precisará saber qual fluxo de concessão OAuth usar para seu aplicativo para selecionar o provedor de autenticação apropriado para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a591b-108">You'll need to know which OAuth grant flow to use for your application in order to select the appropriate authentication provider for your application.</span></span>

## <a name="authorization-code-oauth-flow"></a><span data-ttu-id="a591b-109">Fluxo OAuth de código de autorização</span><span class="sxs-lookup"><span data-stu-id="a591b-109">Authorization code OAuth flow</span></span>

<span data-ttu-id="a591b-110">O fluxo de código de autorização permite que aplicativos nativos e Web obtenham tokens com segurança no nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="a591b-110">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="a591b-111">Para saber mais, confira [Microsoft Identity Platform and OAuth 2,0 Authorization Code Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span><span class="sxs-lookup"><span data-stu-id="a591b-111">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="a591b-112">Basic</span><span class="sxs-lookup"><span data-stu-id="a591b-112">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = AuthorizationCodeProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a591b-113">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a591b-113">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a591b-114">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="a591b-114">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="a591b-115">Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="a591b-115">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="a591b-116">Java</span><span class="sxs-lookup"><span data-stu-id="a591b-116">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="a591b-117">Android</span><span class="sxs-lookup"><span data-stu-id="a591b-117">Android</span></span>](#tab/Android)

<span data-ttu-id="a591b-118">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-118">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a591b-119">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a591b-119">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a591b-120">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-120">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="a591b-121">PHP</span><span class="sxs-lookup"><span data-stu-id="a591b-121">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a591b-122">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-122">Not yet available.</span></span> <span data-ttu-id="a591b-123">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-123">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="a591b-124">Ruby</span><span class="sxs-lookup"><span data-stu-id="a591b-124">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a591b-125">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="a591b-125">Not available, yet.</span></span> <span data-ttu-id="a591b-126">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-126">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="client-credential-oauth-flow"></a><span data-ttu-id="a591b-127">Fluxo OAuth de credenciais do cliente</span><span class="sxs-lookup"><span data-stu-id="a591b-127">Client credential OAuth flow</span></span>

<span data-ttu-id="a591b-128">O fluxo de credenciais do cliente permite que aplicativos de serviço sejam executados sem interação do usuário.</span><span class="sxs-lookup"><span data-stu-id="a591b-128">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="a591b-129">O acesso baseia-se na identidade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a591b-129">Access is based on the identity of the application.</span></span> <span data-ttu-id="a591b-130">Para obter mais informações, consulte [Microsoft Identity Platform e The OAuth 2,0 Client Credentials Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="a591b-130">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="a591b-131">Basic</span><span class="sxs-lookup"><span data-stu-id="a591b-131">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = ClientCredentialProvider.CreateClientApplication(clientId, clientCredential);
ClientCredentialProvider authProvider = new ClientCredentialProvider(clientApplication);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a591b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a591b-132">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a591b-133">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="a591b-133">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="a591b-134">Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span><span class="sxs-lookup"><span data-stu-id="a591b-134">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="a591b-135">Java</span><span class="sxs-lookup"><span data-stu-id="a591b-135">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="a591b-136">Android</span><span class="sxs-lookup"><span data-stu-id="a591b-136">Android</span></span>](#tab/Android)

<span data-ttu-id="a591b-137">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-137">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a591b-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a591b-138">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a591b-139">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-139">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="a591b-140">PHP</span><span class="sxs-lookup"><span data-stu-id="a591b-140">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a591b-141">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="a591b-141">Not available, yet.</span></span> <span data-ttu-id="a591b-142">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-142">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="a591b-143">Ruby</span><span class="sxs-lookup"><span data-stu-id="a591b-143">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a591b-144">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="a591b-144">Not available, yet.</span></span> <span data-ttu-id="a591b-145">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-145">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="on-behalf-of-oauth-flow"></a><span data-ttu-id="a591b-146">Fluxo de OAuth em nome de</span><span class="sxs-lookup"><span data-stu-id="a591b-146">On-behalf-of OAuth flow</span></span>

<span data-ttu-id="a591b-147">O fluxo em nome de é aplicável quando o aplicativo chama uma API de serviço/Web que, em seguida, chama a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a591b-147">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="a591b-148">Saiba mais lendo a [plataforma de identidade da Microsoft e o fluxo em nome de do OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span><span class="sxs-lookup"><span data-stu-id="a591b-148">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="a591b-149">Basic</span><span class="sxs-lookup"><span data-stu-id="a591b-149">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = OnBehalfOfProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
OnBehalfOfProvider authProvider = new OnBehalfOfProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a591b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a591b-150">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a591b-151">O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento.</span><span class="sxs-lookup"><span data-stu-id="a591b-151">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="a591b-152">Leia [usando provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="a591b-152">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="a591b-153">Java</span><span class="sxs-lookup"><span data-stu-id="a591b-153">Java</span></span>](#tab/Java)

<span data-ttu-id="a591b-154">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-154">Not yet available.</span></span> <span data-ttu-id="a591b-155">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-155">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="a591b-156">Android</span><span class="sxs-lookup"><span data-stu-id="a591b-156">Android</span></span>](#tab/Android)

<span data-ttu-id="a591b-157">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-157">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a591b-158">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a591b-158">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a591b-159">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-159">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="a591b-160">PHP</span><span class="sxs-lookup"><span data-stu-id="a591b-160">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a591b-161">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-161">Not yet available.</span></span> <span data-ttu-id="a591b-162">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-162">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="a591b-163">Ruby</span><span class="sxs-lookup"><span data-stu-id="a591b-163">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a591b-164">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-164">Not yet available.</span></span> <span data-ttu-id="a591b-165">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-165">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-grant-oauth-flow"></a><span data-ttu-id="a591b-166">Fluxo de concessão OAuth implícito</span><span class="sxs-lookup"><span data-stu-id="a591b-166">Implicit grant OAuth flow</span></span>

<span data-ttu-id="a591b-167">O fluxo de concessão implícito é usado em aplicativos baseados em navegador.</span><span class="sxs-lookup"><span data-stu-id="a591b-167">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="a591b-168">Para obter mais informações, consulte [Microsoft Identity Platform and implícito Grant Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="a591b-168">For more information, see [Microsoft identity platform and Implicit grant flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="a591b-169">Basic</span><span class="sxs-lookup"><span data-stu-id="a591b-169">C#</span></span>](#tab/CS)

<span data-ttu-id="a591b-170">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-170">Not applicable.</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a591b-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a591b-171">Javascript</span></span>](#tab/Javascript)

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

# <a name="javatabjava"></a>[<span data-ttu-id="a591b-172">Java</span><span class="sxs-lookup"><span data-stu-id="a591b-172">Java</span></span>](#tab/Java)

<span data-ttu-id="a591b-173">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-173">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="a591b-174">Android</span><span class="sxs-lookup"><span data-stu-id="a591b-174">Android</span></span>](#tab/Android)

<span data-ttu-id="a591b-175">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-175">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a591b-176">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a591b-176">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a591b-177">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-177">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="a591b-178">PHP</span><span class="sxs-lookup"><span data-stu-id="a591b-178">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a591b-179">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-179">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="a591b-180">Ruby</span><span class="sxs-lookup"><span data-stu-id="a591b-180">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a591b-181">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-181">Not applicable.</span></span>

---

## <a name="device-code-oauth-flow"></a><span data-ttu-id="a591b-182">Fluxo OAuth de código de dispositivo</span><span class="sxs-lookup"><span data-stu-id="a591b-182">Device code OAuth flow</span></span>

<span data-ttu-id="a591b-183">O fluxo de código de dispositivo permite entrar em dispositivos por meio de outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a591b-183">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="a591b-184">Para obter detalhes, consulte [plataforma de identidade da Microsoft e o fluxo de código de dispositivo OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span><span class="sxs-lookup"><span data-stu-id="a591b-184">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="a591b-185">Basic</span><span class="sxs-lookup"><span data-stu-id="a591b-185">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = DeviceCodeProvider.CreateClientApplication(clientId);
DeviceCodeProvider authProvider = new DeviceCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a591b-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a591b-186">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a591b-187">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-187">Not yet available.</span></span> <span data-ttu-id="a591b-188">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-188">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="a591b-189">Java</span><span class="sxs-lookup"><span data-stu-id="a591b-189">Java</span></span>](#tab/Java)

<span data-ttu-id="a591b-190">Não disponível, ainda.</span><span class="sxs-lookup"><span data-stu-id="a591b-190">Not available, yet.</span></span> <span data-ttu-id="a591b-191">Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-191">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="a591b-192">Android</span><span class="sxs-lookup"><span data-stu-id="a591b-192">Android</span></span>](#tab/Android)

<span data-ttu-id="a591b-193">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-193">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a591b-194">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a591b-194">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a591b-195">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-195">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="a591b-196">PHP</span><span class="sxs-lookup"><span data-stu-id="a591b-196">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a591b-197">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-197">Not yet available.</span></span> <span data-ttu-id="a591b-198">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-198">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="a591b-199">Ruby</span><span class="sxs-lookup"><span data-stu-id="a591b-199">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a591b-200">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-200">Not yet available.</span></span> <span data-ttu-id="a591b-201">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-201">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="integrated-windows-flow"></a><span data-ttu-id="a591b-202">Fluxo integrado do Windows</span><span class="sxs-lookup"><span data-stu-id="a591b-202">Integrated Windows flow</span></span>

<span data-ttu-id="a591b-203">O fluxo integrado do Windows oferece uma maneira para que os computadores com Windows adquiram um token de acesso de forma silenciosa quando são associados ao domínio.</span><span class="sxs-lookup"><span data-stu-id="a591b-203">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="a591b-204">Para obter detalhes, consulte [autenticação integrada do Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span><span class="sxs-lookup"><span data-stu-id="a591b-204">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="a591b-205">Basic</span><span class="sxs-lookup"><span data-stu-id="a591b-205">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = IntegratedWindowsAuthenticationProvider.CreateClientApplication(clientId);
IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a591b-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a591b-206">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a591b-207">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-207">Not applicable.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="a591b-208">Java</span><span class="sxs-lookup"><span data-stu-id="a591b-208">Java</span></span>](#tab/Java)

<span data-ttu-id="a591b-209">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-209">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="a591b-210">Android</span><span class="sxs-lookup"><span data-stu-id="a591b-210">Android</span></span>](#tab/Android)

<span data-ttu-id="a591b-211">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-211">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a591b-212">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a591b-212">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a591b-213">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-213">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="a591b-214">PHP</span><span class="sxs-lookup"><span data-stu-id="a591b-214">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a591b-215">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-215">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="a591b-216">Ruby</span><span class="sxs-lookup"><span data-stu-id="a591b-216">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a591b-217">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-217">Not applicable.</span></span>

---

## <a name="interactive-flow"></a><span data-ttu-id="a591b-218">Fluxo interativo</span><span class="sxs-lookup"><span data-stu-id="a591b-218">Interactive flow</span></span>

<span data-ttu-id="a591b-219">O fluxo interativo é usado por aplicativos móveis (Xamarin e UWP) e aplicativos de área de trabalho para chamar o Microsoft Graph no nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a591b-219">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="a591b-220">Para obter detalhes, [](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)consulte adquirindo tokens interativamente.</span><span class="sxs-lookup"><span data-stu-id="a591b-220">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="a591b-221">Basic</span><span class="sxs-lookup"><span data-stu-id="a591b-221">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = InteractiveAuthenticationProvider.CreateClientApplication(clientId);
InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a591b-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a591b-222">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a591b-223">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-223">Not yet available.</span></span> <span data-ttu-id="a591b-224">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-224">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="a591b-225">Java</span><span class="sxs-lookup"><span data-stu-id="a591b-225">Java</span></span>](#tab/Java)

<span data-ttu-id="a591b-226">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-226">Not yet available.</span></span> <span data-ttu-id="a591b-227">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-227">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="a591b-228">Android</span><span class="sxs-lookup"><span data-stu-id="a591b-228">Android</span></span>](#tab/Android)

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

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a591b-229">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a591b-229">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[<span data-ttu-id="a591b-230">PHP</span><span class="sxs-lookup"><span data-stu-id="a591b-230">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a591b-231">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-231">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="a591b-232">Ruby</span><span class="sxs-lookup"><span data-stu-id="a591b-232">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a591b-233">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-233">Not applicable.</span></span>

---

## <a name="resource-owner-password-credential-grant-oauth-flow"></a><span data-ttu-id="a591b-234">Credencial do proprietário do recurso conceder fluxo OAuth</span><span class="sxs-lookup"><span data-stu-id="a591b-234">Resource owner password credential grant OAuth flow</span></span>

<span data-ttu-id="a591b-235">O fluxo de credenciais da senha do proprietário do recurso permite que um aplicativo entre em um usuário usando seu nome de usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="a591b-235">The resource owner password credential flow allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="a591b-236">Use este fluxo somente quando não for possível usar qualquer um dos outros fluxos OAuth.</span><span class="sxs-lookup"><span data-stu-id="a591b-236">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="a591b-237">Para obter mais informações, consulte [plataforma de identidade da Microsoft e a credencial de senha de proprietário do recurso OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span><span class="sxs-lookup"><span data-stu-id="a591b-237">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="ctabcs"></a>[<span data-ttu-id="a591b-238">Basic</span><span class="sxs-lookup"><span data-stu-id="a591b-238">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = UsernamePasswordProvider.CreateClientApplication(clientId);
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a591b-239">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a591b-239">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="a591b-240">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-240">Not yet available.</span></span> <span data-ttu-id="a591b-241">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="a591b-242">Java</span><span class="sxs-lookup"><span data-stu-id="a591b-242">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="a591b-243">Android</span><span class="sxs-lookup"><span data-stu-id="a591b-243">Android</span></span>](#tab/Android)

<span data-ttu-id="a591b-244">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-244">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a591b-245">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a591b-245">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="a591b-246">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="a591b-246">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="a591b-247">PHP</span><span class="sxs-lookup"><span data-stu-id="a591b-247">PHP</span></span>](#tab/PHP)

<span data-ttu-id="a591b-248">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-248">Not yet available.</span></span> <span data-ttu-id="a591b-249">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-249">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="a591b-250">Ruby</span><span class="sxs-lookup"><span data-stu-id="a591b-250">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="a591b-251">Ainda não disponível.</span><span class="sxs-lookup"><span data-stu-id="a591b-251">Not yet available.</span></span> <span data-ttu-id="a591b-252">Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.</span><span class="sxs-lookup"><span data-stu-id="a591b-252">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="a591b-253">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a591b-253">Next steps</span></span>

* <span data-ttu-id="a591b-254">Os provedores de autenticação exigem uma ID de cliente.</span><span class="sxs-lookup"><span data-stu-id="a591b-254">Authentication providers require an client ID.</span></span> <span data-ttu-id="a591b-255">Você deve [registrar seu aplicativo](https://portal.azure.com/) depois de configurar seu provedor de autenticação.</span><span class="sxs-lookup"><span data-stu-id="a591b-255">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="a591b-256">Deixe-nos saber se um fluxo OAuth necessário atualmente não é suportado pela votação ou pela abertura de uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span><span class="sxs-lookup"><span data-stu-id="a591b-256">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>