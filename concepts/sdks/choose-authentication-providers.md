---
title: Escolher um provedor de autenticação do Microsoft Graph
description: Saiba como escolher provedores de autenticação específicos do cenário para seu aplicativo.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 0570087f3b512d7416093757feab43a5f5926310
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364247"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a>Escolher um provedor de autenticação do Microsoft Graph com base no cenário

Os provedores de autenticação implementam o código necessário para adquirir um token usando a biblioteca de autenticação da Microsoft (MSAL); gerenciar vários erros potenciais para casos como o consentimento incremental, senhas expiradas e acesso condicional; e, em seguida, defina o cabeçalho de autorização da solicitação HTTP. A tabela a seguir lista o conjunto de provedores que correspondem aos cenários para diferentes [tipos de aplicativos](/azure/active-directory/develop/v2-app-types).

|Cenário | Fluxo/concessão | Espectadores | Provedor|
|--|--|--|--|
| [Aplicativo de página única](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | Implícito | Consumidor/org delegada |[Provedor implícito](#ImplicitProvider) |
| [Aplicativo Web que chama APIs da Web](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | Código de Autorização | Consumidor/org delegada | [Provedor de código de autorização](#AuthCodeProvider) |
| | Credenciais do cliente  | Somente aplicativo | [Provedor de credenciais do cliente](#ClientCredentialsProvider) |
| [API Web que chama APIs da Web](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | Em nome de | Consumidor/org delegada | [Em nome do provedor](#OnBehalfOfProvider) |
| | Credenciais do cliente  | Somente aplicativo | [Provedor de credenciais do cliente](#ClientCredentialsProvider) |
| [Aplicativo de área de trabalho que chama APIs da Web](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | Interativo | Consumidor/org delegada | [Provedor interativo](#InteractiveProvider) |
| | Integrada do Windows | Organização delegada | [Provedor integrado do Windows](#IntegratedWindowsProvider) |
| | Proprietário do recurso  | Organização delegada | [Provedor de nome de usuário/senha](#UsernamePasswordProvider) |
| | Código de dispositivo  | Organização delegada | [Provedor de código de dispositivo](#DeviceCodeProvider) |
| [Aplicativo daemon](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | Credenciais do cliente  | Somente aplicativo | [Provedor de credenciais do cliente](#ClientCredentialsProvider) |
| [Aplicativo móvel que chama as APIs Web](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | Interativo | Consumidor/org delegada | [Provedor interativo](#InteractiveProvider) |


## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a>Provedor de código de autorização

O fluxo de código de autorização permite que aplicativos nativos e Web obtenham tokens com segurança no nome do usuário. Para saber mais, confira [Microsoft Identity Platform and OAuth 2,0 Authorization Code Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow).

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

O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento. Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).

# <a name="java"></a>[Java](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="android"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Não aplicável.

# <a name="php"></a>[PHP](#tab/PHP)

Ainda não disponível. Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Não disponível, ainda. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

---

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a>Provedor de credenciais do cliente

O fluxo de credenciais do cliente permite que aplicativos de serviço sejam executados sem interação do usuário. O acesso baseia-se na identidade do aplicativo. Para obter mais informações, consulte [Microsoft Identity Platform e The OAuth 2,0 Client Credentials Flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).

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

O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento. Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).

# <a name="java"></a>[Java](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="android"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Não aplicável.

# <a name="php"></a>[PHP](#tab/PHP)

Não disponível, ainda. Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Não disponível, ainda. Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

---

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a>Provedor em nome de

O fluxo em nome de é aplicável quando o aplicativo chama uma API de serviço/Web que, em seguida, chama a API do Microsoft Graph. Saiba mais lendo a [plataforma de identidade da Microsoft e o fluxo em nome de do OAuth 2,0](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

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

O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento. Leia [usando provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) para obter mais informações.

# <a name="java"></a>[Java](#tab/Java)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="android"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Não aplicável.

# <a name="php"></a>[PHP](#tab/PHP)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

---

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a>Provedor implícito

O fluxo de concessão implícito é usado em aplicativos baseados em navegador. Para obter mais informações, consulte [Microsoft Identity Platform and implícito Grant Flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).

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

O fluxo de código de dispositivo permite entrar em dispositivos por meio de outro dispositivo. Para obter detalhes, consulte [plataforma de identidade da Microsoft e o fluxo de código de dispositivo OAuth 2,0](/azure/active-directory/develop/v2-oauth2-device-code).

# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="java"></a>[Java](#tab/Java)

Não disponível, ainda. Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="android"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Não aplicável.

# <a name="php"></a>[PHP](#tab/PHP)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

---

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a>Provedor integrado do Windows

O fluxo integrado do Windows oferece uma maneira para que os computadores com Windows adquiram um token de acesso de forma silenciosa quando são associados ao domínio. Para obter detalhes, consulte [autenticação integrada do Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).

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

O fluxo interativo é usado por aplicativos móveis (Xamarin e UWP) e aplicativos de área de trabalho para chamar o Microsoft Graph no nome de um usuário. Para obter detalhes, consulte [adquirindo tokens interativamente](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).

# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="java"></a>[Java](#tab/Java)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="android"></a>[Android](#tab/Android)

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

O provedor de nome de usuário/senha permite que um aplicativo entre em um usuário usando seu nome de usuário e senha. Use este fluxo somente quando não for possível usar qualquer um dos outros fluxos OAuth. Para obter mais informações, consulte [plataforma de identidade da Microsoft e a credencial de senha de proprietário do recurso OAuth 2,0](/azure/active-directory/develop/v2-oauth-ropc)



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

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="java"></a>[Java](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="android"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Não aplicável.

# <a name="php"></a>[PHP](#tab/PHP)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

---

## <a name="next-steps"></a>Próximas etapas

* Os provedores de autenticação exigem uma ID de cliente. Você deve [registrar seu aplicativo](https://portal.azure.com/) depois de configurar seu provedor de autenticação.
* Deixe-nos saber se um fluxo OAuth necessário atualmente não é suportado pela votação ou pela abertura de uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
