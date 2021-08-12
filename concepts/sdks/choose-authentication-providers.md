---
title: Escolha um provedor de autenticação Graph microsoft
description: Saiba como escolher provedores de autenticação específicos de cenário para seu aplicativo.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 13775e15660f6a3d355553514325c268d3f7f89af404918968d63c9b9b858a15
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236875"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a>Escolher um provedor de autenticação do Microsoft Graph com base no cenário

Os provedores de autenticação implementam o código necessário para adquirir um token usando a Biblioteca de Autenticação da Microsoft (MSAL); lidar com vários erros potenciais para casos como consentimento incremental, senhas expiradas e acesso condicional; e, em seguida, de definir o cabeçalho de autorização de solicitação HTTP. A tabela a seguir lista o conjunto de provedores que combinam com os cenários de diferentes tipos [de aplicativo.](/azure/active-directory/develop/v2-app-types)

|Cenário | Flow/Grant | Espectadores | Provedor|
|--|--|--|--|
| [Aplicativo de Página Única](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | Implícito | Consumidor Delegado/Org |[Provedor Implícito](#ImplicitProvider) |
| [Aplicativo Web que chama APIs da Web](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | Código de Autorização | Consumidor Delegado/Org | [Provedor de Código de Autorização](#AuthCodeProvider) |
| | Credenciais do cliente  | Somente aplicativo | [Provedor de Credenciais do Cliente](#ClientCredentialsProvider) |
| [API Web que chama APIs da Web](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | Em nome de | Consumidor Delegado/Org | [Em nome do provedor](#OnBehalfOfProvider) |
| | Credenciais do cliente  | Somente aplicativo | [Provedor de Credenciais do Cliente](#ClientCredentialsProvider) |
| [Aplicativo de área de trabalho que chama APIs da Web](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | Interativo | Consumidor Delegado/Org | [Provedor Interativo](#InteractiveProvider) |
| | Integração Windows | Organização Delegada | [Provedor Windows integrado](#IntegratedWindowsProvider) |
| | Proprietário do Recurso  | Organização Delegada | [Username /Password Provider](#UsernamePasswordProvider) |
| | Código do dispositivo  | Organização Delegada | [Provedor de Código de Dispositivo](#DeviceCodeProvider) |
| [Aplicativo Daemon](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | Credenciais do cliente  | Somente aplicativo | [Provedor de Credenciais do Cliente](#ClientCredentialsProvider) |
| [Aplicativo móvel que chama APIs da Web](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | Interativo | Consumidor Delegado/Org | [Provedor Interativo](#InteractiveProvider) |

> Observação: Java desenvolvedores android precisam adicionar a biblioteca [do azure-identity](/java/api/overview/azure/identity-readme?view=azure-java-stable) para obter acesso aos diferentes tipos de credenciais.

## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a>Provedor de código de autorização

O fluxo de código de autorização permite que aplicativos nativos e web obtenham tokens com segurança no nome do usuário. Para saber mais, confira plataforma de identidade da Microsoft fluxo de código de autorização [do OAuth 2.0](/azure/active-directory/develop/v2-oauth2-auth-code-flow).

# <a name="c"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

O código de autorização, a credencial do cliente e os fluxos em nome do OAuth exigem que você implemente um provedor de autenticação personalizado no momento. Para obter mais informações, consulte [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).

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

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a>Provedor de credenciais do cliente

O fluxo de credenciais do cliente permite que aplicativos de serviço executem sem interação do usuário. O Access baseia-se na identidade do aplicativo. Para obter mais informações, consulte plataforma de identidade da Microsoft e o fluxo de credenciais do cliente [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

# <a name="c"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

O código de autorização, a credencial do cliente e os fluxos em nome do OAuth exigem que você implemente um provedor de autenticação personalizado no momento. Para obter mais informações, consulte [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).

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

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a>Provedor on-behalf-of

O fluxo em nome do fluxo é aplicável quando seu aplicativo chama uma API de serviço/web que, por sua vez, chama a API Graph Microsoft. Saiba mais lendo [o plataforma de identidade da Microsoft e o fluxo OAuth 2.0 On-Behalf-Of](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="c"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

O código de autorização, a credencial do cliente e os fluxos em nome do OAuth exigem que você implemente um provedor de autenticação personalizado no momento. Leia [Usando o Provedor de Autenticação Personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) para obter mais informações.

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

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a>Provedor implícito

O fluxo de concessão implícito é usado em aplicativos baseados em navegador. Para obter mais informações, [consulte plataforma de identidade da Microsoft fluxo de concessão implícito.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)

# <a name="c"></a>[C#](#tab/CS)

Não aplicável.

# <a name="javascript"></a>[Javascript](#tab/Javascript)

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

##  <a name="device-code-provider"></a><a name="DeviceCodeProvider"></a>Provedor de código de dispositivo

O fluxo de código do dispositivo permite entrar em dispositivos por meio de outro dispositivo. Para obter detalhes, consulte plataforma de identidade da Microsoft e o fluxo de código do dispositivo [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-device-code)

# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Ainda não está disponível. Vote ou abra uma solicitação de [recurso Graph microsoft](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) se isso for importante para você.

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

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a>Provedor Windows integrado

O fluxo Windows integrado fornece uma maneira de Windows computadores adquirirem silenciosamente um token de acesso quando eles estão ingressados no domínio. Para obter detalhes, consulte [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).

# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
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

##  <a name="interactive-provider"></a><a name="InteractiveProvider"></a>Provedor interativo

O fluxo interativo é usado por aplicativos móveis (Xamarin e UWP) e aplicativos de área de trabalho para chamar a Microsoft Graph em nome de um usuário. Para obter detalhes, consulte [Adquirindo tokens interativamente](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).

# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
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

##  <a name="usernamepassword-provider"></a><a name="UsernamePasswordProvider"></a>Provedor de nome de usuário/senha

O provedor de nome de usuário/senha permite que um aplicativo entre em um usuário usando seu nome de usuário e senha. Use esse fluxo somente quando você não puder usar nenhum dos outros fluxos OAuth. Para obter mais informações, consulte plataforma de identidade da Microsoft e a credencial de senha do proprietário do recurso [OAuth 2.0](/azure/active-directory/develop/v2-oauth-ropc)



# <a name="c"></a>[C#](#tab/CS)

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
