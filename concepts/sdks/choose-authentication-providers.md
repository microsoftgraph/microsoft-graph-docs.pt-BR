---
title: Escolher um provedor de autenticação Graph Microsoft
description: Saiba como escolher provedores de autenticação específicos do cenário para seu aplicativo.
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 040a42ae20ee48d5af92dd4460b2e26b059ffea7
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733241"
---
<!-- markdownlint-disable MD001 MD024 MD025 -->

# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a>Escolher um provedor de autenticação do Microsoft Graph com base no cenário

Os provedores de autenticação implementam o código necessário para adquirir um token usando a MSAL (Biblioteca de Autenticação da Microsoft); tratar vários erros potenciais para casos como consentimento incremental, senhas expiradas e acesso condicional; e, em seguida, defina o cabeçalho de autorização de solicitação HTTP. A tabela a seguir lista o conjunto de provedores que correspondem aos cenários de diferentes tipos [de aplicativo](/azure/active-directory/develop/v2-app-types).

| Cenário                                                                                               | Flow/Conceder         | Espectadores               | Provedor |
|--------------------------------------------------------------------------------------------------------|--------------------|------------------------|-----|
| [Aplicativo de Página Única](/azure/active-directory/develop/scenario-spa-acquire-token)                          | Código de autorização com PKCE | Consumidor delegado/organização | [Provedor de código de autorização](#authorization-code-provider) |
| [Aplicativo Web que chama APIs Web](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) |                    |                        |     |
|                                                                                                        | Código de Autorização | Consumidor delegado/organização | [Provedor de código de autorização](#authorization-code-provider) |
|                                                                                                        | Credenciais do cliente | Somente aplicativo               | [Provedor de credenciais do cliente](#client-credentials-provider) |
| [API Web que chama APIs Web](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) |                    |                        |     |
|                                                                                                        | Em nome de       | Consumidor delegado/organização | [Provedor em nome de](#on-behalf-of-provider) |
|                                                                                                        | Credenciais do cliente | Somente aplicativo               | [Provedor de credenciais do cliente](#client-credentials-provider) |
| [Aplicativo da área de trabalho que chama APIs Web](/azure/active-directory/develop/scenario-desktop-acquire-token)      |                    |                        |     |
|                                                                                                        | Interativo        | Consumidor delegado/organização | [Provedor interativo](#interactive-provider) |
|                                                                                                        | Integração Windows | Organização Delegada          | [Provedor Windows integrado](#integrated-windows-provider) |
|                                                                                                        | Proprietário do Recurso     | Organização Delegada          | [Provedor de nome de usuário/senha](#usernamepassword-provider) |
|                                                                                                        | Código do dispositivo        | Organização Delegada          | [Provedor de código do dispositivo](#device-code-provider) |
| [Aplicativo Daemon](/azure/active-directory/develop/scenario-daemon-acquire-token)                            |                    |                        |     |
|                                                                                                        | Credenciais do cliente | Somente aplicativo               | [Provedor de credenciais do cliente](#client-credentials-provider) |
| [Aplicativo móvel que chama APIs Web](/azure/active-directory/develop/scenario-mobile-acquire-token)        |                    |                        |     |
|                                                                                                        | Interativo        | Consumidor delegado/organização | [Provedor interativo](#interactive-provider) |

> [!NOTE]
> Os snippets de código a seguir foram escritos com as versões mais recentes de seus respectivos SDKs. Se você encontrar erros do compilador com esses snippets, verifique se você tem as versões mais recentes. Os provedores de autenticação usados são fornecidos pelas seguintes bibliotecas de Identidade do Azure:
>
> - Os desenvolvedores do .NET precisam adicionar o [pacote Azure.Identity](/dotnet/api/azure.identity) .
> - Os desenvolvedores de JavaScript precisam adicionar a [biblioteca @azure/identidade](/javascript/api/@azure/identity) .
> - Os desenvolvedores de Java e Android precisam adicionar [a biblioteca de identidade do azure](/java/api/overview/azure/identity-readme) .

## <a name="authorization-code-provider"></a>Provedor de código de autorização

O fluxo de código de autorização permite que aplicativos Nativos e Web obtenham tokens com segurança no nome do usuário. Para saber mais, confira plataforma de identidade da Microsoft fluxo de código de autorização [do OAuth 2.0](/azure/active-directory/develop/v2-oauth2-auth-code-flow).

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

// using Azure.Identity;
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

Ainda não disponível. Dê suporte ou abra uma [solicitação de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não está disponível. Vote ou abra uma solicitação [de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota-authentication-azure-go"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewAuthorizationCodeCredential(
    "TENANT_ID",
    "CLIENT_ID",
    "AUTH_CODE",
    "REDIRECT_URL",
    &azidentity.AuthorizationCodeCredentialOptions {
        ClientSecret: "CLIENT_SECRET",
    },
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="client-credentials-provider"></a>Provedor de credenciais do cliente

O fluxo de credenciais do cliente permite que os aplicativos de serviço executem sem interação do usuário. O acesso é baseado na identidade do aplicativo. Para obter mais informações, [plataforma de identidade da Microsoft fluxo de credenciais do cliente OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).

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

// using Azure.Identity;
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

// using Azure.Identity;
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

Ainda não está disponível. Dê suporte ou abra uma [solicitação de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não está disponível. Dê suporte ou abra uma [solicitação de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota-authentication-azure-go"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewClientSecretCredential(
    "TENANT_ID",
    "CLIENT_ID",
    "CLIENT_SECRET",
    nil,
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="on-behalf-of-provider"></a>Provedor em nome de

O fluxo em nome de é aplicável quando seu aplicativo chama um serviço/API Web que, por sua vez, chama o Microsoft API do Graph. Saiba mais lendo [plataforma de identidade da Microsoft e o fluxo On-Behalf-Of do OAuth 2.0](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="c"></a>[C#](#tab/CS)

O `Azure.Identity` pacote não dá suporte ao fluxo em nome da versão 1.4.0. Em vez disso, crie um provedor de autenticação personalizado usando a MSAL.

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

// using Azure.Identity;
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

Fluxos OAuth em nome de exigem que você implemente um provedor de autenticação personalizado no momento. Leia [Usando o Provedor de Autenticação Personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) para obter mais informações.

# <a name="java"></a>[Java](#tab/Java)

```java
final OnBehalfOfCredential onBehalfOfCredential = new OnBehalfOfCredentialBuilder()
        .clientId(clientID)
        .pfxCertificate(pfxCertificatePath) // or .pemCertificate(certificatePath) or .clientSecret("ClientSecret")
        .clientCertificatePassword(pfxCertificatePassword) // remove if using pemCertificate or clientSecret
        .tokenCachePersistenceOptions(tokenCachePersistenceOptions) //Optional: enables the persistent token cache which is disabled by default
        .userAssertion(userAssertion)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, onBehalfOfCredential);

final GraphServiceClient graphClient = GraphServiceClient
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

Ainda não disponível. Vote ou abra uma solicitação [de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não disponível. Vote ou abra uma solicitação [de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

Ainda não disponível. Vote ou abra uma solicitação [de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

---

## <a name="implicit-provider"></a>Provedor implícito

O fluxo de Autenticação Implícita não é recomendado devido às [suas desvantagens](https://datatracker.ietf.org/doc/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6). Clientes públicos, como aplicativos nativos e aplicativos JavaScript, agora devem usar o fluxo de código de autorização com a extensão PKCE. [Referência.](https://oauth.net/2/grant-types/implicit/)

## <a name="device-code-provider"></a>Provedor de código do dispositivo

O fluxo de código do dispositivo permite entrar em dispositivos por meio de outro dispositivo. Para obter detalhes, [consulte plataforma de identidade da Microsoft fluxo de código do dispositivo OAuth 2.0](/azure/active-directory/develop/v2-oauth2-device-code).

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

// using Azure.Identity;
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

Ainda não disponível. Vote ou abra uma solicitação [de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não disponível. Vote ou abra uma solicitação [de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota-authentication-azure-go"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewDeviceCodeCredential(&azidentity.DeviceCodeCredentialOptions{
    ClientID: "CLIENT_ID",
    UserPrompt: func(ctx context.Context, message azidentity.DeviceCodeMessage) error {
        fmt.Println(message.Message)
        return nil
    },
})

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="integrated-windows-provider"></a>Provedor Windows integrado

O fluxo Windows integrado fornece uma maneira para que Windows computadores adquiram silenciosamente um token de acesso quando eles são ingressados no domínio. Para obter detalhes, consulte [Autenticação do Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).

# <a name="c"></a>[C#](#tab/CS)

No `Azure.Identity` momento, o pacote não dá suporte Windows autenticação integrada. Em vez disso, crie um provedor de autenticação personalizado usando a MSAL.

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

# <a name="go"></a>[Ir](#tab/Go)

Não aplicável.

---

## <a name="interactive-provider"></a>Provedor interativo

O fluxo interativo é usado por aplicativos móveis (Xamarin e UWP) e aplicativos de área de trabalho para chamar o Microsoft Graph em nome de um usuário. Para obter detalhes, [consulte Adquirir tokens interativamente](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

// using Azure.Identity;
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

Ainda não disponível. Vote ou abra uma solicitação [de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

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

```objectivec
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

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota-authentication-azure-go"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewInteractiveBrowserCredential(&azidentity.InteractiveBrowserCredentialOptions {
    TenantID: "TENANT_ID",
    ClientID: "CLIENT_ID",
    RedirectURL: "REDIRECT_URL",
})

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="usernamepassword-provider"></a>Provedor de nome de usuário/senha

O provedor de nome de usuário/senha permite que um aplicativo conecte um usuário usando seu nome de usuário e senha. Use esse fluxo somente quando não for possível usar nenhum dos outros fluxos OAuth. Para obter mais informações, [plataforma de identidade da Microsoft a credencial de senha do proprietário do recurso OAuth 2.0](/azure/active-directory/develop/v2-oauth-ropc)

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

// using Azure.Identity;
var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

var userName = "adelev@contoso.com";
var password = "P@ssword1!";

// https://docs.microsoft.com/dotnet/api/azure.identity.usernamepasswordcredential
var userNamePasswordCredential = new UsernamePasswordCredential(
    userName, password, tenantId, clientId, options);

var graphClient = new GraphServiceClient(userNamePasswordCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Ainda não disponível. Vote ou abra uma solicitação [de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

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

Ainda não disponível. Vote ou abra uma solicitação [de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não disponível. Vote ou abra uma solicitação [de recurso do Microsoft Graph caso](https://aka.ms/graphrequests) isso seja importante para você.

# <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota-authentication-azure-go"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewUsernamePasswordCredential(
    "TENANT_ID",
    "CLIENT_ID",
    "USER_NAME",
    "PASSWORD",
    nil,
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="next-steps"></a>Próximas etapas

- Para obter exemplos de código que mostram como usar o plataforma de identidade da Microsoft para proteger diferentes tipos de aplicativo, consulte plataforma de identidade da Microsoft de código (ponto de extremidade [v2.0)](/azure/active-directory/develop/sample-v2-code).
- Os provedores de autenticação exigem uma ID de cliente. Você desejará registrar seu [aplicativo depois](https://portal.azure.com/) de configurar seu provedor de autenticação.
- Informe-nos se no momento não há suporte para um fluxo OAuth necessário votando ou abrindo uma solicitação de recurso do [Microsoft Graph.](https://aka.ms/graphrequests)
