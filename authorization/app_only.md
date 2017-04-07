# <a name="call-microsoft-graph-in-a-service-or-daemon-app"></a>Chamar o Microsoft Graph em um aplicativo de serviço ou daemon

Este artigo descreve as tarefas mínimas obrigatórias para conectar seu aplicativo de serviço ou daemon de locatário único ao Office 365 e chamar a API do Microsoft Graph.

> **Observação:** este tópico aborda o uso do Azure Active Directory como o provedor de autenticação do seu aplicativo. Para implementar um aplicativo de serviço ou daemon usando o ponto de extremidade do Azure AD v2.0, confira <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-client-creds/" target="_newtab">Protocolos da versão 2.0 – Fluxo de Credenciais do Cliente do OAuth 2.0</a>.

## <a name="register-the-application-in-azure-active-directory"></a>Registrar o aplicativo no Azure Active Directory

Antes de começar a trabalhar com o Office 365, você precisa registrar seu aplicativo no [portal do Azure](https://portal.azure.com). Lembre-se dos seguintes detalhes:

- Depois de registrar o aplicativo, configure as permissões de aplicativo exigidas pelo seu aplicativo de serviço ou daemon.
- Anote os valores a seguir no registro do seu aplicativo Azure. Você precisa desses valores para configurar o fluxo OAuth em seu aplicativo de serviço ou daemon:
    * ID do aplicativo (exclusiva para o seu aplicativo)
    * Chave do aplicativo ou segredo (exclusiva para o seu aplicativo)
    * O ponto de extremidade de token OAuth 2.0 de seu aplicativo
      * Encontre esse valor clicando em *Exibir Pontos de Extremidade* na parte inferior do Portal de Gerenciamento do Azure, na página do seu aplicativo. O ponto de extremidade terá a seguinte aparência: `https://login.microsoftonline.com/{tenantId}/oauth2/token`.

## <a name="request-an-access-token-from-the-token-issuing-endpoint"></a>Solicitar um token de acesso do ponto de extremidade de emissão do token

Diferentemente dos aplicativos clientes, o aplicativo de serviço ou daemon é incapaz de fazer um usuário entrar e autorizar seu aplicativo. Em vez disso, seu aplicativo tem que implementar o fluxo de concessão de credenciais de cliente OAuth 2.0, que permite que ele use suas próprias credenciais, sua ID do cliente e uma chave do aplicativo para se autenticar ao chamar o Microsoft Graph, em vez de representar um usuário. Para obter detalhes sobre o fluxo de autenticação, confira [Chamadas serviço a serviço usando as credenciais do cliente](https://msdn.microsoft.com/en-us/library/azure/dn645543.aspx).

Faça uma solicitação HTTP POST ao ponto de extremidade de emissão do token com os seguintes parâmetros, substituindo `<clientId>` e `<clientSecret>` pela ID do cliente e pela chave do aplicativo, respectivamente.

```http
POST https://login.microsoftonline.com/{tenantId}/oauth2/token HTTP/1.1
Content-Type: application/x-www-form-urlencoded

grant_type=client_credentials
&client_id=<clientId>
&client_secret=<clientSecret>
&resource=https://graph.microsoft.com
```

A resposta incluirá um token de acesso e informações sobre a expiração.

```json
{ 
  "token_type": "Bearer",
  "expires_in": "3599",
  "scope": "User.Read",
  "expires_on": "1449685363",
  "not_before": "1449681463",
  "resource": "https://graph.microsoft.com",
  "access_token": "<token>"
}
```

## <a name="use-the-access-token-in-a-request-to-the-microsoft-graph-api"></a>Usar o token de acesso em uma solicitação para a API do Microsoft Graph

Com um token de acesso, o aplicativo pode fazer solicitações autenticadas à API do Microsoft Graph. Seu aplicativo deve anexar o token de acesso ao cabeçalho **Authorization** de cada solicitação.

Por exemplo, um aplicativo de serviço ou daemon poderá recuperar todos os usuários de um locatário se tiver a permissão *Ler perfis completos de todos os usuários* selecionada no Portal de Gerenciamento do Azure. 

```http
GET https://graph.microsoft.com/v1.0/users
Authorization: Bearer <token>
```
