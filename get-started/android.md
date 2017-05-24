# <a name="get-started-with-microsoft-graph-in-an-android-app"></a>Introdução ao Microsoft Graph em um aplicativo Android

> **Criando aplicativos para clientes corporativos?** O aplicativo pode não funcionar caso o cliente corporativo habilite os recursos Enterprise Mobility + Security, como <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">acesso condicional ao dispositivo</a>. Nesse caso, pode ser que você não esteja ciente e seu cliente pode enfrentar problemas de erro. 

> Para fornecer suporte a **todos os clientes corporativos**, em **todos os cenários corporativos**, use o ponto de extremidade do Microsoft Azure AD e gerencie os aplicativos usando o [Portal de Gerenciamento do Microsoft Azure](https://aka.ms/aadapplist). Para saber mais, confira o tópico [Decidindo entre os pontos de extremidade do Azure AD e do Azure AD v2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph. Ele o orienta sobre como criar um [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample) e explica os principais conceitos que você implementa para utilizar o Microsoft Graph em seu aplicativo para Android. O artigo também descreve como acessar o Microsoft Graph usando o [SDK do Microsoft Graph para Android](https://github.com/microsoftgraph/msgraph-sdk-android) ou chamadas REST não processadas.

Para usar o Microsoft Graph em seu aplicativo para Android, você precisa mostrar a página de entrada da Microsoft a seus usuários, conforme mostrado na captura de tela a seguir.

![Página de entrada das contas da Microsoft no Android](images/AndroidConnect.png)

**Não está com vontade de criar um aplicativo?** Comece rapidamente baixando o [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample) no qual este artigo se baseia.


## <a name="prerequisites"></a>Pré-requisitos

Para começar, será necessário: 

- Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](http://dev.office.com/devprogram)
- Android Studio versão 2.0 ou posterior


## <a name="register-the-application"></a>Registrar o aplicativo
Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e a senha que você usará para configurar o aplicativo.

1. Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.

2. Escolha **Adicionar um aplicativo**.

3. Insira um nome para o aplicativo e escolha **Criar aplicativo**. 
    
    A página de registro é exibida, listando as propriedades do seu aplicativo.

4. Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo. 

5. Escolha **Adicionar Plataforma** e **Aplicativo Nativo**.

    > **Observação:** O Portal de Registro de Aplicativos fornece um URI de Redirecionamento com um valor de *urn:ietf:wg:oauth:2.0:oob*. No entanto, você usará o valor de URI de Redirecionamento padrão *https://login.microsoftonline.com/common/oauth2/nativeclient*.

6. Escolha **Salvar**.


## <a name="configure-the-project"></a>Configurar o projeto

Inicie um novo projeto no Android Studio. Você pode manter os valores padrão para a maioria do assistente, apenas certifique-se de escolher as seguintes opções:

* Direcionar para Dispositivos Android – **Telefones e Tablets**
    * SDK Mínimo – **API 16: 4.1 Android (Jelly Bean)**
* Adicionar uma Atividade ao Dispositivo Móvel – **Atividade Básica**
 
Isso fornece um projeto para Android com uma atividade e um botão que você pode usar para autenticar o usuário.

> Observação: Você também pode usar o [Projeto inicial](https://github.com/microsoftgraph/android-java-connect-sample/tree/master/starter-project) que se encarrega da configuração do projeto para que você possa se concentrar nas seções de programação desta explicação passo a passo.

## <a name="authenticate-the-user-and-get-an-access-token"></a>Autenticar o usuário e obter um token de acesso
Você vai usar uma biblioteca do OAuth para simplificar o processo de autenticação. O [OpenID](http://openid.net) oferece o [AppAuth para Android](https://github.com/openid/AppAuth-Android), uma biblioteca que você pode usar neste projeto.

### <a name="add-the-dependency-to-appbuildgradle"></a>Adicionar a dependência a app/build.gradle

Abra o arquivo `build.gradle` no módulo do aplicativo e inclua a seguinte dependência:

```gradle
compile 'net.openid:appauth:0.3.0'
```

### <a name="start-the-authentication-flow"></a>Iniciar o fluxo de autenticação

1. Abra o arquivo **MainActivity** e declare um objeto **AuthorizationService** no método **onCreate**.
    ```java
    final AuthorizationService authorizationService =
        new AuthorizationService(this);
    ```
    
2. Localize o manipulador de eventos do evento de clique de *FloatingActionButton*. Substitua o método **onClick** pelo código a seguir. Insira a **ID do aplicativo** de seu aplicativo no espaço reservado marcado com **\<YOUR_APPLICATION_ID\>**.
    ```java
    @Override
    public void onClick(View view) {
        Uri authorizationEndpoint =
            Uri.parse("https://login.microsoftonline.com/common/oauth2/v2.0/authorize");
        Uri tokenEndpoint =
            Uri.parse("https://login.microsoftonline.com/common/oauth2/v2.0/token");
        AuthorizationServiceConfiguration config =
            new AuthorizationServiceConfiguration(
                    authorizationEndpoint,
                    tokenEndpoint,null);

        List<String> scopes = new ArrayList<>(
            Arrays.asList("openid mail.send".split(" ")));

        AuthorizationRequest authorizationRequest = new AuthorizationRequest.Builder(
            config,
            "<YOUR_APPLICATION_ID>",
            ResponseTypeValues.CODE,
            Uri.parse("https://login.microsoftonline.com/common/oauth2/nativeclient"))
            .setScopes(scopes)
            .build();

        Intent intent = new Intent(view.getContext(), MainActivity.class);

        PendingIntent redirectIntent =
            PendingIntent.getActivity(
                    view.getContext(),
                    authorizationRequest.hashCode(),
                    intent, 0);

        authorizationService.performAuthorizationRequest(
            authorizationRequest,
            redirectIntent);
    }
    ```
    
Nesse ponto, você deverá ter um aplicativo Android com um botão. Se você pressionar o botão, o aplicativo apresentará uma página de autenticação, utilizando o navegador do dispositivo. O próximo passo é manipular o código que o servidor de autorização envia para o URI de redirecionamento e trocá-lo por um token de acesso.

### <a name="exchange-the-authorization-code-for-an-access-token"></a>Trocar o código de autorização para solicitar um token de acesso

Você precisa preparar seu aplicativo para lidar com a resposta do servidor de autorização, que contém um código que você pode substituir por um token de acesso.

1. Você precisa informar ao sistema do Android que **MainActivity** pode lidar com solicitações para *https://login.microsoftonline.com/common/oauth2/nativeclient*. Para isso, abra o arquivo **AndroidManifest** e adicione os seguintes filhos ao elemento **intent-filter** de MainActivity.
    ```xml
    <action android:name="android.intent.action.VIEW"/>
    <category android:name="android.intent.category.DEFAULT"/>
    <category android:name="android.intent.category.BROWSABLE"/>
    <data android:scheme="https"/>
    <data android:host="login.microsoftonline.com"/>
    <data android:path="/common/oauth2/nativeclient"/>
    ```

2. A atividade será chamada quando o servidor de autorização enviar uma resposta. Você pode solicitar um token de acesso com a resposta do servidor de autorização. Volte para **MainActivity** e acrescente o seguinte código ao método **onCreate**.
    ```java
    Bundle extras = getIntent().getExtras();
    if (extras != null) {
        AuthorizationResponse authorizationResponse = AuthorizationResponse.fromIntent(getIntent());
        AuthorizationException authorizationException = AuthorizationException.fromIntent(getIntent());
        final AuthState authState = new AuthState(authorizationResponse, authorizationException);

        if (authorizationResponse != null) {
            HashMap<String, String> additionalParams = new HashMap<>();
            TokenRequest tokenRequest = authorizationResponse.createTokenExchangeRequest(additionalParams);

            authorizationService.performTokenRequest(
                tokenRequest,
                new AuthorizationService.TokenResponseCallback() {
                    @Override
                    public void onTokenRequestCompleted(
                            @Nullable TokenResponse tokenResponse,
                            @Nullable AuthorizationException ex) {
                        authState.update(tokenResponse, ex);
                        if (tokenResponse != null) {
                            String accessToken = tokenResponse.accessToken;
                        }
                    }
                });
        } else {
            Log.i("MainActivity", "Authorization failed: " + authorizationException);
        }
    }
    ```

Observe que você tem um token de acesso nesta linha `String accessToken = tokenResponse.accessToken;`. Agora você está pronto para adicionar código para chamar o Microsoft Graph. 

## <a name="call-microsoft-graph"></a>Chamar o Microsoft Graph
Você pode [usar o SDK do Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-sdk) ou a [API REST do Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-rest-api) para chamar o Microsoft Graph.

### <a name="call-microsoft-graph-using-the-microsoft-graph-sdk"></a>Chamar o Microsoft Graph usando o SDK do Microsoft Graph
O [SDK do Microsoft Graph para Android](https://github.com/microsoftgraph/msgraph-sdk-android) fornece classes que criam solicitações e processam resultados do Microsoft Graph. Siga estas etapas para usar o SDK do Microsoft Graph.

1. Adicione permissões de Internet ao seu aplicativo. Abra o arquivo **AndroidManifest** e adicione os seguintes filhos ao elemento de manifesto.
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    ```

2. Adicione dependências ao SDK do Microsoft Graph e GSON.
    ```gradle
    compile 'com.microsoft.graph:msgraph-sdk-android:1.0.0'
    compile 'com.google.code.gson:gson:2.7'
    ```
   
3. Substitua a linha `String accessToken = tokenResponse.accessToken;` pelo código a seguir. Insira seu endereço de email no espaço reservado marcado com **\<SEU_ENDEREÇO_DE_EMAIL\>**.
    ```java
    final String accessToken = tokenResponse.accessToken;
    final IClientConfig clientConfig = 
            DefaultClientConfig.createWithAuthenticationProvider(new IAuthenticationProvider() {
        @Override
        public void authenticateRequest(IHttpRequest request) {
            request.addHeader("Authorization", "Bearer " + accessToken);
        }
    });

    final IGraphServiceClient graphServiceClient = new GraphServiceClient
        .Builder()
        .fromConfig(clientConfig)
        .buildClient();

    final Message message = new Message();
    EmailAddress emailAddress = new EmailAddress();
    emailAddress.address = "<YOUR_EMAIL_ADDRESS>";
    Recipient recipient = new Recipient();
    recipient.emailAddress = emailAddress;
    message.toRecipients = Collections.singletonList(recipient);
    ItemBody itemBody = new ItemBody();
    itemBody.content = "This is the email body";
    itemBody.contentType = BodyType.text;
    message.body = itemBody;
    message.subject = "Sent using the Microsoft Graph SDK";

    AsyncTask.execute(new Runnable() {
        @Override
        public void run() {
            graphServiceClient
                .getMe()
                .getSendMail(message, false)
                .buildRequest()
                .post();
        }
    });
    ```

### <a name="call-microsoft-graph-using-the-microsoft-graph-rest-api"></a>Chamar o Microsoft Graph usando a API REST do Microsoft Graph
A [API REST do Microsoft Graph](http://developer.microsoft.com/en-us/graph/docs) expõe várias APIs dos serviços de nuvem da Microsoft por meio de um único ponto de extremidade da API REST. Siga estas etapas para usar a API REST.

1. Adicione permissões de Internet ao seu aplicativo. Abra o arquivo **AndroidManifest** e adicione os seguintes filhos ao elemento de manifesto.
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    ```

2. Adicione uma dependência à biblioteca HTTP de Volley.

    ```gradle
    compile 'com.android.volley:volley:1.0.0'
    ```
   
3. Substitua a linha `String accessToken = tokenResponse.accessToken;` pelo código a seguir. Insira seu endereço de email no espaço reservado marcado com **\<SEU_ENDEREÇO_DE_EMAIL\>**.
    ```java
    final String accessToken = tokenResponse.accessToken;

    final RequestQueue queue = Volley.newRequestQueue(getApplicationContext());
    String url ="https://graph.microsoft.com/v1.0/me/sendMail";
    final String body = "{" +
        "  Message: {" +
        "    subject: 'Sent using the Microsoft Graph REST API'," +
        "    body: {" +
        "      contentType: 'text'," +
        "      content: 'This is the email body'" +
        "    }," +
        "    toRecipients: [" +
        "      {" +
        "        emailAddress: {" +
        "          address: '<YOUR_EMAIL_ADDRESS>'" +
        "        }" +
        "      }" +
        "    ]}" +
        "}";

    final StringRequest stringRequest = new StringRequest(Request.Method.POST, url,
        new Response.Listener<String>() {
            @Override
            public void onResponse(String response) {
                Log.d("Response", response);
            }
        },
        new Response.ErrorListener() {
            @Override
            public void onErrorResponse(VolleyError error) {
                Log.d("ERROR","error => " + error.getMessage());
            }
        }
    ) {
        @Override
        public Map<String, String> getHeaders() throws AuthFailureError {
            Map<String,String> params = new HashMap<>();
            params.put("Authorization", "Bearer " + accessToken);
            params.put("Content-Length", String.valueOf(body.getBytes().length));
            return params;
        }
        @Override
        public String getBodyContentType() {
            return "application/json";
        }
        @Override
        public byte[] getBody() throws AuthFailureError {
            return body.getBytes();
        }
    };

    AsyncTask.execute(new Runnable() {
        @Override
        public void run() {
            queue.add(stringRequest);
        }
    });
    ```

## <a name="run-the-app"></a>Executar o aplicativo
Você está pronto para experimentar seu aplicativo Android.

1. Inicie seu emulador Android ou conecte seu dispositivo físico ao seu computador.
2. No Android Studio, pressione Shift + F10 para executar seu aplicativo.
3. Escolha seu dispositivo ou emulador Android na caixa de diálogo de implantação.
4. Toque no Botão de Ação Flutuante na atividade principal.
5. Entre com sua conta pessoal, comercial ou de estudante e conceda as permissões solicitadas.
6. Na caixa de diálogo de seleção de aplicativo, toque em seu aplicativo para continuar.

Verifique a caixa de entrada do endereço de email que você configurou em [Chamar Microsoft Graph](#call-microsoft-graph). É provável que você tenha um email da conta que utilizou para entrar no aplicativo.

## <a name="next-steps"></a>Próximas etapas
- Experimente o [Explorador do Microsoft Graph](https://graph.microsoft.io/graph-explorer).
- Encontre exemplos de operações comuns em [Exemplo de trechos para Android](https://github.com/microsoftgraph/android-java-snippets-sample) ou explore nossos outros [Exemplos para Android](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android) no GitHub.


## <a name="see-also"></a>Veja também
* [SDK do Microsoft Graph para Android](https://github.com/microsoftgraph/msgraph-sdk-android) 
* [Protocolos do Azure AD v2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
* [Tokens do Azure AD v2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
