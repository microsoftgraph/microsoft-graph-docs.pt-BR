# <a name="get-started-with-microsoft-graph-in-a-python-app"></a>Introdução ao Microsoft Graph em um aplicativo Python 

Este artigo descreve as tarefas obrigatórias para obter um token de acesso do Azure AD e chamar o Microsoft Graph. Ele orientará você em relação ao [Exemplo de conexão com Microsoft Graph para Python](https://github.com/microsoftgraph/python3-connect-rest-sample) e explica os principais conceitos que você implementa para utilizar a API do Microsoft Graph. O artigo descreve como acessar o Microsoft Graph usando chamadas diretas REST.

![Captura de tela do exemplo de Connect do Python do Office 365](./images/web-screenshot.png)

##  <a name="prerequisites"></a>Pré-requisitos

* [Python 3.5.2](https://www.python.org/downloads/)
* [Flask-OAuthlib](https://github.com/lepture/flask-oauthlib)
* [Flask-Script 0.4](http://flask-script.readthedocs.io/en/latest/)
* Uma [Conta da Microsoft](https://www.outlook.com/) ou uma [Conta do Office 365 para empresas](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)
* O [Exemplo de Connect do Microsoft Graph para Python](https://github.com/microsoftgraph/python3-connect-rest-sample)

## <a name="register-the-application-in-azure-active-directory"></a>Registrar o aplicativo no Azure Active Directory

Primeiro, você precisa registrar seu aplicativo e definir permissões para usar o Microsoft Graph. Isso permite que os usuários entrem no aplicativo com contas corporativas ou de estudante.

## <a name="register-the-application"></a>Registrar o aplicativo

Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e a senha que você usará para configurar o aplicativo para autenticação.

1. Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.

2. Escolha **Adicionar um aplicativo**.

3. Insira um nome para o aplicativo e escolha **Criar aplicativo**.

    A página de registro é exibida, listando as propriedades do seu aplicativo.

4. Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo.

5. Em **Segredos do Aplicativo**, escolha **Gerar Nova Senha**. Copie o segredo do aplicativo da caixa de diálogo **Nova senha gerada**.

    Você usará a ID do aplicativo e o segredo do aplicativo para configurar o aplicativo.

6. Em **Plataformas**, escolha **Adicionar plataforma** > **Web**.

7. Não deixe de marcar a caixa de diálogo **Permitir Fluxo Implícito** e insira *http://localhost:5000/login/authorized* como o URI de Redirecionamento.

    A opção **Permitir Fluxo Implícito** habilita o fluxo híbrido do OpenID Connect. Durante a autenticação, isso permite que o aplicativo receba informações de entrada (o **id_token**) e artefatos (neste caso, um código de autorização) que o aplicativo usa para obter um token de acesso.

    O URI de redirecionamento *http://localhost:5000/login/authorized* é o valor que o middleware OmniAuth está configurado para usar quando tiver processado a solicitação de autenticação.

8. Escolha **Salvar**.

## <a name="create-oauth-client"></a>Criar o cliente OAuth

Seu aplicativo precisa registrar uma instância do cliente Flask OAuth que você usará para iniciar o fluxo do OAuth e obter um token de acesso. 

No exemplo de Connect, o seguinte código (localizado em [*connect/__init__.py*](https://github.com/microsoftgraph/python3-connect-rest-sample/blob/master/connect/__init__.py)) registra o cliente com todos os valores obrigatórios, inclusive a ID de aplicativo (client_id), o segredo de aplicativo (client_secret) e a URL de autorização usada para autenticar esse usuário.

```python
    # Put your consumer key and consumer secret into a config file
    # and don't check it into github!!
    microsoft = oauth.remote_app(
        'microsoft',
        consumer_key=client_id,
        consumer_secret=client_secret,
        request_token_params={'scope': 'User.Read Mail.Send'},
        base_url='https://graph.microsoft.com/v1.0/',
        request_token_url=None,
        access_token_method='POST',
        access_token_url='https://login.microsoftonline.com/common/oauth2/v2.0/token',
        authorize_url='https://login.microsoftonline.com/common/oauth2/v2.0/authorize'
    )
```

<!--<a name="authCode"></a>-->
## <a name="receive-an-authorization-code-in-your-reply-url-page"></a>Receber um código de autorização em sua página de URL de resposta

Depois que o usuário entra, o navegador é redirecionado para a URL de resposta, a rota ```login/authorized``` em [*connect/__init__.py*](https://github.com/microsoftgraph/python3-connect-rest-sample/blob/master/connect/__init__.py), com um token de acesso na resposta. O exemplo armazena o token como uma variável de sessão.

```python
    @app.route('/login/authorized')
    def authorized():
        response = microsoft.authorized_response()
    
        if response is None:
            return "Access Denied: Reason=%s\nError=%s" % (
                request.args['error'], 
                request.args['error_description']
            )
    
        # Check response for state
        if str(session['state']) != str(request.args['state']):
            raise Exception('State has been messed with, end authentication')
        # Remove state session variable to prevent reuse.
        session['state'] = ""
            
        # Okay to store this in a local variable, encrypt if it's going to client
        # machine or database. Treat as a password. 
        session['microsoft_token'] = (response['access_token'], '')
        # Store the token in another session variable for easy access
        session['access_token'] = response['access_token']
        meResponse = microsoft.get('me')
        meData = json.dumps(meResponse.data)
        me = json.loads(meData)
        userName = me['displayName']
        userEmailAddress = me['userPrincipalName']
        session['alias'] = userName
        session['userEmailAddress'] = userEmailAddress
        return redirect('main')
```

<!--<a name="request"></a>-->
## <a name="use-the-access-token-in-a-request-to-the-microsoft-graph-api"></a>Usar o token de acesso em uma solicitação para a API do Microsoft Graph

Com um token de acesso, o aplicativo pode fazer solicitações autenticadas à API do Microsoft Graph. Seu aplicativo deve anexar o token de acesso ao cabeçalho **Authorization** de cada solicitação.

O exemplo do Connect envia um email usando o ponto de extremidade ```me/microsoft.graph.sendMail``` na API do Microsoft Graph. O código está na função ```call_sendMail_endpoint``` no arquivo [*connect/graph_service.py*](https://github.com/microsoftgraph/python3-connect-rest-sample/blob/master/connect/graph_service.py). Esse é o código que mostra como anexar o código de acesso ao cabeçalho Authorization.

```python
    # Set request headers.
    headers = { 
      'User-Agent' : 'python_tutorial/1.0',
      'Authorization' : 'Bearer {0}'.format(access_token),
      'Accept' : 'application/json',
      'Content-Type' : 'application/json'
    }
```

> **Observação** A solicitação também deve enviar um cabeçalho **Content-Type** com um valor aceito pela API do Microsoft Graph, por exemplo, `application/json`.

A API do Microsoft Graph é uma API unificadora muito poderosa que pode ser usada para interagir com todos os tipos de dados da Microsoft. Confira a referência de API para explorar o que mais você pode fazer com o Microsoft Graph.