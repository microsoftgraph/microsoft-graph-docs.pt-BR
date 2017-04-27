
# <a name="microsoft-graph-app-authentication-using-azure-ad"></a>Autenticação do aplicativo Microsoft Graph usando o Azure AD

Este artigo apresenta uma visão detalhada de um exemplo de fluxo de autenticação e autorização para um aplicativo Microsoft Graph. Este exemplo usa o Azure Active Directory (Azure AD) como o provedor de autenticação e o <a href="https://msdn.microsoft.com/en-us/library/azure/dn645542.aspx" target="_newtab">Fluxo de Concessão de Código de Autorização</a> como fluxo de autenticação. Este exemplo mostrará como usar o Azure AD em um aplicativo Microsoft Graph para autenticar um usuário, obter um token de acesso e renovar um token de acesso usando um token de atualização.

Para fluxos de concessão de código, o processo de autenticação pode ser dividido em duas etapas básicas:

1. Solicitar um código de autorização
2. Usar o código de autorização para solicitar tokens de acesso e de atualização 

Você pode usar o token de atualização para adquirir um novo token de acesso quando o token de acesso atual expira.
 
##<a name="authenticate-a-user-and-get-app-authorized"></a>Autenticar um usuário e obter autorização para o aplicativo

A fim de obter autorização para o aplicativo, você deve autenticar o usuário primeiro. Para fazer isso, redirecione o usuário ao ponto de extremidade de autorização do Azure AD (Azure Active Directory) junto com as informações do seu aplicativo para entrar em sua conta corporativa ou de estudante. Depois que o usuário entrar e conceder as permissões solicitadas pelo aplicativo (se o usuário já não tiver feito isso), o aplicativo receberá um código de autorização obrigatório para adquirir um token de acesso OAuth.

> **Observação**:  Você pode fazer isso chamando métodos na [ADAL (Biblioteca de autenticação do Azure AD)](https://msdn.microsoft.com/en-us/library/azure/jj573266.aspx). Para saber mais sobre fluxo de autorização, confira [Fluxo de concessão de código de autorização](https://msdn.microsoft.com/en-us/library/azure/dn645542.aspx).

A autorização de um aplicativo começa com o envio de uma solicitação HTTPS GET usando a seguinte URL:
 
```GET https://login.microsoftonline.com/common/oauth2/authorize?response_type=code&redirect_uri=<uri>&client_id=<id>```

**Parâmetros de cadeia de caracteres de consulta obrigatórios**

| Nome do parâmetro  | Valor  | Descrição                                                                                            |
|:----------------|:-------|:-------------------------------------------------------------------------------------------------------|
| *client_id*     | string | A ID do cliente criada para o seu aplicativo. Esse é o valor **ID DO CLIENTE** do seu aplicativo definido no registro de aplicativo do locatário do Azure.                                                                  |
| *response_type* | string | Especifica o tipo de resposta solicitado. Em uma solicitação de concessão de código de autorização, o valor deve ser o código. |
| *redirect_uri*  | string | A URL de redirecionamento para a qual o navegador é enviado quando a autenticação é concluída.  Esse valor deve ser correspondente ao valor pré-configurado **URL DE RESPOSTA** do aplicativo.                        |
 


Veja a seguir um exemplo dessa solicitação implementada em um aplicativo em funcionamento:


```GET https://login.microsoftonline.com/common/oauth2/authorize?response_type=code&redirect_uri=http%3a%2f%2flocalhost:1339/auth/azureoauth/callback&client_id=8b8539cd-7b75-427f-bef1-4a6264fd4940``` 

Essa solicitação retornará uma resposta `200 OK` e apresentará a página de entrada da conta do Azure AD. 

Após o usuário entrar com credenciais válidas e conceder as permissões para o aplicativo, a página de logon enviará uma solicitação `POST` para o Azure. Se a solicitação for bem-sucedida, o Azure responderá com uma mensagem `302 Found` para encaminhar a chamada ao URI de redirecionamento do aplicativo, para que este receba o token de acesso obrigatório. O URI encaminhado, especificado no cabeçalho `Location` da resposta, corresponde à URL DE RESPOSTA do aplicativo com dois parâmetros de consulta anexados a ela: `code=...` e `session_state=...`. O exemplo abaixo mostra um trecho desse tipo de resposta: 

```no-highlight 
HTTP/1.1 302 Found
Cache-Control: no-cache, no-store
Pragma: no-cache
Content-Type: text/html; charset=utf-8
Expires: -1
Location: http://localhost:1339/auth/azureoauth/callback?code=AAABAAAAvPM...&session_state=a9556cd3-cae6-4bc9-bf51-672f7b79b7c6
Server: Microsoft-IIS/8.5
P3P: CP="DSP CUR OTPi IND OTRi ONL FIN"

..... 
```

Neste exemplo, a URL DE RESPOSTA do aplicativo é `http://localhost:1339/auth/azureoauth/callback`. Ao processar essa resposta, você deve extrair o valor do parâmetro `code` e usá-lo para adquirir os tokens de acesso e de atualização OAuth 2.0 iniciais (confira a próxima seção).

> **Observação:** a resposta `302 Found` acima é diferente da resposta `302 Found` obtida se você começou o processo de logon com a URL `https://login.windows.net/{tenantId}/oauth2/authorize?...`. Neste último, a resposta `302 Found` encaminha sua solicitação para `login.microsoftonline.com`.
 
<!---<a name="msg_get_app_authenticated"> </a> -->

##<a name="acquire-an-access-token"></a>Adquirir um token de acesso
Para acessar recursos do Microsoft Graph, seu aplicativo deve incluir um token de acesso OAuth 2.0 válido em cada solicitação HTTP. Você pode obter o token de acesso usando a seguinte solicitação POST:

```no-highlight 
POST https://login.microsoftonline.com/common/oauth2/token HTTP/1.1
content-type : application/x-www-form-urlencoded
content-length : 144
```
 
Essa solicitação requer uma carga de consulta codificada como URL nos seguintes formatos:
 
```no-highlight 
grant_type=authorization_code
&redirect_uri=<uri>
&client_id=<id>
&client_secret=<secret_key>
&code=<code>
&resource=https%3A%2F%2Fgraph.microsoft.com%2F
```

**Parâmetros de cadeia de caracteres de consulta obrigatórios**

| Nome do parâmetro  | Valor  | Descrição                                                                                            |
|:----------------|:-------|:-------------------------------------------------------------------------------------------------------|
| *client_id*     | string | A ID do cliente criada para o seu aplicativo.  |
| *client_secret*  | string | A chave criada para o aplicativo. Esse valor é o mesmo valor da seção **Chaves** da página de configuração do aplicativo no Portal de Gerenciamento do Azure|
| *redirect_uri*  | string | A URL de redirecionamento para a qual o navegador é enviado quando a autenticação é concluída.  |
| *código*  | string | O código de autorização. O valor do parâmetro de consulta `code` retornado da resposta à solicitação de autorização. |
| *recurso*   | string | O recurso que você deseja acessar. Para chamar a API do Microsoft Graph, defina esse valor de parâmetro como "https://graph.microsoft.com/".|

O trecho a seguir mostra um exemplo da carga de solicitação usada para adquirir o token de acesso OAuth 2.0 inicial:

```no-highlight  
grant_type=authorization_code&
redirect_uri=http%3A%2F%2Flocalhost%3A1339%2Fauth%2Fazureoauth%2Fcallback&
client_id=8b8539cd-7b75-427f-bef1-4a6264fd4940&client_secret=PJW3dznGfyNSm3rM9aHeXWGKsTMepKXT1Eqy45XXdU4%3D&
code=AAABAAAAvPM1KaPlrEqdFSBzjqfTGBLRVQc6BtQmJ_9DQZUg8Tb7TJgTmbTE7AHM93qB5EKc4Bf-bOgzt3mebAywK-09X1uBHwOluuqSWfd9LU2HHgZtxcZFIYI5UL7L1UEvhrJRvX2iHhfz9ZSRMZMVL55n_K79gCOxtSATeCUw52zPk5ZaQ87Y42SCLsRZN4Y_zddhD3mMpkObiHVT8HzfhBUiT0oX0e-Q439vkbZoKiq1HaqMR3IPHiCXDbPPH5u7a4NTe5xAhh-o2MUIe6s4Xqql86sv1-IwyroOJJMueGUarkfbgwqmYL9Tm-jWab8o-BAK_plVsN73GU8cXO8ts30wa2YmNR5ZxSkw8oiB4mSZwGzGQlch55DRnucDs0SZBgj5etGi3SeXv5jhKlDU2S0bAPnGxF3QAH0N_zBpfakETVlcsHKi714u-tn9da6aTPQsE0IYKTAYgxjTMei6zfRFvCZi-tKdFR6X9TvvmF2iPdGQGWKeLw8CMWUzU8VmOhiHc0aBKG6RaXAOTM067J_9WKYPxMopcytD2z8HVkL1QhggAA&
resource=https%3A%2F%2Fgraph.microsoft.com%2F
```

Quando essa solicitação é bem-sucedida, uma resposta `200 OK` é retornada. Um exemplo é mostrado da seguinte maneira:

```no-highlight  
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8
Expires: -1
Content-Length: 2978
Access-Control-Allow-Origin: *

{
    "token_type":"Bearer",
    "expires_in":"3599",
    "expires_on":"1426551729",
    "not_before":"1426547829",
    "resource":"https://graph.microsoft.com/",
    "access_token":"eyJ0eXAiOiJKV1QiLCJhb...",
    "refresh_token":"AAABAAAAvPM1KaPlrEqd...",
    "scope": "Calendar.ReadWrite Directory.Read.All Files.ReadWrite Group.ReadWrite.All Mail.ReadWrite Mail.Send User.ReadBasic.All",
    "id_token":"eyJ0eXAiOiJKV1QiLCJhbGci..."
}
```

 
O corpo da resposta é uma cadeia de caracteres de formato JSON que contém o token de acesso (`access_token`). Você precisa fornecer esse token às solicitações HTTP seguintes para acessar os recursos do Microsoft Graph. 

O valor da propriedade `scope` deve corresponder às permissões concedidas para o aplicativo durante o registro dele.

O token de acesso permanecerá válido no intervalo de tempo especificado (`3599` segundos no exemplo acima ou 1 hora) a contar do momento da emissão, como especificado na propriedade `expires_in`. O resultado também contém um token de atualização (`refresh_token`) que deve ser usado para renovar um token de acesso expirado ou prestes a expirar. 

Nos códigos de produção, seu aplicativo precisa observar a expiração desses tokens e renovar o token de acesso prestes a expirar antes que o token de atualização expire. 
-->

<!---<a name="msg_renew_access_token using refresh token"> </a> -->

##<a name="renew-expiring-access-token-using-refresh-token"></a>Renovar o token de acesso prestes a expirar usando o token de atualização
Para atualizar um token de acesso expirado, use uma solicitação POST semelhante ao seguinte exemplo (supondo que o token de atualização não tenha expirado):

```no-highlight  
POST https://login.microsoftonline.com/common/oauth2/token HTTP/1.1
Host: login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded
Content-Length: 897


grant_type=refresh_token
&redirect_uri=http%3A%2F%2Flocalhost%3A1339%2Fauth%2Fazureoauth%2Fcallback
&client_id=8b8539cd-7b75-427f-bef1-4a6264fd4940
&client_secret=PJW3dznGfyNSm3rM9aHeXWGKsTMepKXT1Eqy45XXdU4%3D
&refresh_token=AAABAAAAvPM1KaPlrEqdFSBzjqfTGM74--...
&resource=https%3A%2F%2Fgraph.microsoft.com%2F
```

**Parâmetros de cadeia de caracteres de consulta obrigatórios**

| Nome do parâmetro  | Valor  | Descrição                                                                                                                                         |
|:----------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| *client_id*     | string | A ID do cliente criada para o aplicativo.  |
| *redirect_uri*  | string | A URL de redirecionamento para a qual o navegador é enviado quando a autenticação é concluída. Isso deve corresponder ao valor *redirect_uri* usado na primeira solicitação. |
| *client_secret* | string | Um dos valores de Chaves criados para o aplicativo.                                                                                                     |
| *refresh_token* | string | O token de atualização recebido anteriormente.    |
| *recurso*      | string | O recurso que você deseja acessar.|

Observe que essa solicitação é quase idêntica à solicitação de aquisição de token inicial. Há duas diferenças na carga de solicitação, isto é, o parâmetro `grant_type` agora tem o valor `refresh_token` (em vez de `code`).
 
A resposta bem-sucedida retorna a carga de uma cadeia de caracteres JSON semelhante ao seguinte:

```no-highlight 
{
    "token_type":"Bearer",
    "expires_in":"3600",
    "expires_on":"1426561346",
    "not_before":"1426557446",
    "resource":"https://graph.microsoft.com/",
    "access_token":"eyJ0eXAiOiJKV1QiLCJhbGciOi...", 
    "refresh_token":"AAABAAAAvPM1KaPlrEqdFSBzj...",
   "scope":"Graph.Read",
    "pwd_exp":"6553342",
    "pwd_url":"https://portal.microsoftonline.com/ChangePassword.aspx"
}
```
 
Tirando a falta da propriedade `id_token`, esse corpo de resposta possui sintaxe e semântica idênticas às da resposta de aquisição do token inicial. Os tempos de vida dos valores `access_token` e `refresh_token` retornados recentemente são prorrogados. O novo horário de expiração do token de acesso é o número de segundos, especificado no valor `expires_in`, a partir do momento em que a solicitação de atualização de token foi enviada com êxito. 
 
Quando o token de atualização expira, você não pode renovar os tokens de acesso expirados usando a solicitação POST que acabou de ser descrita. Em vez disso, você deve reiniciar o processo de autenticação e autorização de aplicativo.



