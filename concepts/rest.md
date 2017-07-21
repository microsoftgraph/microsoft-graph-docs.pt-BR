# <a name="get-started-with-microsoft-graph-and-rest"></a>Introdução ao Microsoft Graph e REST

Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph usando chamadas REST. Ele descreve a sequência de solicitações e respostas que um aplicativo usa para autenticar e recuperar as mensagens de email.

Primeiro, você precisa registrar seu aplicativo com o Azure Active Directory (Azure AD). 

## <a name="register-the-application"></a>Registrar o aplicativo

Há duas opções para registrar o aplicativo com o Azure AD.

  - Registre um aplicativo para usar o ponto de extremidade do Azure AD v2.0 que funciona para identidades pessoais (Microsoft) e contas corporativas ou de estudante (Azure AD).
  - Registre um aplicativo para usar o ponto de extremidade do Azure AD compatível apenas com contas corporativas ou de estudante.

Este artigo pressupõe que haja um registro do v2.0, então você registrará seu aplicativo no [Portal de registro do aplicativo](https://apps.dev.microsoft.com/). Siga as instruções em [Registrar seu aplicativo Microsoft Graph com o ponto de extremidade do Azure AD v2.0](../concepts/auth_register_app_v2.md) para registrar seu aplicativo. Para obter informações sobre como usar o ponto de extremidade do Azure AD, confira [Autenticar usando o Azure AD](../concepts/auth_v2_user.md).

> Algumas limitações aplicam-se ao usar o ponto de extremidade do v2.0. Para decidir se ele é ideal para você, confira [Devo usar o ponto de extremidade do v2.0?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)

## <a name="authenticate-the-user-and-get-an-access-token"></a>Autenticar o usuário e obter um token de acesso

O aplicativo descrito neste artigo implementa o [fluxo de Concessão de Código de Autorização](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/) para obter os tokens de acesso do ponto de extremidade do Azure AD v2.0, seguindo os [protocolos OAuth 2.0](http://tools.ietf.org/html/rfc6749) padrão. Para obter um guia completo para os fluxos compatíveis com o ponto de extremidade do Azure AD v2.0, confira [Tipos do ponto de extremidade do v2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/).

Com o fluxo de Concessão de Código de Autorização, primeiro você recebe um código de autorização e, em seguida, troca o código por um token de acesso.

### <a name="getting-an-authorization-code"></a>Obtendo um código de autorização

A primeira etapa no fluxo de concessão de código de autorização é obter um código de autorização. O código é retornado ao aplicativo pelo servidor autorização quando o usuário se conecta e permite as permissões que o aplicativo solicitou.

Você solicita um código de autorização enviando uma solicitação GET para o ponto de extremidade do Azure AD v2.0. Essa URL deve ser aberta em um navegador para que o usuário possa entrar e dar permissão.

#### <a name="construct-the-request"></a>Construir a solicitação

1) Comece com a URL base:

```
https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
```

O segmento *locatário* nos controles de caminho que pode entrar no aplicativo. Os valores permitidos são *comuns*, *organizações*, *consumidores* e os identificadores de locatários. Para mais informações, confira [Pontos de extremidade de protocolo](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints).

2) Acrescente parâmetros de consulta para a URL base. Eles são usados para identificar o aplicativo, as permissões solicitadas e outras informações de solicitação de autenticação. A tabela a seguir descreve alguns dos parâmetros comuns.

| Parâmetro | Descrições |
|:------|:------|
| client_id | A ID do aplicativo gerada durante o registro do aplicativo. Isso permite que o Azure AD saiba qual aplicativo está solicitando o logon. |
| redirect_uri | O local para o qual o Azure será redirecionado depois de o usuário conceder permissão para o aplicativo. Esse valor deve corresponder ao valor **URI de redirecionamento** usado ao registrar o aplicativo. |
| response_type | O tipo de resposta que o aplicativo está esperando. Esse valor é `code` para o fluxo de Concessão de Código de Autorização. |
| escopo | Uma lista de escopos separados por espaços dos [escopos de permissão do Microsoft Graph](./permissions_reference.md) que o aplicativo está solicitando. Você também pode especificar [Escopos do OpenId Connect](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes) para o [logon único](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/).  |
| state | Um valor incluído na solicitação que também será retornado na resposta de token, usado para validação. |

Por exemplo, a URL de solicitação para nosso aplicativo que requer acesso de leitura para os emails teria a seguinte aparência:

```
GET https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=<app ID>&redirect_uri=http%3A%2F%2Flocalhost/myapp%2F&response_type=code&state=1234&scope=mail.read
```

3) Redirecione o usuário para a URL de logon. O usuário verá uma tela de entrada exibindo o nome do aplicativo. Depois de entrar, o usuário verá uma lista das permissões que o aplicativo exige e será solicitado a permiti-las ou negá-las. Se o usuário consentir, o navegador redirecionará para a URI de redirecionamento com o código de autorização e o estado na cadeia de caracteres de consulta, conforme mostrado no exemplo a seguir.

```
http://localhost/myapp/?code=AwABAAAA...cZZ6IgAA&state=1234
```

A próxima etapa é trocar o código de autorização retornado por um token de acesso

### <a name="getting-an-access-token"></a>Obtendo um token de acesso

Para obter um token de acesso, o aplicativo posta parâmetros codificados em formulário na URL de solicitação de token (por exemplo, `https://login.microsoftonline.com/common/oauth2/v2.0/token`) com os parâmetros a seguir.

| Parâmetro | Descrições |
|:------|:------|
| client_id | A ID do aplicativo gerada durante o registro do aplicativo. |
| client_secret | O segredo de aplicativo gerado ao registrar o aplicativo. |
| código | O código de autorização obtido na etapa anterior. |
| redirect_uri | Esse valor deve ser igual ao valor usado na solicitação de código de autorização. |
| grant_type | O tipo de concessão que o aplicativo está usando. Esse valor é `code` para o fluxo de Concessão de Código de Autorização. |
| escopo | Uma lista de escopos separados por espaços dos [escopos de permissão do Microsoft Graph](./permissions_reference.md) que o aplicativo está solicitando. |

A URL de solicitação de nosso aplicativo, usando o código da etapa anterior, teria a seguinte aparência.

```
POST https://login.microsoftonline.com/common/oauth2/v2.0/token
Content-Type: application/x-www-form-urlencoded

{
  grant_type=authorization_code
  &code=AwABAAAA...cZZ6IgAA
  &redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
  &resource=https%3A%2F%2Fgraph.microsoft.com%2F
  &scope=mail.read
  &client\_id=<app ID>
  &client\_secret=<app SECRET>
}
```

O servidor responde com uma carga JSON que inclui o token de acesso.

```
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

{
  "token_type":"Bearer",
  "expires_in":"3600",
  "access_token":"eyJ0eXAi...b66LoPVA",
  "scope":"https://graph.microsoft.com/mail.read",
  ...
}
```

O token de acesso é encontrado no campo `access_token` da carga JSON. O aplicativo usa esse valor para definir o cabeçalho Authorization ao fazer chamadas REST à API.

## <a name="call-microsoft-graph"></a>Chamar o Microsoft Graph

Depois que o aplicativo tem um token de acesso, ele está pronto para chamar o Microsoft Graph. Como esse aplicativo de exemplo está recuperando mensagens, ele usará uma solicitação HTTP GET para o ponto de extremidade `https://graph.microsoft.com/v1.0/me/messages`.

### <a name="refine-the-request"></a>Refinar a solicitação

Os aplicativos podem controlar o comportamento de solicitações GET, usando parâmetros de consulta OData. Recomendamos que os aplicativos usem esses parâmetros para limitar o número de resultados retornados e limitar os campos retornados para cada item. 

Este aplicativo de exemplo exibirá mensagens em uma tabela que mostra o assunto, o remetente e a data e hora em que a mensagem foi recebida. A tabela exibe um máximo de 25 linhas e está classificada de modo que a mensagem recebida mais recentemente esteja na parte superior. O aplicativo usa os parâmetros de consulta a seguir para obter esses resultados.

- `$select` - Especifica apenas os campos `subject`, `sender` e `dateTimeReceived`.
- `$top` - Especifica um máximo de 25 itens.
- `$orderby` - Classifica os resultados pelo campo `dateTimeReceived`.

Isso resulta na solicitação a seguir.

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

Agora que você viu como fazer chamadas ao Microsoft Graph, pode usar a referência de API para construir outros tipos de chamada que seu aplicativo tenha que fazer. No entanto, tenha em mente que seu aplicativo precisa ter as permissões apropriadas configuradas no registro de aplicativo para as chamadas feitas.

## <a name="next-steps"></a>Próximas etapas
- Experimente mais da API REST usando o [Explorador do Graph](https://graph.microsoft.io/graph-explorer).

## <a name="see-also"></a>Ver também
- [Obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [Obter acesso em nome de um usuário](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [Obter acesso sem um usuário](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)
