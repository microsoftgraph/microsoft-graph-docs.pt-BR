---
title: Escolha um provedor de autenticação Graph microsoft
description: Saiba como escolher provedores de autenticação específicos de cenário para seu aplicativo.
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 607759b11f1554a91cd169efe7fb56e17862354b
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220567"
---
<!-- markdownlint-disable MD001 MD024 MD025 -->

# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a>Escolher um provedor de autenticação do Microsoft Graph com base no cenário

Os provedores de autenticação implementam o código necessário para adquirir um token usando a Biblioteca de Autenticação da Microsoft (MSAL); lidar com vários erros potenciais para casos como consentimento incremental, senhas expiradas e acesso condicional; e, em seguida, de definir o cabeçalho de autorização de solicitação HTTP. A tabela a seguir lista o conjunto de provedores que combinam com os cenários de diferentes tipos [de aplicativo.](/azure/active-directory/develop/v2-app-types)

| Cenário                                                                                               | Flow/Grant         | Espectadores               | Provedor |
|--------------------------------------------------------------------------------------------------------|--------------------|------------------------|-----|
| [Aplicativo de Página Única](/azure/active-directory/develop/scenario-spa-acquire-token)                          | Código de Autorização |                        |     |
|                                                                                                        | com PKCE          | Consumidor Delegado/Org | [Provedor de código de autorização](#authorization-code-provider) |
| [Aplicativo Web que chama APIs da Web](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) |                    |                        |     |
|                                                                                                        | Código de Autorização | Consumidor Delegado/Org | [Provedor de código de autorização](#authorization-code-provider) |
|                                                                                                        | Credenciais do cliente | Somente aplicativo               | [Provedor de credenciais do cliente](#client-credentials-provider) |
| [API Web que chama APIs da Web](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) |                    |                        |     |
|                                                                                                        | Em nome de       | Consumidor Delegado/Org | [Provedor on-behalf-of](#on-behalf-of-provider) |
|                                                                                                        | Credenciais do cliente | Somente aplicativo               | [Provedor de credenciais do cliente](#client-credentials-provider) |
| [Aplicativo de área de trabalho que chama APIs da Web](/azure/active-directory/develop/scenario-desktop-acquire-token)      |                    |                        |     |
|                                                                                                        | Interativo        | Consumidor Delegado/Org | [Provedor interativo](#interactive-provider) |
|                                                                                                        | Integração Windows | Organização Delegada          | [Provedor Windows integrado](#integrated-windows-provider) |
|                                                                                                        | Proprietário do Recurso     | Organização Delegada          | [Provedor de nome de usuário/senha](#usernamepassword-provider) |
|                                                                                                        | Código do dispositivo        | Organização Delegada          | [Provedor de código de dispositivo](#device-code-provider) |
| [Aplicativo Daemon](/azure/active-directory/develop/scenario-daemon-acquire-token)                            |                    |                        |     |
|                                                                                                        | Credenciais do cliente | Somente aplicativo               | [Provedor de credenciais do cliente](#client-credentials-provider) |
| [Aplicativo móvel que chama APIs da Web](/azure/active-directory/develop/scenario-mobile-acquire-token)        |                    |                        |     |
|                                                                                                        | Interativo        | Consumidor Delegado/Org | [Provedor interativo](#interactive-provider) |

> [!NOTE]
> Java e os desenvolvedores do Android precisam adicionar a biblioteca [do azure-identity](/java/api/overview/azure/identity-readme) para obter acesso aos diferentes tipos de credenciais. Os desenvolvedores do .NET precisam adicionar o [pacote do Azure.Identity](/dotnet/api/azure.identity) para obter acesso aos diferentes tipos de credenciais.

## <a name="authorization-code-provider"></a>Provedor de código de autorização

O fluxo de código de autorização permite que aplicativos nativos e web obtenham tokens com segurança no nome do usuário. Para saber mais, confira plataforma de identidade da Microsoft fluxo de código de autorização [do OAuth 2.0](/azure/active-directory/develop/v2-oauth2-auth-code-flow).

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

// For authorization code flow, the user signs into the Microsoft
// identity platform, and the browser is redirected back to your app
// with an authorization code in the query parameters
var authorizationCode = "AUTH_CODE_FROM_REDIRECT";

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// https://docs.microsoft.com/dotnet/api/azure.identity.authorizationcodecredential
var authCodeCredential = new AuthorizationCodeCredential(
    tenantId, clientId, clientSecret, authorizationCode, options);

var graphClient = new GraphServiceClient(authCodeCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

### <a name="using-azuremsal-browser-for--browser-applications"></a>Usando @azure/msal-browser para aplicativos de navegador

```javascript

const {
    PublicClientApplication,
    InteractionType,
    AccountInfo
} = require("@azure/msal-browser");

const {
    AuthCodeMSALBrowserAuthenticationProvider,
    AuthCodeMSALBrowserAuthenticationProviderOptions
} = require("@microsoft/microsoft-graph-client/authProviders/authCodeMsalBrowser");

const options: AuthCodeMSALBrowserAuthenticationProviderOptions: {
    account: account, // the AccountInfo instance to acquire the token for.
    interactionType: InteractionType.PopUp, // msal-browser InteractionType
    scopes: ["user.read", "mail.send"] // example of the scopes to be passed
}

// Pass the PublicClientApplication instance from step 2 to create AuthCodeMSALBrowserAuthenticationProvider instance
const authProvider: new AuthCodeMSALBrowserAuthenticationProvider(publicClientApplication, options),
```

### <a name="using-azureidentity-for-server-side-applications"></a>Usando @azure/identidade para aplicativos do lado do servidor

```javascript
const {
    Client
} = require("@microsoft/microsoft-graph-client");
const {
    TokenCredentialAuthenticationProvider
} = require("@microsoft/microsoft-graph-client/authProviders/azureTokenCredentials");
const {
    AuthorizationCodeCredential
} = require("@azure/identity");

const credential = new AuthorizationCodeCredential(
    "<YOUR_TENANT_ID>",
    "<YOUR_CLIENT_ID>",
    "<AUTH_CODE_FROM_QUERY_PARAMETERS>",
    "<REDIRECT_URL>"
);
const authProvider = new TokenCredentialAuthenticationProvider(credential, {
    scopes: [scopes]
});

```

# <a name="java"></a>[Java](#tab/Java)

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

# <a name="android"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Não aplicável.

# <a name="php"></a>[PHP](#tab/PHP)

Ainda não está disponível. Dê suporte ou abra uma solicitação [de recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não está disponível. Vote ou abra uma solicitação de [recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

---

## <a name="client-credentials-provider"></a>Provedor de credenciais do cliente

O fluxo de credenciais do cliente permite que aplicativos de serviço executem sem interação do usuário. O Access baseia-se na identidade do aplicativo. Para obter mais informações, consulte plataforma de identidade da Microsoft e o fluxo de credenciais do cliente [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

# <a name="c"></a>[C#](#tab/CS)

### <a name="using-a-client-secret"></a>Usando um segredo do cliente

```csharp
// The client credentials flow requires that you request the
// /.default scope, and preconfigure your permissions on the
// app registration in Azure. An administrator must grant consent
// to those permissions beforehand.
var scopes = new[] { "https://graph.microsoft.com/.default" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// https://docs.microsoft.com/dotnet/api/azure.identity.clientsecretcredential
var clientSecretCredential = new ClientSecretCredential(
    tenantId, clientId, clientSecret, options);

var graphClient = new GraphServiceClient(clientSecretCredential, scopes);
```

### <a name="using-a-client-certificate"></a>Usando um certificado de cliente

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientCertificate = new X509Certificate2("MyCertificate.pfx");

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// https://docs.microsoft.com/dotnet/api/azure.identity.clientcertificatecredential
var clientCertCredential = new ClientCertificateCredential(
    tenantId, clientId, clientCertificate, options);

var graphClient = new GraphServiceClient(clientCertCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

```javascript
const {
    Client
} = require("@microsoft/microsoft-graph-client");
const {
    TokenCredentialAuthenticationProvider
} = require("@microsoft/microsoft-graph-client/authProviders/azureTokenCredentials");
const {
    ClientSecretCredential
} = require("@azure/identity");

const credential = new ClientSecretCredential(tenantId, clientId, clientSecret);
const authProvider = new TokenCredentialAuthenticationProvider(credential, {
    scopes: [scopes]
});

const client = Client.initWithMiddleware({
    debugLogging: true,
    authProvider
    // Use the authProvider object to create the class.
});
```

# <a name="java"></a>[Java](#tab/Java)

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

# <a name="android"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Não aplicável.

# <a name="php"></a>[PHP](#tab/PHP)

Ainda não está disponível. Dê suporte ou abra uma solicitação [de recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não está disponível. Dê suporte ou abra uma solicitação [de recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

---

## <a name="on-behalf-of-provider"></a>Provedor on-behalf-of

O fluxo em nome do fluxo é aplicável quando seu aplicativo chama uma API de serviço/web que, por sua vez, chama a API Graph Microsoft. Saiba mais lendo [o plataforma de identidade da Microsoft e o fluxo OAuth 2.0 On-Behalf-Of](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="c"></a>[C#](#tab/CS)

O pacote não dá suporte ao fluxo em nome `Azure.Identity` da versão 1.4.0. Em vez disso, crie um provedor de autenticação personalizado usando o MSAL.

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// This is the incoming token to exchange using on-behalf-of flow
var oboToken = "JWT_TOKEN_TO_EXCHANGE";

var cca = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantId)
    .WithClientSecret(clientSecret)
    .Build();

// DelegateAuthenticationProvider is a simple auth provider implementation
// that allows you to define an async function to retrieve a token
// Alternatively, you can create a class that implements IAuthenticationProvider
// for more complex scenarios
var authProvider = new DelegateAuthenticationProvider(async (request) => {
    // Use Microsoft.Identity.Client to retrieve token
    var assertion = new UserAssertion(oboToken);
    var result = await cca.AcquireTokenOnBehalfOf(scopes, assertion).ExecuteAsync();

    request.Headers.Authorization =
        new System.Net.Http.Headers.AuthenticationHeaderValue("Bearer", result.AccessToken);
});

var graphClient = new GraphServiceClient(authProvider);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Fluxos OAuth em nome do OAuth exigem que você implemente um provedor de autenticação personalizado no momento. Leia [Usando o Provedor de Autenticação Personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) para obter mais informações.

# <a name="java"></a>[Java](#tab/Java)

Ainda não está disponível. Vote ou abra uma solicitação de [recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

# <a name="android"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Não aplicável.

# <a name="php"></a>[PHP](#tab/PHP)

Ainda não está disponível. Vote ou abra uma solicitação de [recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não está disponível. Vote ou abra uma solicitação de [recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

---

## <a name="implicit-provider"></a>Provedor implícito

O fluxo de autenticação implícito não é recomendado devido às [suas desvantagens.](https://datatracker.ietf.org/doc/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6) Clientes públicos, como aplicativos nativos e aplicativos JavaScript, agora devem usar o fluxo de código de autorização com a extensão PKCE. [Referência](https://oauth.net/2/grant-types/implicit/).

## <a name="device-code-provider"></a>Provedor de código de dispositivo

O fluxo de código do dispositivo permite entrar em dispositivos por meio de outro dispositivo. Para obter detalhes, consulte plataforma de identidade da Microsoft e o fluxo de código do dispositivo [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-device-code)

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// Callback function that receives the user prompt
// Prompt contains the generated device code that use must
// enter during the auth process in the browser
Func<DeviceCodeInfo, CancellationToken, Task> callback = (code, cancellation) => {
    Console.WriteLine(code.Message);
    return Task.FromResult(0);
};

// https://docs.microsoft.com/dotnet/api/azure.identity.devicecodecredential
var deviceCodeCredential = new DeviceCodeCredential(
    callback, tenantId, clientId, options);

var graphClient = new GraphServiceClient(deviceCodeCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

```javascript
const {
    Client
} = require("@microsoft/microsoft-graph-client");
const {
    TokenCredentialAuthenticationProvider
} = require("@microsoft/microsoft-graph-client/authProviders/azureTokenCredentials");
const {
    DeviceCodeCredential
} = require("@azure/identity");

const credential = new DeviceCodeCredential(tenantId, clientId, clientSecret);
const authProvider = new TokenCredentialAuthenticationProvider(credential, {
    scopes: [scopes]
});

const client = Client.initWithMiddleware({
    debugLogging: true,
    authProvider
    // Use the authProvider object to create the class.
});
```

# <a name="java"></a>[Java](#tab/Java)

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

# <a name="android"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Não aplicável.

# <a name="php"></a>[PHP](#tab/PHP)

Ainda não está disponível. Vote ou abra uma solicitação de [recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não está disponível. Vote ou abra uma solicitação de [recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

---

## <a name="integrated-windows-provider"></a>Provedor Windows integrado

O fluxo Windows integrado fornece uma maneira de Windows computadores adquirirem silenciosamente um token de acesso quando eles estão ingressados no domínio. Para obter detalhes, consulte [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).

# <a name="c"></a>[C#](#tab/CS)

No `Azure.Identity` momento, o pacote não dá suporte Windows autenticação integrada. Em vez disso, crie um provedor de autenticação personalizado usando o MSAL.

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

var pca = PublicClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantId)
    .Build();

// DelegateAuthenticationProvider is a simple auth provider implementation
// that allows you to define an async function to retrieve a token
// Alternatively, you can create a class that implements IAuthenticationProvider
// for more complex scenarios
var authProvider = new DelegateAuthenticationProvider(async (request) => {
    // Use Microsoft.Identity.Client to retrieve token
    var result = await pca.AcquireTokenByIntegratedWindowsAuth(scopes).ExecuteAsync();

    request.Headers.Authorization =
        new System.Net.Http.Headers.AuthenticationHeaderValue("Bearer", result.AccessToken);
});

var graphClient = new GraphServiceClient(authProvider);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Não aplicável.

# <a name="java"></a>[Java](#tab/Java)

Não aplicável.

# <a name="android"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Não aplicável.

# <a name="php"></a>[PHP](#tab/PHP)

Não aplicável.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Não aplicável.

---

## <a name="interactive-provider"></a>Provedor interativo

O fluxo interativo é usado por aplicativos móveis (Xamarin e UWP) e aplicativos de área de trabalho para chamar a Microsoft Graph em nome de um usuário. Para obter detalhes, consulte [Adquirindo tokens interativamente](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

var options = new InteractiveBrowserCredentialOptions
{
    TenantId = tenantId,
    ClientId = clientId,
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud,
    // MUST be http://localhost or http://localhost:PORT
    // See https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/System-Browser-on-.Net-Core
    RedirectUri = new Uri("http://localhost"),
};

// https://docs.microsoft.com/dotnet/api/azure.identity.interactivebrowsercredential
var interactiveCredential = new InteractiveBrowserCredential(options);

var graphClient = new GraphServiceClient(interactiveCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Ainda não está disponível. Vote ou abra uma solicitação de [recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

# <a name="java"></a>[Java](#tab/Java)

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

# <a name="android"></a>[Android](#tab/Android)

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

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[PHP](#tab/PHP)

Não aplicável.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Não aplicável.

---

## <a name="usernamepassword-provider"></a>Provedor de nome de usuário/senha

O provedor de nome de usuário/senha permite que um aplicativo entre em um usuário usando seu nome de usuário e senha. Use esse fluxo somente quando você não puder usar nenhum dos outros fluxos OAuth. Para obter mais informações, consulte plataforma de identidade da Microsoft e a credencial de senha do proprietário do recurso [OAuth 2.0](/azure/active-directory/develop/v2-oauth-ropc)

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

var userName = "adelev@contoso.com";
var password = "P@ssword1!";

var userNamePasswordCredential = new UsernamePasswordCredential(
    userName, password, tenantId, clientId, options);

var graphClient = new GraphServiceClient(userNamePasswordCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Ainda não está disponível. Vote ou abra uma solicitação de [recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

# <a name="java"></a>[Java](#tab/Java)

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

# <a name="android"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Não aplicável.

# <a name="php"></a>[PHP](#tab/PHP)

Ainda não está disponível. Vote ou abra uma solicitação de [recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não está disponível. Vote ou abra uma solicitação de [recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

---

## <a name="next-steps"></a>Próximas etapas

* Para obter exemplos de código que mostram como usar o plataforma de identidade da Microsoft para proteger diferentes tipos de aplicativos, consulte plataforma de identidade da Microsoft exemplos de código (ponto de extremidade [v2.0)](/azure/active-directory/develop/sample-v2-code).
* Os provedores de autenticação exigem uma ID do cliente. Você vai querer registrar [seu aplicativo depois](https://portal.azure.com/) de configurar seu provedor de autenticação.
* Deixe-nos saber se um fluxo OAuth necessário não tem suporte no momento votando ou abrindo uma solicitação de recurso do [Microsoft Graph](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
