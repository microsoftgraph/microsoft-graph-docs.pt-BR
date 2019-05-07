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
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-oauth-flow"></a>Escolher um provedor de autenticação do Microsoft Graph com base no fluxo OAuth

Os provedores de autenticação simplificam a obter um token de acesso, abstraindo os parâmetros exigidos pelas bibliotecas de clientes de autenticação. Os provedores de autenticação do Microsoft Graph simplificam o uso da biblioteca de autenticação da Microsoft (MSAL) fornecendo adaptadores para cada plataforma. Esses adaptadores tratam da aquisição de token para seu aplicativo. Os provedores de autenticação do Microsoft Graph mapeiam para um fluxo de concessão OAuth. Você precisará saber qual fluxo de concessão OAuth usar para seu aplicativo para selecionar o provedor de autenticação apropriado para seu aplicativo.

## <a name="authorization-code-oauth-flow"></a>Fluxo OAuth de código de autorização

O fluxo de código de autorização permite que aplicativos nativos e Web obtenham tokens com segurança no nome do usuário. Para saber mais, confira [Microsoft Identity Platform and OAuth 2,0 Authorization Code Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).

# <a name="ctabcs"></a>[Basic](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = AuthorizationCodeProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/Javascript)

O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento. Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/Objective-C)

Não aplicável.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Ainda não disponível. Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Não disponível, ainda. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

---

## <a name="client-credential-oauth-flow"></a>Fluxo OAuth de credenciais do cliente

O fluxo de credenciais do cliente permite que aplicativos de serviço sejam executados sem interação do usuário. O acesso baseia-se na identidade do aplicativo. Para obter mais informações, consulte [Microsoft Identity Platform e The OAuth 2,0 Client Credentials Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).

# <a name="ctabcs"></a>[Basic](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = ClientCredentialProvider.CreateClientApplication(clientId, clientCredential);
ClientCredentialProvider authProvider = new ClientCredentialProvider(clientApplication);
```

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/Javascript)

O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento. Para obter mais informações, consulte [usar um provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/Objective-C)

Não aplicável.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Não disponível, ainda. Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Não disponível, ainda. Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

---

## <a name="on-behalf-of-oauth-flow"></a>Fluxo de OAuth em nome de

O fluxo em nome de é aplicável quando o aplicativo chama uma API de serviço/Web que, em seguida, chama a API do Microsoft Graph. Saiba mais lendo a [plataforma de identidade da Microsoft e o fluxo em nome de do OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="ctabcs"></a>[Basic](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = OnBehalfOfProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
OnBehalfOfProvider authProvider = new OnBehalfOfProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/Javascript)

O código de autorização, a credencial do cliente e os fluxos do OAuth em nome de OAuth exigem que você implemente um provedor de autenticação personalizado no momento. Leia [usando provedor de autenticação personalizado](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) para obter mais informações.

# <a name="javatabjava"></a>[Java](#tab/Java)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/Objective-C)

Não aplicável.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

---

## <a name="implicit-grant-oauth-flow"></a>Fluxo de concessão OAuth implícito

O fluxo de concessão implícito é usado em aplicativos baseados em navegador. Para obter mais informações, consulte [Microsoft Identity Platform and implícito Grant Flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).

# <a name="ctabcs"></a>[Basic](#tab/CS)

Não aplicável.

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/Javascript)

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

# <a name="javatabjava"></a>[Java](#tab/Java)

Não aplicável.

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/Objective-C)

Não aplicável.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Não aplicável.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Não aplicável.

---

## <a name="device-code-oauth-flow"></a>Fluxo OAuth de código de dispositivo

O fluxo de código de dispositivo permite entrar em dispositivos por meio de outro dispositivo. Para obter detalhes, consulte [plataforma de identidade da Microsoft e o fluxo de código de dispositivo OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).

# <a name="ctabcs"></a>[Basic](#tab/CS)

```csharp
IPublicClientApplication clientApplication = DeviceCodeProvider.CreateClientApplication(clientId);
DeviceCodeProvider authProvider = new DeviceCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/Javascript)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="javatabjava"></a>[Java](#tab/Java)

Não disponível, ainda. Forneça suporte ou abra uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/Objective-C)

Não aplicável.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

---

## <a name="integrated-windows-flow"></a>Fluxo integrado do Windows

O fluxo integrado do Windows oferece uma maneira para que os computadores com Windows adquiram um token de acesso de forma silenciosa quando são associados ao domínio. Para obter detalhes, consulte [autenticação integrada do Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).

# <a name="ctabcs"></a>[Basic](#tab/CS)

```csharp
IPublicClientApplication clientApplication = IntegratedWindowsAuthenticationProvider.CreateClientApplication(clientId);
IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/Javascript)

Não aplicável.

# <a name="javatabjava"></a>[Java](#tab/Java)

Não aplicável.

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/Objective-C)

Não aplicável.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Não aplicável.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Não aplicável.

---

## <a name="interactive-flow"></a>Fluxo interativo

O fluxo interativo é usado por aplicativos móveis (Xamarin e UWP) e aplicativos de área de trabalho para chamar o Microsoft Graph no nome de um usuário. Para obter detalhes, [](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)consulte adquirindo tokens interativamente.

# <a name="ctabcs"></a>[Basic](#tab/CS)

```csharp
IPublicClientApplication clientApplication = InteractiveAuthenticationProvider.CreateClientApplication(clientId);
InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/Javascript)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="javatabjava"></a>[Java](#tab/Java)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="androidtabandroid"></a>[Android](#tab/Android)

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

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Não aplicável.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Não aplicável.

---

## <a name="resource-owner-password-credential-grant-oauth-flow"></a>Credencial do proprietário do recurso conceder fluxo OAuth

O fluxo de credenciais da senha do proprietário do recurso permite que um aplicativo entre em um usuário usando seu nome de usuário e senha. Use este fluxo somente quando não for possível usar qualquer um dos outros fluxos OAuth. Para obter mais informações, consulte [plataforma de identidade da Microsoft e a credencial de senha de proprietário do recurso OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)



# <a name="ctabcs"></a>[Basic](#tab/CS)

```csharp
IPublicClientApplication clientApplication = UsernamePasswordProvider.CreateClientApplication(clientId);
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/Javascript)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Não aplicável.

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/Objective-C)

Não aplicável.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Ainda não disponível. Vote ou abra uma solicitação de [recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) se isso for importante para você.

---

## <a name="next-steps"></a>Próximas etapas

* Os provedores de autenticação exigem uma ID de cliente. Você deve [registrar seu aplicativo](https://portal.azure.com/) depois de configurar seu provedor de autenticação.
* Deixe-nos saber se um fluxo OAuth necessário atualmente não é suportado pela votação ou pela abertura de uma [solicitação de recurso do Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).