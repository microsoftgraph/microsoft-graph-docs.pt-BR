---
title: Obter acesso em nome de um usuário
description: Para usar o Microsoft Graph para ler e gravar recursos em nome de um usuário, seu aplicativo deve obter um token de acesso do Azure AD e anexar o token às solicitações que ele envia para o Microsoft Graph.
author: jackson-woods
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: graphiamtop20
ms.openlocfilehash: d2b3c7a26a0a4d5005f22893e0295585f5e7033b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846153"
---
# <a name="get-access-on-behalf-of-a-user"></a>Obter acesso em nome de um usuário

To use Microsoft Graph to read and write resources on behalf of a user, your app must get an access token from the Microsoft identity platform and attach the token to requests that it sends to Microsoft Graph. The exact authentication flow that you will use to get access tokens will depend on the kind of app you are developing and whether you want to use OpenID Connect to sign the user in to your app. One common flow used by native and mobile apps and also by some Web apps is the OAuth 2.0 authorization code grant flow. This topic  walks through an example using this flow.

## <a name="authentication-and-authorization-steps"></a>Etapas de Autenticação e Autorização

As etapas básicas necessárias para usar o fluxo de concessão de código de autorização do OAuth 2.0 para obter um token de acesso do ponto de extremidade da plataforma de identidade da Microsoft são:

1. Registre seu aplicativo com o Azure AD.
2. Obtenha autorização.
3. Obtenha um token de acesso.
4. Chame o Microsoft Graph usando o token de acesso.
5. Use um token de atualização para obter um novo token de acesso.

## <a name="1-register-your-app"></a>1. Registre seu aplicativo

To use the Microsoft identity platform endpoint, you must register your app using the Azure [app registration portal](https://go.microsoft.com/fwlink/?linkid=2083908). You can use either a Microsoft account or a work or school account to register an app.

Para configurar um aplicativo para usar o fluxo de concessão do código de autorização do OAuth 2.0, salve os seguintes valores quando registrar o aplicativo:

- A ID do Aplicativo (cliente) atribuída pelo portal de registro do aplicativo.
- Um Segredo do Cliente (aplicativo), que pode ser uma senha ou um par de chaves públicas/particulares (certificado). Isso não é necessário para aplicativos nativos.
- Uma URL de redirecionamento (ou URL de resposta) para seu aplicativo receber respostas do Azure AD.

Para saber como configurar um aplicativo no portal do Azure, confira [Registrar seu aplicativo](./auth-register-app-v2.md).

## <a name="2-get-authorization"></a>2. Obter autorização

A primeira etapa para obter um token de acesso para muitos fluxos do OpenID Connect e do OAuth 2.0 é redirecionar o usuário para o ponto de extremidade `/authorize` da plataforma de identidade da Microsoft. O Azure AD conectará o usuário e garantirá seu consentimento para as permissões solicitadas pelo seu aplicativo. No fluxo de concessão do código de autorização, depois de obter o consentimento, o Azure AD retorna um authorization_code para o aplicativo que pode resgatá-lo no ponto de extremidade `/token` da plataforma de identidade da Microsoft para obter um token de acesso.

### <a name="authorization-request"></a>Solicitação de autorização

Veja a seguir um exemplo de solicitação para o ponto de extremidade `/authorize`.

Com o ponto de extremidade da plataforma de identidade da Microsoft, as permissões são solicitadas usando o parâmetro `scope`. Neste exemplo, as permissões do Microsoft Graph solicitadas são para _User.Read_ e _Mail.Read_, o que permitirá que o aplicativo leia o perfil e o email do usuário conectado. A permissão de _acesso\_online_ é solicitada para que o aplicativo possa obter um token de atualização que pode ser usado para obter um novo token de acesso quando o atual expirar.

```
// Line breaks for legibility only

https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize?
client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&response_type=code
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&response_mode=query
&scope=offline_access%20user.read%20mail.read
&state=12345
```

| Parâmetro     | Obrigatório    | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------|-------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| locatário        | obrigatório    | The `{tenant}` value in the path of the request can be used to control who can sign into the application.  The allowed values are `common` for both Microsoft accounts and work or school accounts, `organizations` for work or school accounts only, `consumers` for Microsoft accounts only, and tenant identifiers such as the tenant ID or domain name.  For more detail, see [protocol basics](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints). |
| client_id     | obrigatório    | A ID do Aplicativo atribuída ao seu aplicativo no [portal de registro](https://go.microsoft.com/fwlink/?linkid=2083908).                                                                                                                                                                                                                                                                                                                                                                                   |
| response_type | obrigatório    | Pode incluir `code` para o fluxo do código de autorização.                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| redirect_uri  | recomendado | The redirect_uri of your app, where authentication responses can be sent and received by your app.  It must exactly match one of the redirect_uris you registered in the app registration portal, except it must be URL encoded.  For native and mobile apps, you should use the default value of `https://login.microsoftonline.com/common/oauth2/nativeclient`.                                                                                                                                       |
| escopo         | obrigatório    | A space-separated list of the Microsoft Graph permissions that you want the user to consent to. This may also include OpenID scopes.                                                                                                                                                                                                                                                                                                                                                                    |
| response_mode | recomendado | Specifies the method that should be used to send the resulting token back to your app.  Can be `query` or `form_post`.                                                                                                                                                                                                                                                                                                                                                                                  |
| estado         | recomendado | A value included in the request that will also be returned in the token response.  It can be a string of any content that you wish.  A randomly generated unique value is typically used for [preventing cross-site request forgery attacks](https://tools.ietf.org/html/rfc6749#section-10.12).  The state is also used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.                                     |

> **Important**: Microsoft Graph exposes two kinds of permissions: application and delegated. For apps that run with a signed-in user, you request delegated permissions in the `scope` parameter. These permissions delegate the privileges of the signed-in user to your app, allowing it to act as the signed-in user when making calls to Microsoft Graph. For more detailed information about the permissions available through Microsoft Graph, see the [Permissions reference](./permissions-reference.md).

### <a name="consent-experience"></a>Experiência de consentimento

Neste ponto, o usuário será solicitado a digitar suas credenciais para autenticar usando a Microsoft. O ponto de extremidade v2.0 da plataforma de identidade da Microsoft também assegurará que o usuário concordou com as permissões indicadas no parâmetro de consulta `scope`.  Se o usuário não tiver concordado com nenhuma dessas permissões e se um administrador não tiver concordado previamente em nome de todos os usuários na organização, será solicitado aos usuários que autorizem as permissões necessárias.

O exemplo a seguir mostra a caixa de diálogo de consentimento apresentada para uma conta de usuário da Microsoft.

![Caixa de diálogo de consentimento da conta da Microsoft](./images/v2-consumer-consent.png)

> **Try** If you have a Microsoft account or an Azure AD work or school account, you can try this for yourself by clicking the following link. After signing in, your browser should be redirected to `https://localhost/myapp/` with a `code` in the address bar.
>
> <a href="https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&response_type=code&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F&response_mode=query&scope=offline_access%20user.read%20mail.read&state=12345" target="_blank">https://login.microsoftonline.com/common/oauth2/v2.0/authorize...</a>

### <a name="authorization-response"></a>Resposta da autorização

If the user consents to the permissions your app requested, the response will contain the authorization code in the `code` parameter. Here is an example of a successful response to the previous request. Because the `response_mode` parameter in the request was set to `query`, the response is returned in the query string of the redirect URL.

```
GET https://localhost/myapp/?
code=M0ab92efe-b6fd-df08-87dc-2c6500a7f84d
&state=12345
```

| Parâmetro | Descrição                                                                                                                                                                                                                        |
|-----------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| código      | The authorization_code that the app requested. The app can use the authorization code to request an access token for the target resource.  Authorization_codes are very short lived, typically they expire after about 10 minutes. |
| estado     | If a state parameter is included in the request, the same value should appear in the response. The app should verify that the state values in the request and response are identical.                                              |

## <a name="3-get-a-token"></a>3. Obtenha um token

Seu aplicativo usa a autorização `code` recebida na etapa anterior para solicitar um token de acesso enviando uma solicitação `POST` para o ponto de extremidade `/token`.

### <a name="token-request"></a>Solicitação de token

```
// Line breaks for legibility only

POST /{tenant}/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&code=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq3n8b2JRLk4OxVXr...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=authorization_code
&client_secret=JqQX2PNo9bpM0uEihUPzyrh    // NOTE: Only required for web apps
```

| Parâmetro     | Obrigatório              | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| locatário        | obrigatório              | The `{tenant}` value in the path of the request can be used to control who can sign into the application.  The allowed values are `common` for both Microsoft accounts and work or school accounts, `organizations` for work or school accounts only, `consumers` for Microsoft accounts only, and tenant identifiers such as the tenant ID or domain name.  For more detail, see [protocol basics](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints). |
| client_id     | obrigatório              | A ID do Aplicativo atribuída ao seu aplicativo no [portal de registro)](https://go.microsoft.com/fwlink/?linkid=2083908).                                                                                                                                                                                                                                                                                                                                                                                  |
| grant_type    | obrigatório              | Deve ser `authorization_code` para o fluxo de código de autorização.                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| escopo         | obrigatório              | A space-separated list of scopes.  The scopes requested in this leg must be equivalent to or a subset of the scopes requested in the first (authorization) leg.  If the scopes specified in this request span multiple resource servers, then the v2.0 endpoint will return a token for the resource specified in the first scope.                                                                                                                                                                      |
| código          | obrigatório              | O authorization_code adquirido na primeira etapa do fluxo.                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| redirect_uri  | obrigatório              | O mesmo valor do redirect_uri que foi usado para adquirir o authorization_code.                                                                                                                                                                                                                                                                                                                                                                                                                            |
| client_secret | obrigatório para aplicativos Web | The application secret that you created in the app registration portal for your app.  It should not be used in a native app, because client_secrets cannot be reliably stored on devices.  It is required for web apps and web APIs, which have the ability to store the client_secret securely on the server side.                                                                                                                                                                                     |

### <a name="token-response"></a>Resposta do token

Embora o token de acesso seja opaco para o aplicativo, a resposta contém uma lista das permissões para as quais o token de acesso servirá no parâmetro `scope`.

```json
{
    "token_type": "Bearer",
    "scope": "user.read%20Fmail.read",
    "expires_in": 3600,
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4..."
}
```

| Parâmetro     | Descrição                                                                                                                                                                                                                                                                                                                                                                                  |
|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| token_type    | Indicates the token type value. The only type that Azure AD supports is Bearer.                                                                                                                                                                                                                                                                                                              |
| scope         | Uma lista separada por espaços das permissões do Microsoft Graph para as quais o access_token é válido.                                                                                                                                                                                                                                                                                                |
| expires_in    | Por quanto tempo o token de acesso é válido (em segundos).                                                                                                                                                                                                                                                                                                                                             |
| access_token  | The requested access token. Your app can use this token to call Microsoft Graph.                                                                                                                                                                                                                                                                                                             |
| refresh_token | Um token de atualização OAuth 2.0. Seu aplicativo poderá usar este token para adquirir tokens de acesso adicionais depois que o token de acesso atual expirar.  Os tokens de atualização são de longa duração e podem ser usados para manter o acesso aos recursos por longos períodos de tempo.  Confira mais detalhes na [referência de token v2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-tokens). |

## <a name="4-use-the-access-token-to-call-microsoft-graph"></a>4. Use o token de acesso para chamar o Microsoft Graph

After you have an access token, you can use it to call Microsoft Graph by including it in the `Authorization` header of a request. The following request gets the profile of the signed-in user.

```
GET https://graph.microsoft.com/v1.0/me
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com

```

Uma resposta bem-sucedida terá a seguinte aparência (alguns cabeçalhos de resposta foram removidos).

```
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
request-id: f45d08c0-6901-473a-90f5-7867287de97f
client-request-id: f45d08c0-6901-473a-90f5-7867287de97f
OData-Version: 4.0
Duration: 727.0022
Date: Thu, 20 Apr 2017 05:21:18 GMT
Content-Length: 407

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id":"12345678-73a6-4952-a53a-e9916737ff7f",
    "businessPhones":[
        "+1 555555555"
    ],
    "displayName":"Chris Green",
    "givenName":"Chris",
    "jobTitle":"Software Engineer",
    "mail":null,
    "mobilePhone":"+1 5555555555",
    "officeLocation":"Seattle Office",
    "preferredLanguage":null,
    "surname":"Green",
    "userPrincipalName":"ChrisG@contoso.onmicrosoft.com"
}
```

## <a name="5-use-the-refresh-token-to-get-a-new-access-token"></a>5. Use um token de atualização para obter um novo token de acesso

Access tokens are short lived, and you must refresh them after they expire to continue accessing resources.  You can do so by submitting another `POST` request to the `/token` endpoint, this time providing the `refresh_token` instead of the `code`.

### <a name="request"></a>Solicitação

```
// Line breaks for legibility only

POST /common/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&refresh_token=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=refresh_token
&client_secret=JqQX2PNo9bpM0uEihUPzyrh      // NOTE: Only required for web apps
```

| Parâmetro     | Obrigatório              | Descrição                                                                                                                                                                                                                                                                                                         |
|---------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client_id     | obrigatório              | A ID do Aplicativo atribuída ao seu aplicativo no [portal de registro](https://go.microsoft.com/fwlink/?linkid=2083908).                                                                                                                                                                                               |
| grant_type    | obrigatório              | Deve ser `refresh_token`.                                                                                                                                                                                                                                                                                            |
| escopo         | obrigatório              | A space-separated list of permissions (scopes).  The permissions requested must be equivalent to or a subset of the permissions requested in the original authorization_code request.                                                                                                                               |
| refresh_token | obrigatório              | O refresh_token adquirido durante a solicitação do token.                                                                                                                                                                                                                                                       |
| redirect_uri  | obrigatório              | O mesmo valor do redirect_uri que foi usado para adquirir o authorization_code.                                                                                                                                                                                                                                        |
| client_secret | obrigatório para aplicativos Web | The application secret that you created in the app registration portal for your app.  It should not be used in a native app, because client_secrets cannot be reliably stored on devices.  It is required for web apps and web APIs, which have the ability to store the client_secret securely on the server side. |

### <a name="response"></a>Resposta

Uma resposta de token bem-sucedida será semelhante ao seguinte.

```
{
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "token_type": "Bearer",
    "expires_in": 3599,
    "scope": "user.read%20mail.read",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4...",
}
```
| Parâmetro     | Descrição                                                                                                                                                                        |
|---------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| access_token  | The requested access token. The app can use this token in calls to Microsoft Graph.                                                                                                |
| token_type    | Indicates the token type value. The only type that Azure AD supports is Bearer                                                                                                     |
| expires_in    | Por quanto tempo o token de acesso é válido (em segundos).                                                                                                                                   |
| escopo         | As permissões (escopos) para as quais o access_token é válido.                                                                                                                       |
| refresh_token | A new OAuth 2.0 refresh token. You should replace the old refresh token with this newly acquired refresh token to ensure your refresh tokens remain valid for as long as possible. |

## <a name="supported-app-scenarios-and-additional-resources"></a>Recursos adicionais e cenários de aplicativo com suporte

Você pode chamar o Microsoft Graph em nome de um usuário a partir dos seguintes tipos de aplicativos:

- [Aplicativos Nativos/Móveis](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-overview)
- [Aplicativos Web](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-call-api-overview)
- [Aplicativos de página única (SPA)](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-overview)
- [Back-end de APIs da Web](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-call-api-overview): por exemplo, em cenários onde um aplicativo de cliente, como um aplicativo nativo, implementa a funcionalidade em um back-end da API da Web. Com o ponto de extremidade da plataforma de identidade da Microsoft, tanto o aplicativo de cliente quanto o back-end da API da Web devem ter a mesma ID do Aplicativo.

Para saber mais sobre os cenários de aplicativo compatíveis com o ponto de extremidade da plataforma de identidade da Microsoft, consulte [Cenários de aplicativo e fluxos de autenticação](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios).

> **Observação**: chamar o Microsoft Graph a partir de uma API da Web autônoma atualmente não tem suporte do ponto de extremidade da plataforma de identidade da Microsoft. Nesse caso, você precisa usar o ponto de extremidade do Azure AD.

Para obter mais informações sobre como obter acesso ao Microsoft Graph em nome de um usuário a partir do ponto de extremidade da plataforma de identidade da Microsoft:

- Para obter links para documentação de protocolos e artigos de introdução a diferentes tipos de aplicativos, confira a [Documentação do ponto de extremidade da plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview).
- Para obter explicações detalhadas sobre os tipos de aplicativo e os fluxos de autenticação compatíveis, confira [tipos de aplicativo v2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-app-types).
- Para obter mais informações sobre o middleware de servidor e bibliotecas de autenticação recomendadas da Microsoft e de terceiros da plataforma de identidade da Microsoft, confira as [bibliotecas de autenticação do Azure Active Directory v2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries).

## <a name="endpoint-considerations"></a>Considerações sobre o ponto de extremidade

A Microsoft continua oferecendo suporte ao ponto de extremidade do Azure AD. Existem [várias diferenças](https://docs.microsoft.com/azure/active-directory/develop/azure-ad-endpoint-comparison) entre a utilização do ponto de extremidade da plataforma de identidade da Microsoft e o ponto de extremidade do Azure AD. Durante o uso do ponto de extremidade do Azure AD:

- O aplicativo exigirá uma ID de aplicativo diferente (ID do cliente) para cada plataforma.
- Se o aplicativo for um aplicativo multilocatário, você deve configurá-lo explicitamente para funcionar como multilocatário no [portal do Azure](https://portal.azure.com).
- Todas as permissões que seu aplicativo precisa devem ser configuradas pelo desenvolvedor. O ponto de extremidade do Azure AD não oferece suporte ao consentimento dinâmico (incremental).
- The Azure AD endpoint uses a `resource` parameter in authorization and token requests to specify the resource, such as Microsoft Graph, for which it wants permissions. The endpoint does not support the `scope` parameter.
- The Azure AD endpoint does not expose a specific endpoint for administrator consent. Instead apps use the `prompt=admin_consent` parameter in the authorization request to obtain administrator consent for an organization. For more information, see **Triggering the Azure AD consent framework at runtime** in [Integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications).

Para obter mais informações sobre como obter acesso ao Microsoft Graph em nome de um usuário a partir do ponto de extremidade do Azure AD:

- Para saber mais sobre o ponto de extremidade da plataforma de identidade da Microsoft com diferentes tipos de aplicativos, confira os links de **Introdução** na [documentação de desenvolvedor da plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide). A documentação contém links para tópicos de visão geral, guias de início rápido, tutoriais, exemplos de código e documentação de protocolo para diferentes tipos de aplicativos compatíveis com o ponto de extremidade da plataforma de identidade da Microsoft.
- Para saber mais sobre a MSAL (Biblioteca de Autenticação da Microsoft) e o middleware de servidor disponíveis para uso com o ponto de extremidade da plataforma de identidade da Microsoft, confira [Bibliotecas de Autenticação da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/msal-overview).
