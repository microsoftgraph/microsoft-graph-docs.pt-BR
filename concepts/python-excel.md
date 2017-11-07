# <a name="use-microsoft-graph-to-access-excel-in-a-python-app"></a>Usar o Microsoft Graph para acessar o Excel em um aplicativo Python

Você pode usar a API do Microsoft Graph para ler e atualizar pastas de trabalho armazenadas em plataformas de armazenamento online compatíveis, incluindo o OneDrive e o SharePoint. O recurso `Workbook` (ou o arquivo do Excel) contém todos os outros recursos do Excel, e seu aplicativo pode acessá-los por meio de navegações simples. 

Você pode acessar um conjunto de objetos do Excel (como Table, Range ou Chart) usando APIs REST padrão para realizar operações de criação, leitura, atualização e exclusão (CRUD) na pasta de trabalho. Por exemplo, `https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`  
retorna uma coleção de todos os objetos da planilha que fazem parte da pasta de trabalho.    

Esta explicação passo a passo descreve como fazer solicitações à API REST do Excel desde um aplicativo Web Python. 

##  <a name="prerequisites"></a>Pré-requisitos

* [Python 3.5.2](https://www.python.org/downloads/)
* [Flask-OAuthlib](https://github.com/lepture/flask-oauthlib)
* Uma [conta comercial ou escolar](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. -->


## <a name="authorization-and-scopes"></a>Autorização e escopos
Você pode usar o [ponto de extremidade do Azure AD v2.0](https://graph.microsoft.io/en-us/docs/concepts/converged_auth) para autenticar chamadas da API REST do Excel. Todas as APIs exigem o cabeçalho HTTP `Authorization: Bearer {access-token}`.   
  
Um dos seguintes [escopos de permissão](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference) é obrigatório para se usar o recurso do Excel:

* Files.Read 
* Files.ReadWrite

## <a name="sessions-and-persistence"></a>Sessões e persistência

As APIs do Excel podem ser chamadas em um destes dois modos: 

1. Sessão persistente – Todas as alterações feitas na pasta de trabalho são persistentes (salvas). Este é o modo normal de operação. 
2. Sessão não persistente – As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não afeta o estado do documento.   

Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`. 

## <a name="register-the-application-in-azure-active-directory"></a>Registrar o aplicativo no Azure Active Directory

Primeiro, você precisa registrar seu aplicativo e definir permissões para usar o Microsoft Graph. Isso permite que os usuários entrem no aplicativo com contas corporativas ou de estudante.

### <a name="register-the-application"></a>Registrar o aplicativo

Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e a senha que você usará para configurar o aplicativo para autenticação.

1. Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.

2. Escolha **Adicionar um aplicativo**.

3. Insira um nome para o aplicativo e escolha **Criar aplicativo**.

    A página de registro é exibida, listando as propriedades do seu aplicativo.

4. Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo.

5. Em **Segredos do Aplicativo**, escolha **Gerar Nova Senha**. Copie o segredo do aplicativo da caixa de diálogo **Nova senha gerada**.

    Você usará a ID do aplicativo e o segredo do aplicativo para configurar o aplicativo.

6. Em **Plataformas**, escolha **Adicionar plataforma** > **Web**.

7. Não deixe de marcar a caixa de diálogo **Permitir Fluxo Implícito** e insira o URI de Redirecionamento de seu aplicativo.

    A opção **Permitir Fluxo Implícito** habilita o fluxo híbrido do OpenID Connect. Durante a autenticação, isso permite que o aplicativo receba informações de entrada (o **id_token**) e artefatos (neste caso, um código de autorização) que o aplicativo usa para obter um token de acesso.

8. Escolha **Salvar**.

### <a name="create-oauth-client"></a>Criar o cliente OAuth

Seu aplicativo precisa registrar uma instância do cliente Flask OAuth que você usará para iniciar o fluxo do OAuth e obter um token de acesso. Observe que o escopo *Files.ReadWrite* é necessário para a obtenção de uma sessão do Excel que ofereça suporte a alterações persistentes.

```python
    # Put your consumer key and consumer secret into a config file
    # and don't check it into github!
    microsoft = oauth.remote_app(
        'microsoft',
        consumer_key = client_id,
        consumer_secret = client_secret,
        request_token_params = {'scope': 'User.Read Files.ReadWrite'},
        base_url = 'https://graph.microsoft.com/v1.0/',
        request_token_url = None,
        access_token_method = 'POST',
        access_token_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/token',
        authorize_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/authorize'
    )
```

### <a name="receive-an-authorization-code-in-your-reply-url-page"></a>Receber um código de autorização na sua página de URL de resposta

Depois que o usuário entrar, o navegador será redirecionado para a URL de resposta. Após a autorização bem-sucedida, será retornado o token de acesso (que será usado para autorizar solicitações adicionais) no corpo da resposta. 

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
```

## <a name="make-requests-to-the-excel-api"></a>Fazer solicitações à API do Excel

### <a name="request-headers"></a>Cabeçalhos de solicitação 
Com um token de acesso, o aplicativo pode fazer solicitações autenticadas à API do Microsoft Graph. Seu aplicativo deve anexar o token de acesso ao cabeçalho **Authorization** de cada solicitação.

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

### <a name="getting-an-excel-session"></a>Obtendo uma sessão do Excel
#### <a name="request"></a>Solicitação 

Passe um objeto JSON definindo o valor de `persistChanges` como `true` ou `false`. Quando o valor de `persistChanges` está definido como `false`, uma id de sessão não persistente é retornada. Este exemplo usa a biblioteca HTTP de [Solicitações](http://docs.python-requests.org/en/latest/user/quickstart) 

```python
    # Replace the id with your Excel workbook's drive id
    url = 'https://graph.microsoft.com/v1.0/me/drive/items/01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE/workbook/createSession'
    # Set request headers
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Content-Type' : 'application/json'
    }
    # Specify type of session
    body = {
        'persistChanges': True
    }
    
    response = requests.post(url, headers = headers, json = body)
```

#### <a name="response"></a>Resposta

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/{version}/$metadata#microsoft.graph.sessionInfo",
    "id": "{session-id}",
    "persistChanges": true
}
```

#### <a name="usage"></a>Uso 

A ID de sessão retornada da chamada anterior é transmitida como um cabeçalho nas solicitações de API subsequentes no cabeçalho HTTP **Workbook-Session-Id**. Por exemplo, para listar planilhas nessa pasta de trabalho do Excel.

```python
    # Replace the id with your Excel workbook's drive id
    url = 'https://graph.microsoft.com/v1.0/me/drive/items/01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE/workbook/worksheets'
    # Set request headers - note the session header 
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Workbook-Session-Id': 'cluster=PP1&session=12.a04039942e021.A272...'
    }
    
    response = requests.get(url, headers = headers)
```

#### <a name="response"></a>Resposta

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets",
    "value": [
    {
        "@odata.id": "/users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
        "id": "{00000000-0001-0000-0000-000000000000}",
        "name": "Session 1",
        "position": 0,
        "visibility": "Visible"
    },
    {
        "@odata.id": "/users('8473b867-3e4e-4e44-8d09-8c6da362080f')/drive/items('01TBZDUE23F3CNYSIEGNBZV2LZGWHMC7TE')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
        "id": "{00000000-0001-0000-0100-000000000000}",
        "name": "Session 2",
        "position": 1,
        "visibility": "Visible"
    }]
}
```

## <a name="next-steps"></a>Próximas etapas

Com o cabeçalho HTTP **Workbook-Session-Id**, você pode começar a emitir solicitações para buscar dados, criar gráficos e muito mais. 

* [Cenários comuns de API do Excel](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel#common-excel-scenarios)
* [Trabalhando com o Excel no Microsoft Graph](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel)

A API REST do Excel no Microsoft Graph fornece uma maneira poderosa de acessar e interagir com os dados em pastas de trabalho do Excel. Explore outras coisas que se pode fazer com o Microsoft Graph.

* [Visão geral do Microsoft Graph](https://developer.microsoft.com/graph/docs)
* [Introdução ao Microsoft Graph em um aplicativo Python](https://developer.microsoft.com/graph/docs/get-started/python)
