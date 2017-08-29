# <a name="get-started-with-microsoft-graph-in-an-android-app"></a><span data-ttu-id="90f8d-101">Introdução ao Microsoft Graph em um aplicativo Android</span><span class="sxs-lookup"><span data-stu-id="90f8d-101">Get started with Microsoft Graph in an Android app</span></span>

> <span data-ttu-id="90f8d-p101">**Criando aplicativos para clientes corporativos?** O aplicativo pode não funcionar caso o cliente corporativo habilite os recursos Enterprise Mobility + Security, como <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">acesso condicional ao dispositivo</a>. Nesse caso, pode ser que você não esteja ciente e seu cliente pode enfrentar problemas de erro.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="90f8d-p102">Para fornecer suporte a **todos os clientes corporativos**, em **todos os cenários corporativos**, use o ponto de extremidade do Microsoft Azure AD e gerencie os aplicativos usando o [Portal de Gerenciamento do Microsoft Azure](https://aka.ms/aadapplist). Para saber mais, confira o tópico [Decidindo entre os pontos de extremidade do Azure AD e do Azure AD v2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="90f8d-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="90f8d-p103">Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph. Ele o orienta sobre como criar um [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample) e explica os principais conceitos que você implementa para utilizar o Microsoft Graph em seu aplicativo para Android. O artigo também descreve como acessar o Microsoft Graph usando o [SDK do Microsoft Graph para Android](https://github.com/microsoftgraph/msgraph-sdk-android) ou chamadas REST não processadas.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p103">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) and explains the main concepts that you implement to use Microsoft Graph in your app for Android. The article also describes how to access Microsoft Graph by using either the [Microsoft Graph SDK for Android](https://github.com/microsoftgraph/msgraph-sdk-android) or raw REST calls.</span></span>

<span data-ttu-id="90f8d-110">Para usar o Microsoft Graph em seu aplicativo para Android, você precisa mostrar a página de entrada da Microsoft a seus usuários, conforme mostrado na captura de tela a seguir.</span><span class="sxs-lookup"><span data-stu-id="90f8d-110">To use Microsoft Graph in your app for Android, you need to show the Microsoft sign in page to your users, as shown in the following screenshot.</span></span>

![Página de entrada das contas da Microsoft no Android](images/AndroidConnect.png)

<span data-ttu-id="90f8d-p104">**Não está com vontade de criar um aplicativo?** Comece rapidamente baixando o [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample) no qual este artigo se baseia.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p104">**Don't feel like building an app?** Get up and running fast by downloading the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) that this article is based on.</span></span>


## <a name="prerequisites"></a><span data-ttu-id="90f8d-114">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90f8d-114">Prerequisites</span></span>

<span data-ttu-id="90f8d-115">Para começar, será necessário:</span><span class="sxs-lookup"><span data-stu-id="90f8d-115">To get started, you'll need:</span></span> 

- <span data-ttu-id="90f8d-116">Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="90f8d-116">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- <span data-ttu-id="90f8d-117">Android Studio 2.0 ou posterior</span><span class="sxs-lookup"><span data-stu-id="90f8d-117">Android Studio 2.0 or newer version</span></span>


## <a name="configure-a-new-project"></a><span data-ttu-id="90f8d-118">Configurar um novo projeto</span><span class="sxs-lookup"><span data-stu-id="90f8d-118">Configure a new project</span></span>

<span data-ttu-id="90f8d-119">Se você baixou o [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample), pule esta etapa.</span><span class="sxs-lookup"><span data-stu-id="90f8d-119">If you have downloaded the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample), skip this step.</span></span> 

<span data-ttu-id="90f8d-p105">Inicie um novo projeto no Android Studio. Você pode manter os valores padrão para a maioria do assistente, apenas certifique-se de escolher as seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="90f8d-p105">Start a new project in Android Studio. You can leave the default values for most of the wizard, just make sure to choose the following options:</span></span>

* <span data-ttu-id="90f8d-122">Direcionar para Dispositivos Android – **Telefones e Tablets**</span><span class="sxs-lookup"><span data-stu-id="90f8d-122">Target Android Devices - **Phone and Tablet**</span></span>
    * <span data-ttu-id="90f8d-123">SDK Mínimo – **API 16: 4.1 Android (Jelly Bean)**</span><span class="sxs-lookup"><span data-stu-id="90f8d-123">Minimum SDK - **API 16: Android 4.1 (Jelly Bean)**</span></span>
* <span data-ttu-id="90f8d-124">Adicionar uma Atividade ao Dispositivo Móvel – **Atividade Básica**</span><span class="sxs-lookup"><span data-stu-id="90f8d-124">Add an Activity to Mobile - **Basic Activity**</span></span>
 
<span data-ttu-id="90f8d-125">Isso fornece um projeto para Android com uma atividade e um botão que você pode usar para autenticar o usuário.</span><span class="sxs-lookup"><span data-stu-id="90f8d-125">This provides you with an Android project with an activity and a button that you can use to authenticate the user.</span></span>


## <a name="register-the-application"></a><span data-ttu-id="90f8d-126">Registrar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="90f8d-126">Register the application</span></span>

<span data-ttu-id="90f8d-127">Você precisará registrar seu aplicativo no [Portal de Registro do Aplicativo da Microsoft](https://apps.dev.microsoft.com/) se tiver baixado o exemplo do Connect ou criado um novo projeto.</span><span class="sxs-lookup"><span data-stu-id="90f8d-127">You need to register your app on the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) whether you've downloaded the connect sample or created a new project.</span></span>

<span data-ttu-id="90f8d-p106">Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo que você usará para configurar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p106">Register an app on the Microsoft App Registration Portal. This generates the app ID that you'll use to configure the app.</span></span>

1. <span data-ttu-id="90f8d-130">Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="90f8d-130">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="90f8d-131">Escolha **Adicionar um aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="90f8d-131">Choose **Add an app**.</span></span>

><span data-ttu-id="90f8d-132">Dica: Se tiver baixado o [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample) e estiver criar um registro para ele, desmarque **Instalação Interativa** antes de escolher o botão **Criar**.</span><span class="sxs-lookup"><span data-stu-id="90f8d-132">Tip: If you have downloaded the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) and are just creating a registration for it, uncheck **Guided Setup** before chosing the **Create** button.</span></span>

3. <span data-ttu-id="90f8d-133">Insira um nome para o aplicativo e escolha **Criar**.</span><span class="sxs-lookup"><span data-stu-id="90f8d-133">Enter a name for the app, and choose **Create**.</span></span> 
    
    <span data-ttu-id="90f8d-134">Para o fluxo da **Instalação Interativa**:</span><span class="sxs-lookup"><span data-stu-id="90f8d-134">For the  **Guided Setup** flow:</span></span>
 
    <span data-ttu-id="90f8d-p107">a. Escolha **Aplicativo Móvel e da Área de Trabalho** para definir o tipo de aplicativo que você está criando.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p107">a. Choose **Mobile and Desktop App** to define the kind of app you are creating.</span></span>

    <span data-ttu-id="90f8d-p108">b. Escolha **Android** para definir a tecnologia móvel que você está usando.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p108">b. Choose **Android** to define the mobile technology you are using.</span></span>

    <span data-ttu-id="90f8d-p109">c. Leia o tópico introdutório e quando terminar, clique no botão **Instalação** no final da página.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p109">c. Review the introductory topic and when finished, click the **Setup** button at the end of the page.</span></span>

    <span data-ttu-id="90f8d-p110">d. Siga as instruções na etapa **Instalação** para adicionar a biblioteca de MSAL ao aplicativo build.gradle.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p110">d. Follow the instructions on the **Setup** step to add the MSAL library to your app build.gradle.</span></span>

    <span data-ttu-id="90f8d-p111">e. Siga as instruções na etapa **Usar** para adicionar a lógica de MSAL ao novo projeto.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p111">e. Follow the directions on the **Use** step to add MSAL logic to your new project</span></span>

    <span data-ttu-id="90f8d-p112">f. Na página **Configurar**, o portal criou uma identificação exclusiva do aplicativo para você. Use-a para configurar seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p112">f. On the **Configure** page, the portal has created a unique application ID for you. Use it to configure your app.</span></span>

    <span data-ttu-id="90f8d-148">Para o fluxo de não interativo:</span><span class="sxs-lookup"><span data-stu-id="90f8d-148">For the unguided flow:</span></span>

    <span data-ttu-id="90f8d-149">A página de registro é exibida, listando as propriedades do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="90f8d-149">The registration page displays, listing the properties of your app.</span></span>

    <span data-ttu-id="90f8d-p113">a. Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p113">a. Copy the application ID. This is the unique identifier for your app.</span></span> 

    <span data-ttu-id="90f8d-p114">b. Escolha **Adicionar Plataforma** e **Aplicativo Nativo**.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p114">b. Choose **Add Platform** and **Native Application**.</span></span>

    > <span data-ttu-id="90f8d-p115">**Observação:** O Portal de Registro de Aplicativos fornece um URI de Redirecionamento com um valor de *msalYOUR NEW APP ID://auth*. Não use URIs de redirecionamento incorporados. O [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample) implementa a biblioteca de autenticação de MSAL que requer esse URI de redirecionamento. Se estiver usando uma [biblioteca de terceiros com suporte](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-libraries#compatible-client-libraries) ou uma biblioteca **ADAL**, você deverá usar URIs de redirecionamento incorporados.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p115">**Note:** The Application Registration Portal provides a Redirect URI with a value of *msalYOUR NEW APP ID://auth*. Do not use the built-in redirect URIs. The [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) implements the MSAL authentication library which requires this redirect URI. If using a [supported third party library](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-libraries#compatible-client-libraries) or the **ADAL** library then you must use the built-in redirect URIs.</span></span>

    <span data-ttu-id="90f8d-158">Para o fluxo de Instalação Interativa e o fluxo não interativo</span><span class="sxs-lookup"><span data-stu-id="90f8d-158">For Guided Setup flow and unguided flow</span></span>

    <span data-ttu-id="90f8d-p116">a. Adicione permissões delegadas. Você precisará de **profile**, **Mail.ReadWrite**, **Mail.Send**, **Files.ReadWrite** e **User.ReadBasic.All**.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p116">a. Add delegated permissions. You'll need **profile**, **Mail.ReadWrite**, **Mail.Send**, **Files.ReadWrite**, and **User.ReadBasic.All**.</span></span> 
   
    <span data-ttu-id="90f8d-p117">b. Escolha **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p117">b. Choose **Save**.</span></span>


## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="90f8d-164">Autenticar o usuário e obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="90f8d-164">Authenticate the user and get an access token</span></span>

> <span data-ttu-id="90f8d-p118">**Observação:** Se você seguiu as instruções no fluxo da **Instalação Interativa** do portal de registro do aplicativo para criar um novo aplicativo, ignore essas etapas. Vá para [Chamar o Microsoft Graph usando o SDK do Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-sdk) para saber mais sobre a API do Graph</span><span class="sxs-lookup"><span data-stu-id="90f8d-p118">**Note:** If you followed the instructions in the **Guided Setup** flow from the application registration portal to create a new application, you can skip these steps. Go to [Call Microsoft Graph using the Microsoft Graph SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk) to learn more about the Graph API.</span></span>

<span data-ttu-id="90f8d-167">Vamos examinar o [Exemplo do Connect para Android](https://github.com/microsoftgraph/android-java-connect-sample) para conhecer o MSAL e o código adicionado do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="90f8d-167">Let's walk through the [Connect Sample for Android](https://github.com/microsoftgraph/android-java-connect-sample) to learn about the MSAL and Microsoft Graph code we've added.</span></span>

### <a name="add-the-dependency-to-appbuildgradle"></a><span data-ttu-id="90f8d-168">Adicionar a dependência a app/build.gradle</span><span class="sxs-lookup"><span data-stu-id="90f8d-168">Add the dependency to app/build.gradle</span></span>

<span data-ttu-id="90f8d-169">Abra o arquivo `build.gradle` no módulo do aplicativo e localize a seguinte dependência:</span><span class="sxs-lookup"><span data-stu-id="90f8d-169">Open the `build.gradle` file in the app module and find the following dependency:</span></span>

```gradle
    compile ('com.microsoft.identity.client:msal:0.1.+') {
        exclude group: 'com.android.support', module: 'appcompat-v7'
    }
    compile 'com.android.volley:volley:1.0.0'

```

### <a name="start-the-authentication-flow"></a><span data-ttu-id="90f8d-170">Iniciar o fluxo de autenticação</span><span class="sxs-lookup"><span data-stu-id="90f8d-170">Start the authentication flow</span></span>

1. <span data-ttu-id="90f8d-171">Abra o arquivo **AuthenticationManager** e localize a declaração do objeto **PublicClientApplication** e, em seguida, a instição no método **getInstance**.</span><span class="sxs-lookup"><span data-stu-id="90f8d-171">Open the **AuthenticationManager** file and find the **PublicClientApplication** object declaration and then the instation in the **getInstance** method.</span></span>

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


2. <span data-ttu-id="90f8d-p119">Na classe **ConnectActivity**, localize o manipulador de eventos do evento de clique de **mConnectButton**. Localize o método **onClick** e analise o código relevante.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p119">In the **ConnectActivity** class, locate the event handler for the click event of the **mConnectButton**. Find the **onClick** method and review relevant code.</span></span>
  
    <span data-ttu-id="90f8d-p120">O método **connect** habilita o log de Informações de Identificação Pessoal (IIP), obtém uma instância da classe auxiliar **AuthenticationManager** e obtém o conjunto de usuários do objeto da plataforma MSAL. Se não houver usuários, o novo usuário é levado para o fluxo de autorização e autenticação do Azure AD. Caso contrário, um símbolo de autenticação é obtido no modo silencioso.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p120">The **connect** method enables personally identifyable information (PII) logging, gets an instance of the sample helper class **AuthenticationManager**, and gets the MSAL platform object users collection. If there are no users, the new user is taken to the Azure AD authentication and authorization flow. Otherwise, an authentication token is obtained silently.</span></span>

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
3. <span data-ttu-id="90f8d-p121">Localize o manipulador de eventos que processa a resposta de redirecionamento do Azure AD gerada pelo Azure AD quando o usuário fecha a caixa de diálogo autenticação. Esse manipulador está na classe **ConnectActivity**.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p121">Find the event handler that processes the Azure AD redirect response generated by Azure AD when the user closes the authintication dialog. This handler is in the **ConnectActivity** class.</span></span>

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
3. <span data-ttu-id="90f8d-179">Localize o método de retorno de autenticação que armazena em cache o token de autenticação usado em chamadas da API do Graph.</span><span class="sxs-lookup"><span data-stu-id="90f8d-179">Find the authentication callback method that caches the authentication token that is used in Graph API calls.</span></span>

 

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
    
<span data-ttu-id="90f8d-p122">O aplicativo de exemplo do Connect conta com um botão **Connect** na atividade principal. Ao usar pela primeira vez, se você pressionar o botão, o aplicativo apresentará uma página de autenticação utilizando o navegador do dispositivo. O próximo passo é manipular o código que o servidor de autorização envia para o URI de redirecionamento e trocá-lo por um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p122">The connect sample app has a **Connect** button on the main activity. If you press the button, on first use, the app presents an authentication page using the device's browser. The next step is to handle the code that the authorization server sends to the redirect URI and exchange it for an access token.</span></span>

### <a name="exchange-the-authorization-code-for-an-access-token"></a><span data-ttu-id="90f8d-183">Trocar o código de autorização para solicitar um token de acesso</span><span class="sxs-lookup"><span data-stu-id="90f8d-183">Exchange the authorization code for an access token</span></span>

<span data-ttu-id="90f8d-184">Você precisa preparar seu aplicativo para lidar com a resposta do servidor de autorização, que contém um código que você pode substituir por um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="90f8d-184">You need to make your app ready to handle the authorization server response, which contains a code that you can exchange for an access token.</span></span>

1. <span data-ttu-id="90f8d-p123">Precisamos informar ao sistema Android que o aplicativo do Connect pode lidar com solicitações para a URL de redirecionamento configurada no registro do aplicativo. Para isso, abra o arquivo **AndroidManifest** e adicione os seguintes filhos ao elemento**\<application/\>** do projeto.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p123">We need to tell the Android system that Connect app can handle requests to the redirect URL configured in the application registration. To do this open the **AndroidManifest** file and add the following children to the projects  **\<application/\>** element.</span></span>
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
2. <span data-ttu-id="90f8d-p124">A biblioteca de **MSAL** precisa acessar a identificação do aplicativo atribuído através do portal de registro. **A biblioteca de MSAL refere-se à identificação do aplicativo como a "ID do cliente"**. Ela obtém a ID do Aplicativo (ID de cliente) no contexto do aplicativo passado no construtor da biblioteca.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p124">The **MSAL** library needs access to the application Id assigned by the registration portal. **The MSAL library refers to the application Id as the "Client Id"**. It gets the application Id (Client Id) from the application context that you pass in the library constructor.</span></span> 

   ><span data-ttu-id="90f8d-190">Observação: Você também pode fornecer a ID de cliente em tempo de execução passando um parâmetro de cadeia de caracteres para o construtor.</span><span class="sxs-lookup"><span data-stu-id="90f8d-190">Note: You can also provide the client Id at run-time by passing a string parameter to the constructor.</span></span> 

3. <span data-ttu-id="90f8d-p125">A atividade é chamada quando o servidor de autorização enviar uma resposta. Solicite um token de acesso com a resposta do servidor de autorização. Vá para seu **AuthenticationManager** e localize o seguinte código na classe.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p125">The activity is invoked when the authorization server sends a response. Request an access token with the response from the authorization server. Go to your **AuthenticationManager** and find the following code in the class.</span></span>

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


## <a name="call-microsoft-graph"></a><span data-ttu-id="90f8d-194">Chamar o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="90f8d-194">Call Microsoft Graph</span></span>
<span data-ttu-id="90f8d-195">Você pode [usar o SDK do Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-sdk) ou a [API REST do Microsoft Graph](#call-microsoft-graph-using-the-microsoft-graph-rest-api) para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="90f8d-195">You can [use the Microsoft Graph SDK](#call-microsoft-graph-using-the-microsoft-graph-sdk) or the [Microsoft Graph REST API](#call-microsoft-graph-using-the-microsoft-graph-rest-api) to call Microsoft Graph.</span></span>

### <a name="call-microsoft-graph-using-the-microsoft-graph-sdk"></a><span data-ttu-id="90f8d-196">Chamar o Microsoft Graph usando o SDK do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="90f8d-196">Call Microsoft Graph using the Microsoft Graph SDK</span></span>
<span data-ttu-id="90f8d-p126">O [SDK do Microsoft Graph para Android](https://github.com/microsoftgraph/msgraph-sdk-android) fornece classes que criam solicitações e processam resultados do Microsoft Graph. Siga estas etapas para usar o SDK do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p126">The [Microsoft Graph SDK for Android](https://github.com/microsoftgraph/msgraph-sdk-android) provides classes that build requests and process results from Microsoft Graph. Follow these steps to use the Microsoft Graph SDK.</span></span>

1. <span data-ttu-id="90f8d-p127">Adicione permissões de Internet ao seu aplicativo. Abra o arquivo **AndroidManifest** e adicione os seguintes filhos ao elemento de manifesto.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p127">Add Internet permissions to your app. Open the **AndroidManifest** file and add the following child to the manifest element.</span></span>
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
    <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />

    ```

2. <span data-ttu-id="90f8d-201">Adicione dependências ao SDK do Microsoft Graph e GSON.</span><span class="sxs-lookup"><span data-stu-id="90f8d-201">Add dependencies to the Microsoft Graph SDK and GSON.</span></span>
   ```gradle
    compile 'com.microsoft.graph:msgraph-sdk-android:1.3.2'
    compile 'com.google.code.gson:gson:2.7'
   ```


3. <span data-ttu-id="90f8d-p128">Adicione o token de autenticação às novas solicitações usando o método auxiliar **uthenticateRequest**. Esse método implementa o mesmo método a partir da interface **IAuthenticationProvider** da Autenticação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="90f8d-p128">Add authentication token to new requests using the **uthenticateRequest** helper method. This method implements the same method from the Microsoft Graph Authentication **IAuthenticationProvider** interface</span></span>
    
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

4. <span data-ttu-id="90f8d-204">Crie um email de rascunho e envie-o usando os seguintes métodos auxiliares da classe auxiliar **GraphServiceController**.</span><span class="sxs-lookup"><span data-stu-id="90f8d-204">Create a draft email and send it using the following helper methods from the **GraphServiceController** helper class.</span></span>

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
### <a name="call-microsoft-graph-using-the-microsoft-graph-rest-api"></a><span data-ttu-id="90f8d-205">Chamar o Microsoft Graph usando a API REST do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="90f8d-205">Call Microsoft Graph using the Microsoft Graph REST API</span></span>
<span data-ttu-id="90f8d-p129">A [API REST do Microsoft Graph](http://developer.microsoft.com/en-us/graph/docs) expõe várias APIs dos serviços de nuvem da Microsoft por meio de um único ponto de extremidade da API REST. Siga estas etapas para usar a API REST.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p129">The [Microsoft Graph REST API](http://developer.microsoft.com/en-us/graph/docs) exposes multiple APIs from Microsoft cloud services through a single REST API endpoint. Follow these steps to use the REST API.</span></span>

1. <span data-ttu-id="90f8d-p130">Adicione permissões de Internet ao seu aplicativo. Abra o arquivo **AndroidManifest** e adicione os seguintes filhos ao elemento de manifesto.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p130">Add Internet permissions to your app. Open the **AndroidManifest** file and add the following child to the manifest element.</span></span>
    ```xml
    <uses-permission android:name="android.permission.INTERNET" />
    ```

2. <span data-ttu-id="90f8d-210">Adicione uma dependência à biblioteca HTTP de Volley.</span><span class="sxs-lookup"><span data-stu-id="90f8d-210">Add a dependency to the Volley HTTP library.</span></span>

    ```gradle
    compile 'com.android.volley:volley:1.0.0'
    ```
   
3. <span data-ttu-id="90f8d-p131">Substitua a linha `String accessToken = tokenResponse.accessToken;` pelo código a seguir. Insira seu endereço de email no espaço reservado marcado com **\<SEU_ENDEREÇO_DE_EMAIL\>**.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p131">Replace the line `String accessToken = tokenResponse.accessToken;` with the following code. Insert your email address in the placeholder marked with **\<YOUR_EMAIL_ADDRESS\>**.</span></span>
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

## <a name="run-the-app"></a><span data-ttu-id="90f8d-213">Executar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="90f8d-213">Run the app</span></span>
<span data-ttu-id="90f8d-214">Você está pronto para experimentar seu aplicativo Android.</span><span class="sxs-lookup"><span data-stu-id="90f8d-214">You're ready to try your Android app.</span></span>

1. <span data-ttu-id="90f8d-215">Inicie seu emulador Android ou conecte seu dispositivo físico ao seu computador.</span><span class="sxs-lookup"><span data-stu-id="90f8d-215">Start your Android emulator or connect your physical device to your computer.</span></span>
2. <span data-ttu-id="90f8d-216">No Android Studio, pressione Shift + F10 para executar seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="90f8d-216">In Android Studio, press Shift + F10 to run your app.</span></span>
3. <span data-ttu-id="90f8d-217">Escolha seu dispositivo ou emulador Android na caixa de diálogo de implantação.</span><span class="sxs-lookup"><span data-stu-id="90f8d-217">Choose your Android emulator or device from the deployment dialog box.</span></span>
4. <span data-ttu-id="90f8d-218">Toque no Botão de Ação Flutuante na atividade principal.</span><span class="sxs-lookup"><span data-stu-id="90f8d-218">Tap the Floating Action Button on the main activity.</span></span>
5. <span data-ttu-id="90f8d-219">Entre com sua conta pessoal, comercial ou de estudante e conceda as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="90f8d-219">Sign in with your personal or work or school account and grant the requested permissions.</span></span>
6. <span data-ttu-id="90f8d-220">Na caixa de diálogo de seleção de aplicativo, toque em seu aplicativo para continuar.</span><span class="sxs-lookup"><span data-stu-id="90f8d-220">In the app selection dialog, tap your app to continue.</span></span>

<span data-ttu-id="90f8d-p132">Verifique a caixa de entrada do endereço de email que você configurou em [Chamar Microsoft Graph](#call-microsoft-graph). É provável que você tenha um email da conta que utilizou para entrar no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="90f8d-p132">Check the inbox of the email address that you configured in [Call Microsoft Graph](#call-microsoft-graph). You should have an email from the account that you used to sign in to the app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="90f8d-223">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="90f8d-223">Next steps</span></span>
- <span data-ttu-id="90f8d-224">Experimente o [Explorador do Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="90f8d-224">Try out the [Microsoft Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="90f8d-225">Encontre exemplos de operações comuns em [Exemplo de trechos para Android](https://github.com/microsoftgraph/android-java-snippets-sample) ou explore nossos outros [Exemplos para Android](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="90f8d-225">Find examples of common operations in the [Snippets Sample for Android](https://github.com/microsoftgraph/android-java-snippets-sample), or explore our other [Android samples](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=android) on GitHub.</span></span>


## <a name="see-also"></a><span data-ttu-id="90f8d-226">Veja também</span><span class="sxs-lookup"><span data-stu-id="90f8d-226">See also</span></span>
- [<span data-ttu-id="90f8d-227">SDK do Microsoft Graph para Android</span><span class="sxs-lookup"><span data-stu-id="90f8d-227">Microsoft Graph SDK for Android</span></span>](https://github.com/microsoftgraph/msgraph-sdk-android) 
- [<span data-ttu-id="90f8d-228">Obter tokens de acesso para chamar o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="90f8d-228">Get access tokens to call Microsoft Graph</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [<span data-ttu-id="90f8d-229">Obter acesso em nome de um usuário</span><span class="sxs-lookup"><span data-stu-id="90f8d-229">Get access on behalf of a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [<span data-ttu-id="90f8d-230">Obter acesso sem um usuário</span><span class="sxs-lookup"><span data-stu-id="90f8d-230">Get access without a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)
