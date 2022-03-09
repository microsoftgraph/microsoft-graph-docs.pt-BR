---
title: Obtenha acesso sem um usuário
description: Alguns aplicativos chamam o Microsoft Graph com sua própria identidade e não em nome de um usuário. Em muitos casos, esses são os serviços em plano de fundo ou daemons que podem ser executados em um servidor sem a presença de um usuário conectado.
author: jackson-woods
ms.localizationpriority: high
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 4310bbc6c2dc64b9e59cb6f0dfe1010a043452c4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333635"
---
# <a name="get-access-without-a-user"></a>Obter acesso sem um usuário

Alguns aplicativos chamam o Microsoft Graph com sua própria identidade e não em nome de um usuário. Em muitos casos, esses aplicativos são serviços em segundo plano ou daemons executados em um servidor sem a presença de um usuário conectado. Um exemplo desse aplicativo pode ser um serviço de arquivamento de email que é ativado e executado durante a noite. Em alguns casos, os aplicativos que têm um usuário conectado presente também podem precisar chamar o Microsoft Graph sob sua própria identidade. Por exemplo, um aplicativo pode precisar usar a funcionalidade que exige privilégios mais elevados em uma organização do que o usuário conectado pode ter.  

Aplicativos que chamam o Microsoft Graph com sua própria identidade usam o [fluxo de concessão de credenciais de cliente](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) do OAuth 2.0 para obter tokens de acesso do Azure Active Directory. Este artigo descreve as etapas básicas para configurar um serviço e usar o fluxo de concessão de credenciais do cliente OAuth para obter um token de acesso.

## <a name="authentication-and-authorization-steps"></a>Etapas de autenticação e autorização

Siga estas etapas básicas para configurar um serviço e obter um token do ponto de extremidade da plataforma de identidade da Microsoft. Seu serviço pode usar o token para chamar o Microsoft Graph sob sua própria identidade.

1. Registre seu aplicativo.
2. Configure permissões para o Microsoft Graph em seu aplicativo.
3. Obtenha o consentimento do administrador.
4. Obtenha um token de acesso.
5. Use o token de acesso para chamar o Microsoft Graph.

## <a name="1-register-your-app"></a>1. Registre seu aplicativo

Para autenticar com o ponto de extremidade da plataforma de identidade da Microsoft, primeiro você deve registrar seu aplicativo no [Portal de Registro de Aplicativos do Azure](https://go.microsoft.com/fwlink/?linkid=2083908). Você pode usar uma conta da Microsoft ou uma conta corporativa ou de estudante para registrar seu aplicativo.

Para um serviço que chamará o Microsoft Graph com sua própria identidade, você precisa registrar seu aplicativo na plataforma Web e copiar os seguintes valores:

- A ID do aplicativo atribuída pelo portal de registro de aplicativo do Azure.
- Um segredo do cliente (aplicativo), que pode ser uma senha ou um par de chaves públicas/particulares (certificado).
- Uma URL de redirecionamento para seu serviço receber respostas do token.
- Uma URL de redirecionamento para seu serviço receber respostas de consentimento do administrador se seu aplicativo implementar a funcionalidade para solicitar o consentimento do administrador.  

Para saber como configurar um aplicativo usando o Portal de Registro de Aplicativos do Azure, confira [Registre seu aplicativo](./auth-register-app-v2.md).

Com o fluxo de concessão de credenciais do cliente OAuth 2.0, seu aplicativo é autenticado diretamente no ponto de extremidade `/token` da plataforma de identidade da Microsoft usando a ID do aplicativo atribuída pelo Azure Active Directory e o segredo do cliente que você cria usando o portal.

## <a name="2-configure-permissions-for-microsoft-graph"></a>2. Configure permissões para o Microsoft Graph

Microsoft Graph expõe **permissões de aplicativo** para aplicativos que chamam o Microsoft Graph sob sua própria identidade (o Microsoft Graph também expõe permissões delegadas para aplicativos que chamam o Microsoft Graph em nome de um usuário).

Você pré-configura as permissões de aplicativo de que seu aplicativo precisa ao registrar seu aplicativo. As permissões de aplicativo sempre exigem consentimento do administrador. Um administrador pode consentir com essas permissões usando o [portal do Azure](https://portal.azure.com) quando seu aplicativo estiver instalado em sua organização ou você pode fornecer uma experiência de inscrição em seu aplicativo por meio da qual os administradores podem consentir com as permissões configuradas. Depois que o consentimento do administrador é registrado pelo Azure Active Directory, seu aplicativo pode solicitar tokens sem precisar solicitar consentimento novamente. Para obter informações mais detalhadas sobre as permissões disponíveis com o Microsoft Graph, consulte a [Referência de permissões](./permissions-reference.md)

Para configurar permissões de aplicativo para seu aplicativo no [portal de registros de aplicativos do Azure](https://go.microsoft.com/fwlink/?linkid=2083908), na página de **permissões de API** de um aplicativo, escolha **Adicionar uma permissão**, selecione **Microsoft Graph** e, em seguida, escolha as permissões que seu aplicativo requer em **Permissões de aplicativo**.

A captura de tela a seguir mostra a caixa de diálogo **Selecionar Permissões** para permissões de aplicativo do Microsoft Graph.

:::image type="content" source="./images/auth-v2/v2-application-permissions.png" alt-text="Selecionar Janela de permissões para as permissões do aplicativo do Microsoft Graph." border="true":::

> [!IMPORTANT]
> 
> Configure o conjunto menos privilegiado de permissões exigido pelo aplicativo para melhorar sua segurança. Para obter mais informações, consulte [Aprimorar a segurança com o princípio de privilégios mínimos](/azure/active-directory/develop/secure-least-privileged-access).

## <a name="3-get-administrator-consent"></a>3. Obtenha o consentimento do administrador

Você pode confiar em um administrador para conceder as permissões que seu aplicativo precisa no [Portal do Azure](https://portal.azure.com). No entanto, muitas vezes, a melhor opção seria fornecer uma experiência de inscrição para administradores usando o ponto de extremidade `/adminconsent` da plataforma de identidade da Microsoft. 

> [!IMPORTANT]
> 
> Ao alterar as permissões configuradas, você também deve repetir o processo de consentimento do administrador. As alterações feitas no portal de registro de aplicativos não serão refletidas até que o consentimento tiver sido reaplicado pelo administrador do locatário.

### <a name="request"></a>Solicitação

```
// Line breaks are for legibility only.

GET https://login.microsoftonline.com/{tenant}/adminconsent
?client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&state=12345
&redirect_uri=https://localhost/myapp/permissions
```

| Parâmetro     | Condição   | Descrição 
|:--------------|:------------|:------------
| locatário        | Obrigatório    | O locatário de diretório do qual você deseja solicitar permissão. O valor pode estar no GUID ou em um formato de nome amigável. Se você não souber a qual locatário o usuário pertence e quiser permitir que ele entre com qualquer locatário, use `common`.
| client_id     | Obrigatório    | A ID do aplicativo que o [portal de registro de aplicativo do Azure](https://go.microsoft.com/fwlink/?linkid=2083908) atribuiu ao seu aplicativo.
| redirect_uri  | Obrigatório    | A URI de redirecionamento para a qual você deseja que a resposta seja enviada para o seu aplicativo manipular. Ela deve corresponder a uma das URIs de redirecionamento que você registrou no portal. Ela deve ser codificada em URL e pode ter segmentos de caminho adicionais.
| estado         | Recomendado | Um valor incluído na solicitação e que também será retornado na resposta do token. Pode ser uma cadeia de caracteres de qualquer conteúdo que você desejar. O estado é usado para codificar as informações sobre o estado do usuário no aplicativo antes da solicitação de autenticação ter ocorrido, como a página ou o modo de exibição em que ele estava.

### <a name="administrator-consent-experience"></a>Experiência de consentimento do administrador

Através de solicitações ao ponto de extremidade `/adminconsent`, o Azure Active Directory exige que apenas um administrador de locatário possa fazer logon para concluir a solicitação. Será solicitado ao administrador a aprovação de todas as permissões de aplicativo que você solicitar para seu aplicativo no portal de registro de aplicativos.

A captura de tela a seguir é um exemplo da caixa de diálogo de consentimento que o Azure Active Directory apresenta ao administrador:

:::image type="content" source="./images/auth-v2/admin-consent.png" alt-text="Caixa de diálogo do consentimento do administrador." border="true":::

### <a name="response"></a>Resposta

Se o administrador aprovar as permissões de seu aplicativo, a resposta bem-sucedida ficará assim:

```
// Line breaks are for legibility only.

GET https://localhost/myapp/permissions
?tenant=a8990e1f-ff32-408a-9f8e-78d3b9139b95&state=12345
&admin_consent=True
```

| Parâmetro     | Descrição
|:--------------|:------------
| locatário        | O locatário do diretório que concedeu as permissões de aplicativo solicitadas, no formato GUID.
| estado         | Um valor incluído na solicitação e que também será retornado na resposta do token. Pode ser uma cadeia de caracteres de qualquer conteúdo que você desejar. O estado é usado para codificar as informações sobre o estado do usuário no aplicativo antes da solicitação de autenticação ter ocorrido, como a página ou o modo de exibição em que ele estava.
| admin_consent | Definir como **true**.


> **Tente**: você pode tentar isso por conta própria colando a seguinte solicitação em um navegador. Se você entrar como administrador global de um locatário do Azure Active Directory, verá a caixa de diálogo de consentimento do administrador para o aplicativo. (Este será um aplicativo diferente daquele na captura de tela da caixa de diálogo de consentimento mostrada anteriormente.)
> 
> https://login.microsoftonline.com/common/adminconsent?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&state=12345&redirect_uri=https://localhost/myapp/permissions 

## <a name="4-get-an-access-token"></a>4. Obter um token de acesso

No fluxo de concessão de credenciais do cliente OAuth 2.0, você usa a ID do aplicativo e os valores secretos do cliente que salvou quando registrou seu aplicativo para solicitar um token de acesso diretamente do ponto de extremidade `/token`da plataforma de identidade da Microsoft.

Você especifica as permissões pré-configuradas passando `https://graph.microsoft.com/.default` como o valor para o parâmetro `scope` na solicitação de token. Confira a descrição do parâmetro `scope` na solicitação de token abaixo para obter detalhes.

### <a name="token-request"></a>Solicitação de token

Envie uma solicitação POST ao ponto de extremidade `/token` da plataforma de identidade para adquirir um token de acesso:

```
// Line breaks are for legibility only.

POST https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token HTTP/1.1
Host: login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=535fb089-9ff3-47b6-9bfb-4f1264799865
&scope=https%3A%2F%2Fgraph.microsoft.com%2F.default
&client_secret=qWgdYAmab0YSkuL1qKv5bPX
&grant_type=client_credentials
```

| Parâmetro     | Condição | Descrição 
|:--------------|:----------|:------------
| locatário        | Obrigatório  | O locatário de diretório do qual você deseja solicitar permissão. O valor pode estar no GUID ou em um formato de nome amigável.
| client_id     | Obrigatório  | A ID do aplicativo que o [portal de registro de aplicativo do Azure](https://go.microsoft.com/fwlink/?linkid=2083908) atribuído quando você registrou seu aplicativo.
| scope         | Obrigatório  | O valor passado para o `scope` parâmetro nesta solicitação deve ser o identificador do recurso (URI da ID do aplicativo) do recurso desejado, afixado com o sufixo `.default`. Para o Microsoft Graph, o valor é `https://graph.microsoft.com/.default`. Esse valor informa ao ponto de extremidade da plataforma de identidade da Microsoft para incluir no token de acesso todas as permissões no nível do aplicativo que o administrador consentiu.
| client_secret | Obrigatório  | O segredo do cliente que você gerou para seu aplicativo no portal de registro do aplicativo. Verifique se a URL está codificada.
| grant_type    | Obrigatório  | Deve ser `client_credentials`.

#### <a name="token-response"></a>Resposta do token

Uma resposta bem-sucedida tem esta aparência:

```json
{
  "token_type": "Bearer",
  "expires_in": 3599,
  "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik1uQ19WWmNBVGZNNXBP..."
}
```

| Parâmetro     | Descrição
|:--------------|:------------
| access_token  | O token de acesso solicitado. Seu aplicativo pode usar esse token em chamadas para o Microsoft Graph.
| token_type    | Indica o valor de tipo de token. O único tipo ao qual o Azure AD dá suporte é `bearer`.
| expires_in    | Por quanto tempo o token de acesso é válido (em segundos).

## <a name="5-use-the-access-token-to-call-microsoft-graph"></a>5. Use o token de acesso para chamar o Microsoft Graph

Após obter o token de acesso, você pode usá-lo para chamar o Microsoft Graph, incluindo-o no cabeçalho `Authorization` de uma solicitação. A solicitação a seguir obtém o perfil de um usuário específico. Seu aplicativo deve ter a permissão _User.Read.All_ para chamar essa API.

```
GET https://graph.microsoft.com/v1.0/users/12345678-73a6-4952-a53a-e9916737ff7f
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com
```
Uma resposta bem-sucedida terá a seguinte aparência (alguns cabeçalhos de resposta foram removidos):

```http
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
request-id: f45d08c0-6901-473a-90f5-7867287de97f
client-request-id: f45d08c0-6901-473a-90f5-7867287de97f
OData-Version: 4.0
Duration: 309.0273
Date: Wed, 26 Apr 2017 19:53:49 GMT
Content-Length: 407
```

```json
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

## <a name="supported-app-scenarios-and-resources"></a>Recursos e cenários de aplicativo com suporte

Os aplicativos que chamam o Microsoft Graph com sua própria identidade se enquadram em uma dessas categorias:

- [Serviços em segundo plano (daemons)](/azure/active-directory/develop/scenario-daemon-overview) que podem ser executados em um servidor sem um usuário conectado.
- Aplicativos que têm um usuário conectado, mas também chamam o Microsoft Graph com sua própria identidade. Por exemplo, para usar a funcionalidade que requer privilégios mais elevados do que o usuário tem.

Os aplicativos que chamam o Microsoft Graph com sua própria identidade usam a concessão de credenciais do cliente OAuth 2.0 para autenticar com o Azure Active Directory e obter um token. Para o ponto de extremidade da plataforma de identidade da Microsoft, você pode explorar ainda mais esse cenário com os seguintes recursos:

- Para ver um tratamento mais completo do Fluxo de Concessão de Credenciais do Cliente que também inclui respostas de erro, confira o artigo [Azure Active Directory v2.0 e o fluxo de Credenciais do Cliente OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).
- Para obter um exemplo que chama o Microsoft Graph a partir de um serviço, confira o [exemplo do daemon v2.0](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2) no GitHub.
- Para obter mais informações sobre bibliotecas de autenticação recomendadas da Microsoft e de terceiros, confira as [bibliotecas de autenticação da plataforma de identidade da Microsoft](/azure/active-directory/develop/reference-v2-libraries).

## <a name="endpoint-considerations"></a>Considerações sobre o ponto de extremidade

A Microsoft continua oferecendo suporte ao ponto de extremidade do Azure AD. Existem [várias diferenças](/azure/active-directory/develop/azure-ad-endpoint-comparison) entre a utilização do ponto de extremidade da plataforma de identidade da Microsoft e o ponto de extremidade do Azure AD. Durante o uso do ponto de extremidade do Azure AD:

- Se o aplicativo for multilocatário, você deve configurá-lo explicitamente para funcionar como multilocatário no [portal do Azure](https://portal.azure.com).
- Não há nenhum ponto de extremidade de consentimento do administrador. Em vez disso, seu aplicativo pode solicitar o consentimento do administrador durante o runtime adicionando o `prompt=admin_consent`parâmetro a uma solicitação de autorização. Para obter mais informações, consulte **Disparando a estrutura de consentimento do Azure Active Directory no runtime** em [Integrando aplicativos com o Azure Active Directory](/azure/active-directory/develop/active-directory-integrating-applications).
- Os parâmetros em solicitações de autorização e token são diferentes. Por exemplo, não há nenhum `scope` parâmetro em solicitações de ponto de extremidade do Azure Active Directory; em vez disso, o `resource` parâmetro é usado para especificar a URI do recurso (`resource=https://graph.microsoft.com`) para o qual a autorização (para consentimento do administrador) ou um token está sendo solicitado.

Você pode explorar esse cenário ainda mais com os seguintes recursos:

- Para saber mais sobre a plataforma de identidade da Microsoft com diferentes tipos de aplicativos, confira os links de **Introdução** na [documentação da plataforma de identidade da Microsoft](/azure/active-directory/develop/active-directory-developers-guide).
- Para saber mais sobre a MSAL (Biblioteca de Autenticação da Microsoft) e o middleware de servidor disponíveis para uso com o ponto de extremidade da plataforma de identidade da Microsoft, confira [Bibliotecas de Autenticação da Microsoft](/azure/active-directory/develop/active-directory-authentication-libraries).


## <a name="see-also"></a>Confira também

- [Escolher um provedor de autenticação do Microsoft Graph com base no cenário](/graph/sdks/choose-authentication-providers?tabs=CS)
- [Saiba como criar um aplicativo Web que chama o Microsoft Graph sob sua própria identidade](/azure/app-service/scenario-secure-app-access-microsoft-graph-as-app).
- Para exemplos de uso da plataforma de identidade da Microsoft para garantir diferentes tipos de aplicativos, confira [Exemplos de código da plataforma de identidade da Microsoft (ponto de extremidade v2.0)](/azure/active-directory/develop/sample-v2-code).
