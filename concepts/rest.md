# <a name="get-started-with-microsoft-graph-and-rest"></a><span data-ttu-id="a6d97-101">Introdução ao Microsoft Graph e REST</span><span class="sxs-lookup"><span data-stu-id="a6d97-101">Get started with Microsoft Graph and REST</span></span>

<span data-ttu-id="a6d97-p101">Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph usando chamadas REST. Ele descreve a sequência de solicitações e respostas que um aplicativo usa para autenticar e recuperar as mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph using REST calls. It describes the sequence of requests and responses that an app uses to authenticate and retrieve email messages.</span></span>

<span data-ttu-id="a6d97-104">Primeiro, você precisa registrar seu aplicativo com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a6d97-104">First, you need register your app with Azure Active Directory (Azure AD).</span></span> 

## <a name="register-the-application"></a><span data-ttu-id="a6d97-105">Registrar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6d97-105">Register the application</span></span>

<span data-ttu-id="a6d97-106">Há duas opções para registrar o aplicativo com o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a6d97-106">There are currently two options to register your app with Azure AD.</span></span>

  - <span data-ttu-id="a6d97-107">Registre um aplicativo para usar o ponto de extremidade do Azure AD v2.0 que funciona para identidades pessoais (Microsoft) e contas corporativas ou de estudante (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a6d97-107">Register an app to use the Azure AD v2.0 endpoint that works for both personal (Microsoft) identities and work and school (Azure AD) accounts.</span></span>
  - <span data-ttu-id="a6d97-108">Registre um aplicativo para usar o ponto de extremidade do Azure AD compatível apenas com contas corporativas ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="a6d97-108">Register an app to use the Azure AD endpoint that supports work and school accounts only.</span></span>

<span data-ttu-id="a6d97-p102">Este artigo pressupõe que haja um registro do v2.0, então você registrará seu aplicativo no [Portal de registro do aplicativo](https://apps.dev.microsoft.com/). Siga as instruções em [Registrar seu aplicativo Microsoft Graph com o ponto de extremidade do Azure AD v2.0](../concepts/auth_register_app_v2.md) para registrar seu aplicativo. Para obter informações sobre como usar o ponto de extremidade do Azure AD, confira [Autenticar usando o Azure AD](../concepts/auth_v2_user.md).</span><span class="sxs-lookup"><span data-stu-id="a6d97-p102">This article assumes a v2.0 registration, so you'll register your app on the [Application Registration Portal](https://apps.dev.microsoft.com/). Follow the instructions in [Register your Microsoft Graph application with the Azure AD v2.0 endpoint](../concepts/auth_register_app_v2.md) to register your app. For information about using the Azure AD endpoint, see [Authenticate using Azure AD](../concepts/auth_v2_user.md).</span></span>

> <span data-ttu-id="a6d97-p103">Algumas limitações aplicam-se ao usar o ponto de extremidade do v2.0. Para decidir se ele é ideal para você, confira [Devo usar o ponto de extremidade do v2.0?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)</span><span class="sxs-lookup"><span data-stu-id="a6d97-p103">Some limitations apply when using the v2.0 endpoint. To decide if it's right for you, see [Should I use the v2.0 endpoint?](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-limitations/)</span></span>

## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="a6d97-114">Autenticar o usuário e obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="a6d97-114">Authenticate the user and get an access token</span></span>

<span data-ttu-id="a6d97-p104">O aplicativo descrito neste artigo implementa o [fluxo de Concessão de Código de Autorização](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/) para obter os tokens de acesso do ponto de extremidade do Azure AD v2.0, seguindo os [protocolos OAuth 2.0](http://tools.ietf.org/html/rfc6749) padrão. Para obter um guia completo para os fluxos compatíveis com o ponto de extremidade do Azure AD v2.0, confira [Tipos do ponto de extremidade do v2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/).</span><span class="sxs-lookup"><span data-stu-id="a6d97-p104">The app described in this article implements the [Authorization Code Grant flow](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-code/) to get access tokens from the Azure AD v2.0 endpoint, following standard [OAuth 2.0 protocols](http://tools.ietf.org/html/rfc6749). For a complete guide to the flows supported in the Azure AD v2.0 endpoint see [Types of the v2.0 endpoint](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-flows/).</span></span>

<span data-ttu-id="a6d97-117">Com o fluxo de Concessão de Código de Autorização, primeiro você recebe um código de autorização e, em seguida, troca o código por um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="a6d97-117">With the Authorization Code Grant flow, first you get an authorization code and then you exchange the code for an access token.</span></span>

### <a name="getting-an-authorization-code"></a><span data-ttu-id="a6d97-118">Obtendo um código de autorização</span><span class="sxs-lookup"><span data-stu-id="a6d97-118">Getting an authorization code</span></span>

<span data-ttu-id="a6d97-p105">A primeira etapa no fluxo de concessão de código de autorização é obter um código de autorização. O código é retornado ao aplicativo pelo servidor autorização quando o usuário se conecta e permite as permissões que o aplicativo solicitou.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p105">The first step in the Authorization Code Grant flow is to get an authorization code. The code is returned to the app by the authorization server when the user signs in and consents to the permissions requested by the app.</span></span>

<span data-ttu-id="a6d97-p106">Você solicita um código de autorização enviando uma solicitação GET para o ponto de extremidade do Azure AD v2.0. Essa URL deve ser aberta em um navegador para que o usuário possa entrar e dar permissão.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p106">You request an authorization code by sending a GET request to the Azure AD v2.0 endpoint. This URL must be opened in a browser so that the user can sign in and provide consent.</span></span>

#### <a name="construct-the-request"></a><span data-ttu-id="a6d97-123">Construir a solicitação</span><span class="sxs-lookup"><span data-stu-id="a6d97-123">Construct the request</span></span>

<span data-ttu-id="a6d97-124">1) Comece com a URL base:</span><span class="sxs-lookup"><span data-stu-id="a6d97-124">1- Start with the base URL:</span></span>

```
https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
```

<span data-ttu-id="a6d97-p107">O segmento *locatário* nos controles de caminho que pode entrar no aplicativo. Os valores permitidos são *comuns*, *organizações*, *consumidores* e os identificadores de locatários. Para mais informações, confira [Pontos de extremidade de protocolo](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints).</span><span class="sxs-lookup"><span data-stu-id="a6d97-p107">The *tenant* segment in the path controls who can sign into the application. Allowed values are *common*, *organizations*, *consumers*, and tenant identifiers. For more information, see [Protocol endpoints](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/#endpoints).</span></span>

<span data-ttu-id="a6d97-p108">2) Acrescente parâmetros de consulta para a URL base. Eles são usados para identificar o aplicativo, as permissões solicitadas e outras informações de solicitação de autenticação. A tabela a seguir descreve alguns dos parâmetros comuns.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p108">2- Append query parameters to the base URL. These are used to identify the app, the requested permissions, and other auth request information. The following table describes some common parameters.</span></span>

| <span data-ttu-id="a6d97-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a6d97-131">Parameter</span></span> | <span data-ttu-id="a6d97-132">Descrições</span><span class="sxs-lookup"><span data-stu-id="a6d97-132">Descriptions</span></span> |
|:------|:------|
| <span data-ttu-id="a6d97-133">client_id</span><span class="sxs-lookup"><span data-stu-id="a6d97-133">client_id</span></span> | <span data-ttu-id="a6d97-p109">A ID do aplicativo gerada durante o registro do aplicativo. Isso permite que o Azure AD saiba qual aplicativo está solicitando o logon.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p109">The app ID generated by registering the app. This lets Azure AD know which app is requesting the logon.</span></span> |
| <span data-ttu-id="a6d97-136">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="a6d97-136">redirect_uri</span></span> | <span data-ttu-id="a6d97-p110">O local para o qual o Azure será redirecionado depois de o usuário conceder permissão para o aplicativo. Esse valor deve corresponder ao valor **URI de redirecionamento** usado ao registrar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p110">The location that Azure will redirect to after the user has granted consent to the app. This value must correspond to the value of **Redirect URI** used when registering the app.</span></span> |
| <span data-ttu-id="a6d97-139">response_type</span><span class="sxs-lookup"><span data-stu-id="a6d97-139">response_type</span></span> | <span data-ttu-id="a6d97-p111">O tipo de resposta que o aplicativo está esperando. Esse valor é `code` para o fluxo de Concessão de Código de Autorização.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p111">The type of response the app is expecting. This value is `code` for the Authorization Code Grant flow.</span></span> |
| <span data-ttu-id="a6d97-142">escopo</span><span class="sxs-lookup"><span data-stu-id="a6d97-142">scope</span></span> | <span data-ttu-id="a6d97-p112">Uma lista de escopos separados por espaços dos [escopos de permissão do Microsoft Graph](./permissions_reference.md) que o aplicativo está solicitando. Você também pode especificar [Escopos do OpenId Connect](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes) para o [logon único](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/).</span><span class="sxs-lookup"><span data-stu-id="a6d97-p112">A space-separated list of [Microsoft Graph permission scopes](./permissions_reference.md) that the app is requesting. You can also specify [OpenId Connect scopes](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#openid-connect-scopes) for [single sign-on](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oidc/).</span></span>  |
| <span data-ttu-id="a6d97-145">state</span><span class="sxs-lookup"><span data-stu-id="a6d97-145">state</span></span> | <span data-ttu-id="a6d97-146">Um valor incluído na solicitação que também será retornado na resposta de token, usado para validação.</span><span class="sxs-lookup"><span data-stu-id="a6d97-146">A value included in the request that will also be returned in the token response, used for validation.</span></span> |

<span data-ttu-id="a6d97-147">Por exemplo, a URL de solicitação para nosso aplicativo que requer acesso de leitura para os emails teria a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="a6d97-147">For example, the request URL for an application that requires read access to mail might look like the following.</span></span>

```
GET https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=<app ID>&redirect_uri=http%3A%2F%2Flocalhost/myapp%2F&response_type=code&state=1234&scope=mail.read
```

<span data-ttu-id="a6d97-p113">3) Redirecione o usuário para a URL de logon. O usuário verá uma tela de entrada exibindo o nome do aplicativo. Depois de entrar, o usuário verá uma lista das permissões que o aplicativo exige e será solicitado a permiti-las ou negá-las. Se o usuário consentir, o navegador redirecionará para a URI de redirecionamento com o código de autorização e o estado na cadeia de caracteres de consulta, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p113">3- Redirect the user to the logon URL. The user is presented with a sign in screen that displays the name of the app. After signing in, the user is presented with the list of the permissions the app requires and prompted to allow or deny. If the user consents, the browser redirects to the redirect URI with the authorization code and state in the query string, as shown in the following example.</span></span>

```
http://localhost/myapp/?code=AwABAAAA...cZZ6IgAA&state=1234
```

<span data-ttu-id="a6d97-152">A próxima etapa é trocar o código de autorização retornado por um token de acesso</span><span class="sxs-lookup"><span data-stu-id="a6d97-152">The next step is to exchange the authorization code returned for an access token.</span></span>

### <a name="getting-an-access-token"></a><span data-ttu-id="a6d97-153">Obtendo um token de acesso</span><span class="sxs-lookup"><span data-stu-id="a6d97-153">Getting an access token</span></span>

<span data-ttu-id="a6d97-154">Para obter um token de acesso, o aplicativo posta parâmetros codificados em formulário na URL de solicitação de token (por exemplo, `https://login.microsoftonline.com/common/oauth2/v2.0/token`) com os parâmetros a seguir.</span><span class="sxs-lookup"><span data-stu-id="a6d97-154">To get an access token, the app posts form-encoded parameters to the token request URL (for example, `https://login.microsoftonline.com/common/oauth2/v2.0/token`) with the following parameters.</span></span>

| <span data-ttu-id="a6d97-155">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a6d97-155">Parameter</span></span> | <span data-ttu-id="a6d97-156">Descrições</span><span class="sxs-lookup"><span data-stu-id="a6d97-156">Descriptions</span></span> |
|:------|:------|
| <span data-ttu-id="a6d97-157">client_id</span><span class="sxs-lookup"><span data-stu-id="a6d97-157">client_id</span></span> | <span data-ttu-id="a6d97-158">A ID do aplicativo gerada durante o registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6d97-158">The app ID generated by registering the app.</span></span> |
| <span data-ttu-id="a6d97-159">client_secret</span><span class="sxs-lookup"><span data-stu-id="a6d97-159">client_secret</span></span> | <span data-ttu-id="a6d97-160">O segredo de aplicativo gerado ao registrar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6d97-160">The app secret generated when registering the app.</span></span> |
| <span data-ttu-id="a6d97-161">código</span><span class="sxs-lookup"><span data-stu-id="a6d97-161">code</span></span> | <span data-ttu-id="a6d97-162">O código de autorização obtido na etapa anterior.</span><span class="sxs-lookup"><span data-stu-id="a6d97-162">The authorization code obtained in the prior step.</span></span> |
| <span data-ttu-id="a6d97-163">redirect_uri</span><span class="sxs-lookup"><span data-stu-id="a6d97-163">redirect_uri</span></span> | <span data-ttu-id="a6d97-164">Esse valor deve ser igual ao valor usado na solicitação de código de autorização.</span><span class="sxs-lookup"><span data-stu-id="a6d97-164">This value must be the same as the value used in the authorization code request.</span></span> |
| <span data-ttu-id="a6d97-165">grant_type</span><span class="sxs-lookup"><span data-stu-id="a6d97-165">grant_type</span></span> | <span data-ttu-id="a6d97-p114">O tipo de concessão que o aplicativo está usando. Esse valor é `code` para o fluxo de Concessão de Código de Autorização.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p114">The type of grant the app is using. This value is `code` for the Authorization Code Grant flow.</span></span> |
| <span data-ttu-id="a6d97-168">escopo</span><span class="sxs-lookup"><span data-stu-id="a6d97-168">scope</span></span> | <span data-ttu-id="a6d97-169">Uma lista de escopos separados por espaços dos [escopos de permissão do Microsoft Graph](./permissions_reference.md) que o aplicativo está solicitando.</span><span class="sxs-lookup"><span data-stu-id="a6d97-169">A space-separated list of [Microsoft Graph permission scopes](./permissions_reference.md) that the app is requesting.</span></span> |

<span data-ttu-id="a6d97-170">A URL de solicitação de nosso aplicativo, usando o código da etapa anterior, teria a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="a6d97-170">The request URL for our application, using the code from the previous step, looks like the following.</span></span>

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

<span data-ttu-id="a6d97-171">O servidor responde com uma carga JSON que inclui o token de acesso.</span><span class="sxs-lookup"><span data-stu-id="a6d97-171">The server responds with a JSON payload which includes the access token.</span></span>

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

<span data-ttu-id="a6d97-p115">O token de acesso é encontrado no campo `access_token` da carga JSON. O aplicativo usa esse valor para definir o cabeçalho Authorization ao fazer chamadas REST à API.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p115">The access token is found in the `access_token` field of the JSON payload. The app uses this value to set the Authorization header when making REST calls to the API.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="a6d97-174">Chamar o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a6d97-174">Call Microsoft Graph</span></span>

<span data-ttu-id="a6d97-p116">Depois que o aplicativo tem um token de acesso, ele está pronto para chamar o Microsoft Graph. Como esse aplicativo de exemplo está recuperando mensagens, ele usará uma solicitação HTTP GET para o ponto de extremidade `https://graph.microsoft.com/v1.0/me/messages`.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p116">After the app has an access token, it's ready to call Microsoft Graph. Because this sample app is retrieving messages, it will use an HTTP GET request to the `https://graph.microsoft.com/v1.0/me/messages` endpoint.</span></span>

### <a name="refine-the-request"></a><span data-ttu-id="a6d97-177">Refinar a solicitação</span><span class="sxs-lookup"><span data-stu-id="a6d97-177">Refine the request</span></span>

<span data-ttu-id="a6d97-p117">Os aplicativos podem controlar o comportamento de solicitações GET, usando parâmetros de consulta OData. Recomendamos que os aplicativos usem esses parâmetros para limitar o número de resultados retornados e limitar os campos retornados para cada item.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p117">Apps can control the behavior of GET requests by using OData query parameters. We recommend that apps use these parameters to limit the number of results that are returned and to limit the fields that are returned for each item.</span></span> 

<span data-ttu-id="a6d97-p118">Este aplicativo de exemplo exibirá mensagens em uma tabela que mostra o assunto, o remetente e a data e hora em que a mensagem foi recebida. A tabela exibe um máximo de 25 linhas e está classificada de modo que a mensagem recebida mais recentemente esteja na parte superior. O aplicativo usa os parâmetros de consulta a seguir para obter esses resultados.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p118">This sample app will display messages in a table that shows the subject, sender, and the date and time the message was received. The table displays a maximum of 25 rows and is sorted so that the most recently received message is at the top. The app uses the following query parameters to get these results.</span></span>

- <span data-ttu-id="a6d97-183">`$select` - Especifica apenas os campos `subject`, `sender` e `dateTimeReceived`.</span><span class="sxs-lookup"><span data-stu-id="a6d97-183">`$select` - Specifies only the `subject`, `sender`, and `dateTimeReceived` fields.</span></span>
- <span data-ttu-id="a6d97-184">`$top` - Especifica um máximo de 25 itens.</span><span class="sxs-lookup"><span data-stu-id="a6d97-184">`$top` - Specifies a maximum of 25 items.</span></span>
- <span data-ttu-id="a6d97-185">`$orderby` - Classifica os resultados pelo campo `dateTimeReceived`.</span><span class="sxs-lookup"><span data-stu-id="a6d97-185">`$orderby` - Sorts the results by the `dateTimeReceived` field.</span></span>

<span data-ttu-id="a6d97-186">Isso resulta na solicitação a seguir.</span><span class="sxs-lookup"><span data-stu-id="a6d97-186">This results in the following request.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

<span data-ttu-id="a6d97-p119">Agora que você viu como fazer chamadas ao Microsoft Graph, pode usar a referência de API para construir outros tipos de chamada que seu aplicativo tenha que fazer. No entanto, tenha em mente que seu aplicativo precisa ter as permissões apropriadas configuradas no registro de aplicativo para as chamadas feitas.</span><span class="sxs-lookup"><span data-stu-id="a6d97-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a6d97-189">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a6d97-189">Next steps</span></span>
- <span data-ttu-id="a6d97-190">Experimente mais da API REST usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="a6d97-190">Try out more of the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="a6d97-191">Ver também</span><span class="sxs-lookup"><span data-stu-id="a6d97-191">See also</span></span>
- [<span data-ttu-id="a6d97-192">Protocolos do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="a6d97-192">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="a6d97-193">Tokens do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="a6d97-193">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
