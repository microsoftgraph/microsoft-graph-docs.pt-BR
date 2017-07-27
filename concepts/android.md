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
- Android Studio 2.0 ou posterior


## <a name="configure-a-new-project"></a>Configurar um novo projeto

Se você baixou o [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample), pule esta etapa. 

Inicie um novo projeto no Android Studio. Você pode manter os valores padrão para a maioria do assistente, apenas certifique-se de escolher as seguintes opções:

* Direcionar para Dispositivos Android – **Telefones e Tablets**
    * SDK Mínimo – **API 16: 4.1 Android (Jelly Bean)**
* Adicionar uma Atividade ao Dispositivo Móvel – **Atividade Básica**
 
Isso fornece um projeto para Android com uma atividade e um botão que você pode usar para autenticar o usuário.


## <a name="register-the-application"></a>Registrar o aplicativo

Você precisará registrar seu aplicativo no [Portal de Registro do Aplicativo da Microsoft](https://apps.dev.microsoft.com/) se tiver baixado o exemplo do Connect ou criado um novo projeto.

Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo que você usará para configurar o aplicativo.

1. Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.

2. Escolha **Adicionar um aplicativo**.

>Dica: Se tiver baixado o [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample) e estiver criar um registro para ele, desmarque **Instalação Interativa** antes de escolher o botão **Criar**.

3. Insira um nome para o aplicativo e escolha **Criar**. 
    
    Para o fluxo da **Instalação Interativa**:
 
    a. Escolha **Aplicativo Móvel e da Área de Trabalho** para definir o tipo de aplicativo que você está criando.

    b. Escolha **Android** para definir a tecnologia móvel que você está usando.

    c. Leia o tópico introdutório e quando terminar, clique no botão **Instalação** no final da página.

    d. Siga as instruções na etapa **Instalação** para adicionar a biblioteca de MSAL ao aplicativo build.gradle.

    e. Siga as instruções na etapa **Usar** para adicionar a lógica de MSAL ao novo projeto.

    f. Na página **Configurar**, o portal criou uma identificação exclusiva do aplicativo para você. Use-a para configurar seu aplicativo.

    Para o fluxo de não interativo:

    A página de registro é exibida, listando as propriedades do seu aplicativo.

    a. Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo. 

    b. Escolha **Adicionar Plataforma** e **Aplicativo Nativo**.

    > **Observação:** O Portal de Registro de Aplicativos fornece um URI de Redirecionamento com um valor de *msalYOUR NEW APP ID://auth*. Não use URIs de redirecionamento incorporados. O [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample) implementa a biblioteca de autenticação de MSAL que requer esse URI de redirecionamento. Se estiver usando uma [biblioteca de terceiros com suporte](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-libraries#compatible-client-libraries) ou uma biblioteca **ADAL**, você deverá usar URIs de redirecionamento incorporados.

    Para o fluxo de Instalação Interativa e o fluxo não interativo

    a. Adicione permissões delegadas. Você precisará de **profile**, **Mail.ReadWrite**, **Mail.Send**, **Files.ReadWrite** e **User.ReadBasic.All**. 
   
    b. Escolha **Salvar**.


## <a name="authenticate-the-user-and-get-an-access-token"></a>Autenticar o usuário e obter um token de acesso

> **Observação:** Se você seguiu as instruções no fluxo da **Instalação Interativa** do portal de registro do aplicativo para criar um novo aplicativo, ignore essas etapas. Vá para [Chamar o Microsoft Graph usando o SDK do Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-sdk) para saber mais sobre a API do Graph

Vamos examinar o [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample) para conhecer o MSAL e o código adicionado do Microsoft Graph.

### <a name="add-the-dependency-to-appbuildgradle"></a>Adicionar a dependência a app/build.gradle

Abra o arquivo `build.gradle` no módulo do aplicativo e localize a seguinte dependência:

```gradle
    compile ('com.microsoft.identity.client:msal:0.1.+') {
        exclude group: 'com.android.support', module: 'appcompat-v7'
    }
    compile 'com.android.volley:volley:1.0.0'

```

### <a name="start-the-authentication-flow"></a>Iniciar o fluxo de autenticação

1. Abra o arquivo **AuthenticationManager** e localize a declaração do objeto **PublicClientApplication** e, em seguida, a instição no método **getInstance**.

   ```java
    private static PublicClientApplication mPublicClientApplication;
    ....

    public static synchronized AuthenticationManager getInstance() {
        if (INSTANCE == null) {
            INSTANCE = new AuthenticationManager();
            if (mPublicClientApplication == null) {
                mPublicClientApplication = new PublicClientApplication(Connect.getInstance());
            }
        }
        return INSTANCE;
    }

   ```


2. Na classe **ConnectActivity**, localize o manipulador de eventos do evento de clique de **mConnectButton**. Localize o método **onClick** e analise o código relevante.
  
    O método **connect** habilita o log de Informações de Identificação Pessoal (IIP), obtém uma instância da classe auxiliar **AuthenticationManager** e obtém o conjunto de usuários do objeto da plataforma MSAL. Se não houver usuários, o novo usuário é levado para o fluxo de autorização e autenticação do Azure AD. Caso contrário, um símbolo de autenticação é obtido no modo silencioso.

   ```java
    @Override
    public void onClick(View view) {
        ....
        connect();
    }

        private void connect() {

        if (mEnablePiiLogging) {
            Logger.getInstance().setEnablePII(true);
        } else {
            Logger.getInstance().setEnablePII(false);
        }

        AuthenticationManager mgr = AuthenticationManager.getInstance();

        List<User> users = null;

        try {
            users = mgr.getPublicClient().getUsers();

            if (users != null && users.size() == 1) {
                mUser = users.get(0);
                mgr.callAcquireTokenSilent(mUser, true, this);
            } else {
                mgr.callAcquireToken(
                        this,
                        this);
            }
        } catch (MsalClientException e) {
            Log.d(TAG, "MSAL Exception Generated while getting users: " + e.toString());

        } catch (IndexOutOfBoundsException e) {
            Log.d(TAG, "User at this position does not exist: " + e.toString());
        }
    }

   ```
3. Localize o manipulador de eventos que processa a resposta de redirecionamento do Azure AD gerada pelo Azure AD quando o usuário fecha a caixa de diálogo autenticação. Esse manipulador está na classe **ConnectActivity**.

   ```java
       /**
     * Handles redirect response from https://login.microsoftonline.com/common and
     * notifies the MSAL library that the user has completed the authentication
     * dialog
     * @param requestCode
     * @param resultCode
     * @param data
     */
    @Override
    protected void onActivityResult(int requestCode, int resultCode, Intent data) {
        super.onActivityResult(requestCode, resultCode, data);
        if (AuthenticationManager
                .getInstance()
                .getPublicClient() != null) {
            AuthenticationManager
                    .getInstance()
                    .getPublicClient()
                    .handleInteractiveRequestRedirect(requestCode, resultCode, data);
        }
    }

   ```    
3. Localize o método de retorno de autenticação que armazena em cache o token de autenticação usado em chamadas da API do Graph.

 

```java
    /* Callback used for interactive request.  If succeeds we use the access
         * token to call the Microsoft Graph. Does not check cache
         */
    private AuthenticationCallback getAuthInteractiveCallback() {
        return new AuthenticationCallback() {
            @Override
            public void onSuccess(AuthenticationResult authenticationResult) {
            /* Successfully got a token, call graph now */
                Log.d(TAG, "Successfully authenticated");
                Log.d(TAG, "ID Token: " + authenticationResult.getIdToken());

            /* Store the auth result */
                mAuthResult = authenticationResult;
                if (mActivityCallback != null)
                    mActivityCallback.onSuccess(mAuthResult);
            }

            @Override
            public void onError(MsalException exception) {
            /* Failed to acquireToken */
                Log.d(TAG, "Authentication failed: " + exception.toString());
                if (mActivityCallback != null)
                    mActivityCallback.onError(exception);
            }

            @Override
            public void onCancel() {
            /* User canceled the authentication */
                Log.d(TAG, "User cancelled login.");
            }
        };
    }

```
    
O aplicativo de exemplo do Connect conta com um botão **Connect** na atividade principal. Ao usar pela primeira vez, se você pressionar o botão, o aplicativo apresentará uma página de autenticação utilizando o navegador do dispositivo. O próximo passo é manipular o código que o servidor de autorização envia para o URI de redirecionamento e trocá-lo por um token de acesso.

### <a name="exchange-the-authorization-code-for-an-access-token"></a>Trocar o código de autorização para solicitar um token de acesso

Você precisa preparar seu aplicativo para lidar com a resposta do servidor de autorização, que contém um código que você pode substituir por um token de acesso.

1. Precisamos informar ao sistema Android que o aplicativo do Connect pode lidar com solicitações para a URL de redirecionamento configurada no registro do aplicativo. Para isso, abra o arquivo **AndroidManifest** e adicione os seguintes filhos ao elemento**\<application/\>** do projeto.
    ```xml
        <uses-sdk tools:overrideLibrary="com.microsoft.identity.msal" />
        <application ...>
            ...
            <activity
                android:name="com.microsoft.identity.client.BrowserTabActivity">
                <intent-filter>
                    <action android:name="android.intent.action.VIEW" />
                    <category android:name="android.intent.category.DEFAULT" />
                    <category android:name="android.intent.category.BROWSABLE" />
                    <data android:scheme="msalENTER_YOUR_CLIENT_ID"
                        android:host="auth" />
                </intent-filter>
            </activity>
            <meta-data
                android:name="https://login.microsoftonline.com/common"
                android:value="authority string"/>
            <meta-data
                android:name="com.microsoft.identity.client.ClientId"
                android:value="ENTER_YOUR_CLIENT_ID"/>
        </application>
    ```
2. A biblioteca de **MSAL** precisa acessar a identificação do aplicativo atribuído através do portal de registro. **A biblioteca de MSAL refere-se à identificação do aplicativo como a "ID do cliente"**. Ela obtém a ID do Aplicativo (ID de cliente) no contexto do aplicativo passado no construtor da biblioteca. 

   >Observação: Você também pode fornecer a ID de cliente em tempo de execução passando um parâmetro de cadeia de caracteres para o construtor. 

3. A atividade é chamada quando o servidor de autorização enviar uma resposta. Solicite um token de acesso com a resposta do servidor de autorização. Vá para seu **AuthenticationManager** e localize o seguinte código na classe.

   ```java
    /**
     * Authenticates the user and lets the user authorize the app for the requested permissions.
     * An authentication token is returned via the getAuthInteractiveCalback method
     * @param activity
     * @param authenticationCallback
     */
    public void connect(Activity activity, final MSALAuthenticationCallback authenticationCallback){
        mActivityCallback = authenticationCallback;
        mPublicClientApplication.acquireToken(
                activity, Constants.SCOPES, getAuthInteractiveCallback());
    }


     /* Callback used for interactive request.  If succeeds we use the access
         * token to call the Microsoft Graph. Does not check cache
         */
    private AuthenticationCallback getAuthInteractiveCallback() {
        return new AuthenticationCallback() {
            @Override
            public void onSuccess(AuthenticationResult authenticationResult) {
            /* Successfully got a token, call graph now */
                Log.d(TAG, "Successfully authenticated");
                Log.d(TAG, "ID Token: " + authenticationResult.getIdToken());

            /* Store the auth result */
                mAuthResult = authenticationResult;
                if (mActivityCallback != null)
                    mActivityCallback.onSuccess(mAuthResult);
            }

            @Override
            public void onError(MsalException exception) {
            /* Failed to acquireToken */
                Log.d(TAG, "Authentication failed: " + exception.toString());
                if (mActivityCallback != null)
                    mActivityCallback.onError(exception);
            }

            @Override
            public void onCancel() {
            /* User canceled the authentication */
                Log.d(TAG, "User cancelled login.");
            }
        };
    }

     /**
     * Returns the access token obtained in authentication
     *
     * @return mAccessToken
     */
    public String getAccessToken() throws AuthenticatorException, IOException, OperationCanceledException {
        return  mAuthResult.getAccessToken();
    }

   ```


## <a name="call-microsoft-graph"></a>Chamar o Microsoft Graph
Você pode [usar o SDK do Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-sdk) ou a [API REST do Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-rest-api) para chamar o Microsoft Graph.

### <a name="call-microsoft-graph-using-the-microsoft-graph-sdk"></a>Chamar o Microsoft Graph usando o SDK do Microsoft Graph
O [SDK do Microsoft Graph para Android](https://github.com/microsoftgraph/msgraph-sdk-android) fornece classes que criam solicitações e processam resultados do Microsoft Graph. Siga estas etapas para usar o SDK do Microsoft Graph.

1. Adicione permissões de Internet ao seu aplicativo. Abra o arquivo **AndroidManifest** e adicione os seguintes filhos ao elemento de manifesto.
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
    <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />

    ```

2. Adicione dependências ao SDK do Microsoft Graph e GSON.
   ```gradle
    compile 'com.microsoft.graph:msgraph-sdk-android:1.3.2'
    compile 'com.google.code.gson:gson:2.7'
   ```


3. Adicione o token de autenticação às novas solicitações usando o método auxiliar **uthenticateRequest**. Esse método implementa o mesmo método a partir da interface **IAuthenticationProvider** da Autenticação do Microsoft Graph
    
   ```java
    /**
     * Appends an access token obtained from the {@link AuthenticationManager} class to the
     * Authorization header of the request.
     * @param request
     */
    @Override
    public void authenticateRequest(IHttpRequest request)  {
        try {
            request.addHeader("Authorization", "Bearer "
                    + AuthenticationManager.getInstance()
                    .getAccessToken());
            // This header has been added to identify this sample in the Microsoft Graph service.
            // If you're using this code for your project please remove the following line.
            request.addHeader("SampleID", "android-java-connect-sample");
        } catch (AuthenticatorException e) {
            e.printStackTrace();
        } catch (IOException e) {
            e.printStackTrace();
        }  catch (OperationCanceledException e) {
            e.printStackTrace();
        } catch (NullPointerException e) {
            e.printStackTrace();
        }
    }
   ```

4. Crie um email de rascunho e envie-o usando os seguintes métodos auxiliares da classe auxiliar **GraphServiceController**.

   ```java
    /**
     * Creates a draft email message using the Microsoft Graph API on Office 365. The mail is sent
     * from the address of the signed in user.
     *
     * @param senderPreferredName The mail senders principal user name (email addr)
     * @param emailAddress        The recipient email address.
     * @param subject             The subject to use in the mail message.
     * @param body                The body of the message.
     * @param callback            The callback method to invoke on completion of the POST request
     */
    public void createDraftMail(
            final String senderPreferredName,
            final String emailAddress,
            final String subject,
            final String body,
            ICallback<Message> callback
    ) {
        try {
            // create the email message
            Message message = createMessage(subject, body, emailAddress);
            mGraphServiceClient
                    .getMe()
                    .getMessages()
                    .buildRequest()
                    .post(message, callback);

        } catch (Exception ex) {
            showException(ex, "exception on send mail","Send mail failed", "The send mail method failed");
        }
    }

        /**
     * Creates a new Message object 
     */
    Message createMessage(
            String subject,
            String body,
            String address) {

        if (address == null || address.isEmpty()) {
            throw new IllegalArgumentException("The address parameter can't be null or empty.");
        } else {
            // perform a simple validation of the email address
            String addressParts[] = address.split("@");
            if (addressParts.length != 2 || addressParts[0].length() == 0 || addressParts[1].indexOf('.') == -1) {
                throw new IllegalArgumentException(
                        String.format("The address parameter must be a valid email address {0}", address)
                );
            }
        }
        Message message = new Message();
        EmailAddress emailAddress = new EmailAddress();
        emailAddress.address = address;
        Recipient recipient = new Recipient();
        recipient.emailAddress = emailAddress;
        message.toRecipients = Collections.singletonList(recipient);
        ItemBody itemBody = new ItemBody();
        itemBody.content = body;
        itemBody.contentType = BodyType.html;
        message.body = itemBody;
        message.subject = subject;
        return message;
    }
    /**
     * Sends a draft message to the specified recipients
     *
     * @param messageId String. The id of the message to send
     * @param callback
     */
    public void sendDraftMessage(String messageId,
                                 ICallback<Void> callback) {
        try {

            mGraphServiceClient
                    .getMe()
                    .getMessages(messageId)
                    .getSend()
                    .buildRequest()
                    .post(callback);

        } catch (Exception ex) {
            showException(ex, "exception on send draft message ","Send draft mail failed", "The send draft mail method failed");
        }
    }

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
- [SDK do Microsoft Graph para Android](https://github.com/microsoftgraph/msgraph-sdk-android) 
- [Obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [Obter acesso em nome de um usuário](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [Obter acesso sem um usuário](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)