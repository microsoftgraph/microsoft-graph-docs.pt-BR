# <a name="use-microsoft-graph-to-access-excel-in-a-python-app"></a><span data-ttu-id="6fc52-101">Usar o Microsoft Graph para acessar o Excel em um aplicativo Python</span><span class="sxs-lookup"><span data-stu-id="6fc52-101">Use Microsoft Graph to access Excel in a Python app</span></span>

<span data-ttu-id="6fc52-102">Você pode usar a API do Microsoft Graph para ler e atualizar pastas de trabalho armazenadas em plataformas de armazenamento online compatíveis, incluindo o OneDrive e o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6fc52-102">You can use the Microsoft Graph API to read and update workbooks stored in supported online storage platforms including, OneDrive and SharePoint. The  (or Excel file) resource contains all the other Excel resources and your app can access them via simple navigations.</span></span> <span data-ttu-id="6fc52-103">O recurso `Workbook` (ou o arquivo do Excel) contém todos os outros recursos do Excel, e seu aplicativo pode acessá-los por meio de navegações simples.</span><span class="sxs-lookup"><span data-stu-id="6fc52-103">You can use the Microsoft Graph API to read and update workbooks stored in supported online storage platforms including, OneDrive and SharePoint. The `Workbook` (or Excel file) resource contains all the other Excel resources and your app can access them via simple navigations.</span></span> 

<span data-ttu-id="6fc52-104">Você pode acessar um conjunto de objetos do Excel (como Table, Range ou Chart) usando APIs REST padrão para realizar operações de criação, leitura, atualização e exclusão (CRUD) na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6fc52-104">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, </span></span> <span data-ttu-id="6fc52-105">Por exemplo, `https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span><span class="sxs-lookup"><span data-stu-id="6fc52-105">For example:`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span></span>  
<span data-ttu-id="6fc52-106">retorna uma coleção de todos os objetos da planilha que fazem parte da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6fc52-106">returns a collection of worksheet objects that are part of the workbook.</span></span>    

<span data-ttu-id="6fc52-107">Esta explicação passo a passo descreve como fazer solicitações à API REST do Excel desde um aplicativo Web Python.</span><span class="sxs-lookup"><span data-stu-id="6fc52-107">This walkthrough describes how to make requests to the Excel REST API from a Python web app.</span></span> 

##  <a name="prerequisites"></a><span data-ttu-id="6fc52-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6fc52-108">Prerequisites</span></span>

* [<span data-ttu-id="6fc52-109">Python 3.5.2</span><span class="sxs-lookup"><span data-stu-id="6fc52-109">Python 3.5.2</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="6fc52-110">Flask-OAuthlib</span><span class="sxs-lookup"><span data-stu-id="6fc52-110">Flask-OAuthlib</span></span>](https://github.com/lepture/flask-oauthlib)
* <span data-ttu-id="6fc52-111">Uma [conta comercial ou escolar](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. --></span><span class="sxs-lookup"><span data-stu-id="6fc52-111">A [work or school account](https://msdn.microsoft.com/en-us/office/office365/howto/setup-development-environment#bk_Office365Account)<!-- This link target doesn't match the link title. Please verify that this is what you want to link to and update the text, or update the URL as appropriate. --></span></span>


## <a name="authorization-and-scopes"></a><span data-ttu-id="6fc52-112">Autorização e escopos</span><span class="sxs-lookup"><span data-stu-id="6fc52-112">Authorization and scopes</span></span>
<span data-ttu-id="6fc52-113">Você pode usar o [ponto de extremidade do Azure AD v2.0](https://graph.microsoft.io/en-us/docs/concepts/converged_auth) para autenticar chamadas da API REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="6fc52-113">You can use the [Azure AD v2.0 endpoint](https://graph.microsoft.io/en-us/docs/concepts/converged_auth) to authenticate Excel REST API calls. All APIs require the  HTTP header.</span></span> <span data-ttu-id="6fc52-114">Todas as APIs exigem o cabeçalho HTTP `Authorization: Bearer {access-token}`.</span><span class="sxs-lookup"><span data-stu-id="6fc52-114">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="6fc52-115">Um dos seguintes [escopos de permissão](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference) é obrigatório para se usar o recurso do Excel:</span><span class="sxs-lookup"><span data-stu-id="6fc52-115">One of the following [permission scopes](https://graph.microsoft.io/en-us/docs/concepts/permissions_reference) is required to use the Excel resource:</span></span>

* <span data-ttu-id="6fc52-116">Files.Read</span><span class="sxs-lookup"><span data-stu-id="6fc52-116">Files.Read</span></span> 
* <span data-ttu-id="6fc52-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6fc52-117">Files.ReadWrite</span></span>

## <a name="sessions-and-persistence"></a><span data-ttu-id="6fc52-118">Sessões e persistência</span><span class="sxs-lookup"><span data-stu-id="6fc52-118">Sessions and persistence</span></span>

<span data-ttu-id="6fc52-119">As APIs do Excel podem ser chamadas em um destes dois modos:</span><span class="sxs-lookup"><span data-stu-id="6fc52-119">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="6fc52-p104">Sessão persistente – Todas as alterações feitas na pasta de trabalho são persistentes (salvas). Este é o modo normal de operação.</span><span class="sxs-lookup"><span data-stu-id="6fc52-p104">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="6fc52-p105">Sessão não persistente – As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não afeta o estado do documento.</span><span class="sxs-lookup"><span data-stu-id="6fc52-p105">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="6fc52-126">Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="6fc52-126">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

## <a name="register-the-application-in-azure-active-directory"></a><span data-ttu-id="6fc52-127">Registrar o aplicativo no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6fc52-127">Register the application in Azure Active Directory</span></span>

<span data-ttu-id="6fc52-p106">Primeiro, você precisa registrar seu aplicativo e definir permissões para usar o Microsoft Graph. Isso permite que os usuários entrem no aplicativo com contas corporativas ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="6fc52-p106">First, you need to register your application and set permissions to use Microsoft Graph. This lets users sign in to the application with work or school accounts.</span></span>

### <a name="register-the-application"></a><span data-ttu-id="6fc52-130">Registrar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fc52-130">Register the application</span></span>

<span data-ttu-id="6fc52-p107">Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e a senha que você usará para configurar o aplicativo para autenticação.</span><span class="sxs-lookup"><span data-stu-id="6fc52-p107">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app for authentication.</span></span>

1. <span data-ttu-id="6fc52-133">Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="6fc52-133">Sign in to the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="6fc52-134">Escolha **Adicionar um aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="6fc52-134">Choose **Add an app**.</span></span>

3. <span data-ttu-id="6fc52-135">Insira um nome para o aplicativo e escolha **Criar aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="6fc52-135">Enter a name for the app, and choose **Create application**.</span></span>

    <span data-ttu-id="6fc52-136">A página de registro é exibida, listando as propriedades do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6fc52-136">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="6fc52-p108">Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6fc52-p108">Copy the application ID. This is the unique identifier for your app.</span></span>

5. <span data-ttu-id="6fc52-p109">Em **Segredos do Aplicativo**, escolha **Gerar Nova Senha**. Copie o segredo do aplicativo da caixa de diálogo **Nova senha gerada**.</span><span class="sxs-lookup"><span data-stu-id="6fc52-p109">Under **Application Secrets**, choose **Generate New Password**. Copy the app secret from the **New password generated** dialog box.</span></span>

    <span data-ttu-id="6fc52-141">Você usará a ID do aplicativo e o segredo do aplicativo para configurar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6fc52-141">You'll use the application ID and app secret to configure the app.</span></span>

6. <span data-ttu-id="6fc52-142">Em **Plataformas**, escolha **Adicionar plataforma** > **Web**.</span><span class="sxs-lookup"><span data-stu-id="6fc52-142">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="6fc52-143">Não deixe de marcar a caixa de diálogo **Permitir Fluxo Implícito** e insira o URI de Redirecionamento de seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6fc52-143">Make sure the **Allow Implicit Flow** check box is selected, and enter your app's Redirect URI.</span></span>

    <span data-ttu-id="6fc52-144">A opção **Permitir Fluxo Implícito** habilita o fluxo híbrido do OpenID Connect.</span><span class="sxs-lookup"><span data-stu-id="6fc52-144">The **Allow Implicit Flow** option enables the OpenID Connect hybrid flow.</span></span> <span data-ttu-id="6fc52-145">Durante a autenticação, isso permite que o aplicativo receba informações de entrada (o **id_token**) e artefatos (neste caso, um código de autorização) que o aplicativo usa para obter um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="6fc52-145">During authentication, this enables the app to receive both sign-in info (the id_token) and artifacts (in this case, an authorization code) that the app can use to obtain an access token.</span></span>

8. <span data-ttu-id="6fc52-146">Escolha **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="6fc52-146">Choose **Save**.</span></span>

### <a name="create-oauth-client"></a><span data-ttu-id="6fc52-147">Criar o cliente OAuth</span><span class="sxs-lookup"><span data-stu-id="6fc52-147">Create OAuth client</span></span>

<span data-ttu-id="6fc52-148">Seu aplicativo precisa registrar uma instância do cliente Flask OAuth que você usará para iniciar o fluxo do OAuth e obter um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="6fc52-148">Your app needs to register an instance of the Flask-OAuth client that you'll use to start the OAuth flow and get an access token.</span></span> <span data-ttu-id="6fc52-149">Observe que o escopo *Files.ReadWrite* é necessário para a obtenção de uma sessão do Excel que ofereça suporte a alterações persistentes.</span><span class="sxs-lookup"><span data-stu-id="6fc52-149">Note that the *Files.ReadWrite* scope is required to obtain an Excel session that supports persisted changes.</span></span>

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

### <a name="receive-an-authorization-code-in-your-reply-url-page"></a><span data-ttu-id="6fc52-150">Receber um código de autorização na sua página de URL de resposta</span><span class="sxs-lookup"><span data-stu-id="6fc52-150">Receive an authorization code in your reply URL page</span></span>

<span data-ttu-id="6fc52-p112">Depois que o usuário entrar, o navegador será redirecionado para a URL de resposta. Após a autorização bem-sucedida, será retornado o token de acesso (que será usado para autorizar solicitações adicionais) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fc52-p112">After the user signs in, the browser is redirected to your reply URL. Upon successful authorization, the access token (which will be used to authorize additional requests) will be returned in the response body.</span></span> 

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

## <a name="make-requests-to-the-excel-api"></a><span data-ttu-id="6fc52-153">Fazer solicitações à API do Excel</span><span class="sxs-lookup"><span data-stu-id="6fc52-153">Make requests to the Excel API</span></span>

### <a name="request-headers"></a><span data-ttu-id="6fc52-154">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fc52-154">Request headers</span></span> 
<span data-ttu-id="6fc52-p113">Com um token de acesso, o aplicativo pode fazer solicitações autenticadas à API do Microsoft Graph. Seu aplicativo deve anexar o token de acesso ao cabeçalho **Authorization** de cada solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fc52-p113">With an access token, your app can make authenticated requests to the Microsoft Graph API. Your app must append the access token to the **Authorization** header of each request.</span></span>

```python
    # Set request headers.
    headers = { 
        'User-Agent' : 'python_tutorial/1.0',
        'Authorization' : 'Bearer {0}'.format(access_token),
        'Accept' : 'application/json',
        'Content-Type' : 'application/json'
    }
```
> <span data-ttu-id="6fc52-157">**Observação** A solicitação também deve enviar um cabeçalho **Content-Type** com um valor aceito pela API do Microsoft Graph, por exemplo, `application/json`.</span><span class="sxs-lookup"><span data-stu-id="6fc52-157">**Note** The request must also send a **Content-Type** header with a value accepted by the Graph API, for example, `application/json`.</span></span>

### <a name="getting-an-excel-session"></a><span data-ttu-id="6fc52-158">Obtendo uma sessão do Excel</span><span class="sxs-lookup"><span data-stu-id="6fc52-158">Getting an Excel Session</span></span>
#### <a name="request"></a><span data-ttu-id="6fc52-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fc52-159">Request</span></span> 

<span data-ttu-id="6fc52-160">Passe um objeto JSON definindo o valor de `persistChanges` como `true` ou `false`.</span><span class="sxs-lookup"><span data-stu-id="6fc52-160">Pass a JSON object by setting the `persistChanges` value to `true` or `false`.</span></span> <span data-ttu-id="6fc52-161">Quando o valor de `persistChanges` está definido como `false`, uma id de sessão não persistente é retornada.</span><span class="sxs-lookup"><span data-stu-id="6fc52-161">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span> <span data-ttu-id="6fc52-162">Este exemplo usa a biblioteca HTTP de [Solicitações](http://docs.python-requests.org/en/latest/user/quickstart)</span><span class="sxs-lookup"><span data-stu-id="6fc52-162">This example uses the [Requests](http://docs.python-requests.org/en/latest/user/quickstart) HTTP library</span></span> 

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

#### <a name="response"></a><span data-ttu-id="6fc52-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fc52-163">Response</span></span>

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

#### <a name="usage"></a><span data-ttu-id="6fc52-164">Uso</span><span class="sxs-lookup"><span data-stu-id="6fc52-164">Usage</span></span> 

<span data-ttu-id="6fc52-165">A ID de sessão retornada da chamada anterior é transmitida como um cabeçalho nas solicitações de API subsequentes no cabeçalho HTTP **Workbook-Session-Id**.</span><span class="sxs-lookup"><span data-stu-id="6fc52-165">The session ID returned from the previous call is passed as a header on subsequent API requests in the **Workbook-Session-Id** HTTP header. For instance, to list worksheets in that Excel workbook.</span></span> <span data-ttu-id="6fc52-166">Por exemplo, para listar planilhas nessa pasta de trabalho do Excel.</span><span class="sxs-lookup"><span data-stu-id="6fc52-166">For instance, to list worksheets in that Excel workbook.</span></span>

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

#### <a name="response"></a><span data-ttu-id="6fc52-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fc52-167">Response</span></span>

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

## <a name="next-steps"></a><span data-ttu-id="6fc52-168">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6fc52-168">Next steps</span></span>

<span data-ttu-id="6fc52-169">Com o cabeçalho HTTP **Workbook-Session-Id**, você pode começar a emitir solicitações para buscar dados, criar gráficos e muito mais.</span><span class="sxs-lookup"><span data-stu-id="6fc52-169">With the **Workbook-Session-Id** HTTP header, you can begin issuing requests to fetch data, create charts, and much more.</span></span> 

* [<span data-ttu-id="6fc52-170">Cenários comuns de API do Excel</span><span class="sxs-lookup"><span data-stu-id="6fc52-170">Common Excel API scenarios</span></span>](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel#common-excel-scenarios)
* [<span data-ttu-id="6fc52-171">Trabalhando com o Excel no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6fc52-171">Working with Excel in Microsoft Graph</span></span>](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/excel)

<span data-ttu-id="6fc52-p116">A API REST do Excel no Microsoft Graph fornece uma maneira poderosa de acessar e interagir com os dados em pastas de trabalho do Excel. Explore outras coisas que se pode fazer com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6fc52-p116">The Excel REST API in Microsoft Graph provides a powerful way to access and interact with data in Excel workbooks. Explore what else is possible with Microsoft Graph.</span></span>

* [<span data-ttu-id="6fc52-174">Visão geral do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6fc52-174">Overview of Microsoft Graph</span></span>](https://developer.microsoft.com/graph/docs)
* [<span data-ttu-id="6fc52-175">Introdução ao Microsoft Graph em um aplicativo Python</span><span class="sxs-lookup"><span data-stu-id="6fc52-175">Get started with Microsoft Graph in a Python app</span></span>](https://developer.microsoft.com/graph/docs/get-started/python)
