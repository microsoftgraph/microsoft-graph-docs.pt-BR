# <a name="get-started-with-microsoft-graph-in-a-ruby-on-rails-app"></a><span data-ttu-id="b014f-101">Introdução ao Microsoft Graph em um aplicativo Ruby on Rails</span><span class="sxs-lookup"><span data-stu-id="b014f-101">Get started with Microsoft Graph in a Ruby on Rails app</span></span>

<span data-ttu-id="b014f-p101">Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph. Ele orientará você em relação a como criar um [Exemplo de conexão da Microsoft para Ruby on Rails](https://github.com/microsoftgraph/ruby-connect-rest-sample) e explica os principais conceitos que você implementa para utilizar o Microsoft Graph. O artigo também descreve como acessar o Microsoft Graph usando chamadas diretas REST.</span><span class="sxs-lookup"><span data-stu-id="b014f-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample) and explains the main concepts that you implement to use the Microsoft Graph. The article also describes how to access Microsoft Graph by using direct REST calls.</span></span>

<span data-ttu-id="b014f-105">Para baixar uma versão do exemplo de conexão que usa o ponto de extremidade do Azure AD, confira [Exemplo de conexão da Microsoft para Ruby on Rails](https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth).</span><span class="sxs-lookup"><span data-stu-id="b014f-105">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth).</span></span>

<span data-ttu-id="b014f-106">A imagem a seguir mostra o aplicativo que você criará.</span><span class="sxs-lookup"><span data-stu-id="b014f-106">The following image shows the app you'll create.</span></span> 

![Captura de tela do exemplo de conexão com o Microsoft Graph para Ruby on Rails](./images/Microsoft-Graph-Ruby-Connect-UI.png)

<span data-ttu-id="b014f-p102">**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) para agilizar o processo ou baixe o [Exemplo de conexão REST para Ruby](https://github.com/microsoftgraph/ruby-connect-rest-sample) no qual este artigo se baseia.</span><span class="sxs-lookup"><span data-stu-id="b014f-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast, or download the [Ruby REST Connect sample](https://github.com/microsoftgraph/ruby-connect-rest-sample) that this article is based on.</span></span>


## <a name="prerequisites"></a><span data-ttu-id="b014f-110">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b014f-110">Prerequisites</span></span>

<span data-ttu-id="b014f-111">Para começar, será necessário:</span><span class="sxs-lookup"><span data-stu-id="b014f-111">To get started, you'll need:</span></span> 

- <span data-ttu-id="b014f-112">Ruby 2.1 para executar o exemplo em um servidor de desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="b014f-112">Ruby 2.1 to run the sample on a development server.</span></span>
- <span data-ttu-id="b014f-113">Estrutura do Rails (o exemplo foi testado nos Rails 4.2).</span><span class="sxs-lookup"><span data-stu-id="b014f-113">Rails framework (the sample has been tested on Rails 4.2).</span></span>
- <span data-ttu-id="b014f-114">Gerenciador de dependências do Bundler.</span><span class="sxs-lookup"><span data-stu-id="b014f-114">Bundler dependency manager.</span></span>
- <span data-ttu-id="b014f-115">Interface de servidor Web Rack para Ruby.</span><span class="sxs-lookup"><span data-stu-id="b014f-115">Rack web server interface for Ruby.</span></span>
- <span data-ttu-id="b014f-116">Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="b014f-116">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- <span data-ttu-id="b014f-p103">O Projeto inicial de conexão com o Microsoft Graph para Ruby on Rails. Baixe o [Exemplo de conexão com o Microsoft Graph para Ruby on Rails](https://github.com/microsoftgraph/ruby-connect-rest-sample). O projeto inicial está localizado na pasta _starter_.</span><span class="sxs-lookup"><span data-stu-id="b014f-p103">The Microsoft Graph Connect Starter Project for Ruby on Rails. Download the [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample). The starter project is located in the _starter_ folder.</span></span>


## <a name="register-the-application"></a><span data-ttu-id="b014f-120">Registrar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="b014f-120">Register the application</span></span>

<span data-ttu-id="b014f-p104">Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e o segredo que você usará para configurar o aplicativo para autenticação.</span><span class="sxs-lookup"><span data-stu-id="b014f-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and secret that you'll use to configure the app for authentication.</span></span>

1. <span data-ttu-id="b014f-123">Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="b014f-123">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="b014f-124">Escolha **Adicionar um aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="b014f-124">Choose **Add an app**.</span></span>

3. <span data-ttu-id="b014f-125">Insira um nome para o aplicativo e escolha **Criar aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="b014f-125">Enter a name for the app, and choose **Create application**.</span></span>

    <span data-ttu-id="b014f-126">A página de registro é exibida, listando as propriedades do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b014f-126">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="b014f-p105">Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b014f-p105">Copy the application ID. This is the unique identifier for your app.</span></span>

5. <span data-ttu-id="b014f-p106">Em **Segredos do Aplicativo**, escolha **Gerar Nova Senha**. Copie o segredo do aplicativo da caixa de diálogo **Nova senha gerada**.</span><span class="sxs-lookup"><span data-stu-id="b014f-p106">Under **Application Secrets**, choose **Generate New Password**. Copy the app secret from the **New password generated** dialog.</span></span>

    <span data-ttu-id="b014f-131">Você usará a ID do aplicativo e o segredo do aplicativo para configurar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b014f-131">You'll use the application ID and app secret to configure the app.</span></span>

6. <span data-ttu-id="b014f-132">Em **Plataformas**, escolha **Adicionar plataforma** > **Web**.</span><span class="sxs-lookup"><span data-stu-id="b014f-132">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="b014f-133">Não se esqueça de marcar a caixa **Permitir Fluxo Implícito** e insira *http://localhost:3000/auth/microsoft_v2_auth/callback* como o URI de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="b014f-133">Make sure the **Allow Implicit Flow** check box is selected, and enter *http://localhost:3000/auth/microsoft_v2_auth/callback* as the Redirect URI.</span></span>

    <span data-ttu-id="b014f-p107">A opção Permitir Fluxo Implícito habilita o fluxo híbrido do OpenID Connect. Durante a autenticação, isso permite que o aplicativo receba informações de entrada (o id_token) e artefatos (neste caso, um código de autorização) que o aplicativo usa para obter um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="b014f-p107">The Allow Implicit Flow option enables the OpenID Connect hybrid flow. During authentication, this enables the app to receive both sign-in info (the id_token) and artifacts (in this case, an authorization code) that the app uses to obtain an access token.</span></span>

    <span data-ttu-id="b014f-136">O URI de redirecionamento *http://localhost:3000/auth/microsoft_v2_auth/callback* é o valor que o middleware OmniAuth está configurado para usar quando tiver processado a solicitação de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b014f-136">The redirect URI *http://localhost:3000/auth/microsoft_v2_auth/callback* is the value that the OmniAuth middleware is configured to use once it has processed the authentication request.</span></span>

8. <span data-ttu-id="b014f-137">Escolha **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="b014f-137">Choose **Save**.</span></span>

## <a name="configure-the-project"></a><span data-ttu-id="b014f-138">Configurar o projeto</span><span class="sxs-lookup"><span data-stu-id="b014f-138">Configure the project</span></span>

1. <span data-ttu-id="b014f-p108">Baixe ou clone o [Exemplo de conexão com o Microsoft Graph para Ruby on Rails](https://github.com/microsoftgraph/ruby-connect-rest-sample). Abra a pasta _starter_ no editor de sua escolha.</span><span class="sxs-lookup"><span data-stu-id="b014f-p108">Download or clone the [Microsoft Graph Ruby on Rails Connect Sample](https://github.com/microsoftgraph/ruby-connect-rest-sample). Open the _starter_ folder in the editor of your choice.</span></span>
1. <span data-ttu-id="b014f-141">Caso ainda não tenha os recursos Bundler e Rack, você pode instalá-los com o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="b014f-141">If you don't already have bundler and rack, you can install them with the following command.</span></span>

    ```
    gem install bundler rack
    ```
2. <span data-ttu-id="b014f-142">No arquivo config/environment.rb, faça o seguinte.</span><span class="sxs-lookup"><span data-stu-id="b014f-142">In the config/environment.rb file, do the following:</span></span>
    - <span data-ttu-id="b014f-143">Substitua *ENTER_YOUR_CLIENT_ID* pela ID do cliente do aplicativo registrado.</span><span class="sxs-lookup"><span data-stu-id="b014f-143">Replace *ENTER_YOUR_CLIENT_ID* with the client ID of your registered  application.</span></span>
    - <span data-ttu-id="b014f-144">Substitua *ENTER_YOUR_SECRET* pela chave do aplicativo registrado.</span><span class="sxs-lookup"><span data-stu-id="b014f-144">Replace *ENTER_YOUR_SECRET* with the key of your registered application.</span></span>

3. <span data-ttu-id="b014f-145">Instale o aplicativo Rails e as dependências com o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="b014f-145">Install the Rails application and dependencies with the following command.</span></span>

    ```
    bundle install
    ```

## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="b014f-146">Autenticar o usuário e obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="b014f-146">Authenticate the user and get an access token</span></span>

<span data-ttu-id="b014f-p109">Este aplicativo usa o fluxo de concessão do código de autorização com uma identidade de usuário delegada. Para um aplicativo Web, o fluxo exige a ID do aplicativo, o segredo e o URI de redirecionamento do aplicativo registrado.</span><span class="sxs-lookup"><span data-stu-id="b014f-p109">This app uses the authorization code grant flow with a delegated user identity. For a web application, the flow requires the application ID, secret, and redirect URI from the registered app.</span></span> 

<span data-ttu-id="b014f-149">O fluxo de autenticação pode ser dividido nestas etapas básicas:</span><span class="sxs-lookup"><span data-stu-id="b014f-149">The auth flow can be broken down into these basic steps:</span></span>

1. <span data-ttu-id="b014f-150">Redirecione o usuário para autenticação e autorização.</span><span class="sxs-lookup"><span data-stu-id="b014f-150">Redirect the user for authentication and consent</span></span>
2. <span data-ttu-id="b014f-151">Obter um código de autorização</span><span class="sxs-lookup"><span data-stu-id="b014f-151">Get an authorization code</span></span>
3. <span data-ttu-id="b014f-152">Resgatar o código de autorização para solicitar um token de acesso</span><span class="sxs-lookup"><span data-stu-id="b014f-152">Redeem the authorization code for an access token</span></span>

><span data-ttu-id="b014f-153">Para mais informações sobre esse fluxo de autenticação, confira [Aplicativo Web para API Web](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api) e [Integrar a identidade da Microsoft e o Microsoft Graph em um aplicativo Web usando OpenID Connect](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/) na documentação do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b014f-153">For more information about this auth flow, see [Web application to web API](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api) and  [Integrate Microsoft identity and the Microsoft Graph into a web application using OpenID Connect](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/) in the Azure AD documentation.</span></span>

<span data-ttu-id="b014f-154">Usaremos uma pilha de três partes do middleware [Rack](http://rack.github.io/) para habilitar o aplicativo para autenticar no Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="b014f-154">We'll be using a stack of three pieces of [Rack](http://rack.github.io/) middleware to enable the app to authenticate against the Microsoft Graph:</span></span>

- <span data-ttu-id="b014f-155">[OmniAuth](https://rubygems.org/gems/omniauth), uma estrutura de Rack generalizada para autenticação de provedor múltiplo.</span><span class="sxs-lookup"><span data-stu-id="b014f-155">[OmniAuth](https://rubygems.org/gems/omniauth), a generalized Rack framework for multiple-provider authentication.</span></span>
- <span data-ttu-id="b014f-156">[Omniauth-oauth2](https://rubygems.org/gems/omniauth-oauth2), uma estratégia abstrata de OAuth2 para OmniAuth.</span><span class="sxs-lookup"><span data-stu-id="b014f-156">[Omniauth-oauth2](https://rubygems.org/gems/omniauth-oauth2), an abstract OAuth2 strategy for OmniAuth.</span></span> 
- <span data-ttu-id="b014f-p110">O omniauth-microsoft_v2_auth, uma estratégia do OmniAuth que personaliza o Omniauth-oauth2 para fornecer autenticação especificamente no ponto de extremidade do Azure AD v2.0. Este projeto está incluído no exemplo de código.</span><span class="sxs-lookup"><span data-stu-id="b014f-p110">omniauth-microsoft_v2_auth, an OmniAuth strategy that customizes Omniauth-oauth2 to specifically provide authentication against the Azure AD v2.0 endpoint. This project is included in the code sample.</span></span>

### <a name="specify-gem-dependencies-for-authentication"></a><span data-ttu-id="b014f-159">Especificar dependências gem para autenticação</span><span class="sxs-lookup"><span data-stu-id="b014f-159">Specify gem dependencies for authentication</span></span>

<span data-ttu-id="b014f-160">No Gemfile, tire os comentários das seguintes gems para adicioná-las como dependências.</span><span class="sxs-lookup"><span data-stu-id="b014f-160">In Gemfile, uncomment the following gems to add them as dependencies.</span></span>

    ```
    gem 'omniauth'
    gem 'omniauth-oauth2'
    gem 'omniauth-microsoft_v2_auth', path: './omniauth-microsoft_v2_auth'
    ```

<span data-ttu-id="b014f-161">Observe que `omniauth-microsoft_v2_auth` está incluído no projeto do aplicativo e será instalado a partir do caminho especificado.</span><span class="sxs-lookup"><span data-stu-id="b014f-161">Note that `omniauth-microsoft_v2_auth` is included in the app project, and will be installed from the path specified.</span></span> 

### <a name="configure-the-authentication-middleware"></a><span data-ttu-id="b014f-162">Configurar o middleware de autenticação</span><span class="sxs-lookup"><span data-stu-id="b014f-162">Configure the authentication middleware</span></span>

<span data-ttu-id="b014f-163">No `config/initializers/omniauth-microsoft_v2_auth.rb`, tire o comentário das linhas a seguir.</span><span class="sxs-lookup"><span data-stu-id="b014f-163">In `config/initializers/omniauth-microsoft_v2_auth.rb`, uncomment the following lines.</span></span>

    ```
    Rails.application.config.middleware.use OmniAuth::Builder do
      provider :microsoft_v2_auth,
      ENV['CLIENT_ID'],
      ENV['CLIENT_SECRET'],
      :scope => ENV['SCOPE']
    end
    ```
<span data-ttu-id="b014f-p111">Isso configura o middleware OmniAuth, incluindo a especificação da ID do aplicativo e o segredo do aplicativo a ser usado, bem como os escopos a serem solicitados para o usuário. Estes são os valores que você especificou anteriormente no `config/environment.rb`.</span><span class="sxs-lookup"><span data-stu-id="b014f-p111">This configures the OmniAuth middleware, including specifying the app ID and app secret to use, as well as the scopes to request for the user. These are the values you specified earlier in `config/environment.rb`.</span></span>

### <a name="specify-routes-for-authentication"></a><span data-ttu-id="b014f-166">Especificar rotas para autenticação</span><span class="sxs-lookup"><span data-stu-id="b014f-166">Specify routes for authentication</span></span>

<span data-ttu-id="b014f-p112">Agora precisamos especificar duas rotas necessárias para o fluxo de autenticação. A primeira rota encaminha a solicitação de autenticação para o middleware OmniAuth e a segunda especifica o local no aplicativo para o qual o OmniAuth deve redirecionar após a autenticação ocorrer.</span><span class="sxs-lookup"><span data-stu-id="b014f-p112">Now we need to specify two routes necessary for the authentication flow. The first route forwards the authentication request to the OmniAuth middleware, and the second specifies the location in the app to which OmniAuth should redirect once authentication has occurred.</span></span>

<span data-ttu-id="b014f-169">No `config/routes.rb`, tire o comentário da diretiva de rota a seguir.</span><span class="sxs-lookup"><span data-stu-id="b014f-169">In `config/routes.rb`, uncomment the following route directive.</span></span>

    get '/login', to: 'pages#login'

<span data-ttu-id="b014f-170">Isso direciona as solicitações de logon para o método `login` do controlador de páginas, que por sua vez redireciona a solicitação para o middleware omniauth-microsoft_v2_auth.</span><span class="sxs-lookup"><span data-stu-id="b014f-170">This directs login requests to the pages controller's `login` method, which in turn redirects the request to the omniauth-microsoft_v2_auth middleware.</span></span>

    def login
        redirect_to '/auth/microsoft_v2_auth'
    end

<span data-ttu-id="b014f-p113">Em seguida, precisamos especificar para onde no aplicativo OmniAuth deve-se redirecionar após a autenticação. Tire o comentário da rota a seguir.</span><span class="sxs-lookup"><span data-stu-id="b014f-p113">Next, we need to specify where in the app OmniAuth should redirect once authentication has occurred. Uncomment the following route.</span></span>

    match '/auth/:provider/callback', to: 'pages#callback', via: [:get, :post]

<span data-ttu-id="b014f-173">Quando o OmniAuth tiver terminado de autenticar o usuário, ele chamará a URL de redirecionamento especificada no registro do aplicativo; nesse caso, *http://localhost:3000/auth/microsoft_v2_auth/callback*.</span><span class="sxs-lookup"><span data-stu-id="b014f-173">When OmniAuth has finished authenticating the user, it calls the redirect URL specified in the app registration; in this case, *http://localhost:3000/auth/microsoft_v2_auth/callback*.</span></span> <span data-ttu-id="b014f-174">O padrão de rota acima corresponde a essa URL e, portanto, encaminha a solicitação para o método `callback` do controlador da página.</span><span class="sxs-lookup"><span data-stu-id="b014f-174">The route pattern above matches that URL and so routes the request to the page controller's `callback` method.</span></span>

### <a name="get-an-access-token"></a><span data-ttu-id="b014f-175">Obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="b014f-175">Get an access token</span></span>

<span data-ttu-id="b014f-176">Em seguida, adicionaremos o código que realmente inicia o processo de autenticação e recupera o token de acesso assim que o usuário tiver entrado com êxito.</span><span class="sxs-lookup"><span data-stu-id="b014f-176">Next, we'll add the code that actually starts the authentication process, and retrieves the access token once the user has successfully signed in.</span></span>

<span data-ttu-id="b014f-p115">Dê uma olhada em `app/views/pages/index.html.erb`, o modo de exibição da raiz do site. O modo de exibição inclui um único botão que permite que os usuários entrem.</span><span class="sxs-lookup"><span data-stu-id="b014f-p115">Take a look at `app/views/pages/index.html.erb`, the view for the site root. The view includes a single button, which enables users to sign in.</span></span>

    <button class="ms-Button" onclick="window.location.href = '/login'">
        <span class="ms-Button-label"><%= t('connect_button') %></span>
    </button>

<span data-ttu-id="b014f-p116">Como mostrado anteriormente, o método de logon redireciona para o middleware OmniAuth, que foi configurado com a ID do aplicativo e o segredo do aplicativo, além dos escopos para a solicitação para o usuário. Depois que o usuário for autenticado com êxito, o OmniAuth retornará um hash com o token de acesso e outras informações do usuário para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b014f-p116">As shown earlier, the login method redirects to the OmniAuth middleware, which has been configured with the app ID and app secret, as well as the scopes to request for the user. Once the user is successfully authenticated, OmniAuth returns a hash with the access token and other user information to the app.</span></span>

<span data-ttu-id="b014f-181">Agora vamos adicionar código para manipular o retorno de chamada OmniAuth e recuperar informações desse hash.</span><span class="sxs-lookup"><span data-stu-id="b014f-181">Now let's add code to handle the OmniAuth callback, and retrieve information from that hash.</span></span> 

<span data-ttu-id="b014f-182">Em `app/controllers/pages_controller.rb`, substitua o método `callback` vazio pelo código a seguir.</span><span class="sxs-lookup"><span data-stu-id="b014f-182">In `app/controllers/pages_controller.rb`, replace the empty `callback` method with the following code.</span></span>

    ```
    def callback
        # Access the authentication hash for omniauth
        # and extract the auth token, user name, and email
        data = request.env['omniauth.auth']
    
        @email = data[:extra][:raw_info][:userPrincipalName]
        @name = data[:extra][:raw_info][:displayName]

        # Associate token/user values to the session
        session[:access_token] = data['credentials']['token']
        session[:name] = @name
        session[:email] = @email
        
        # Debug logging
        logger.info "Name: #{@name}"
        logger.info "Email: #{@email}"
        logger.info "[callback] - Access token: #{session[:access_token]}"
    end

    ```

<span data-ttu-id="b014f-183">Este método recupera o hash de autenticação e, em seguida, armazena o token de acesso, o nome de usuário e o email na sessão atual.</span><span class="sxs-lookup"><span data-stu-id="b014f-183">This method retrieves the authentication hash, and then stores the access token, user name, and email in the current session.</span></span>

> <span data-ttu-id="b014f-p117">**Observação:** A autenticação simples e o tratamento do token neste projeto são apresentados somente para fins ilustrativos. Em um aplicativo de produção, você provavelmente deve construir uma maneira mais eficiente de tratamento de autenticação, incluindo o tratamento seguro de token e atualização de token.</span><span class="sxs-lookup"><span data-stu-id="b014f-p117">**Note:** The simple authentication  and token handling in this project is presented for illustrative purposes only. In a production app, you would likely construct a more robust way of handling authentication, including secure token handling and token refresh.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="b014f-186">Chamar o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b014f-186">Call Microsoft Graph</span></span>

<span data-ttu-id="b014f-187">Agora você está pronto para adicionar código para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b014f-187">Now you're ready to add code to call Microsoft Graph.</span></span> 

<span data-ttu-id="b014f-p118">O modo de exibição renderizado pelo método `callback` (`app/views/pages/callback.html.erb`) inclui um formulário simples com um único botão. O formulário posta em `send_mail` e inclui um único parâmetro, o endereço de email do destinatário.</span><span class="sxs-lookup"><span data-stu-id="b014f-p118">The view rendered by the `callback` method (`app/views/pages/callback.html.erb`) includes a simple form with a single button. The form posts to  `send_mail`, and includes a single parameter, the email address of the intended recipient.</span></span>
    
    ``` 
    <form action="../../send_mail" method="post">
      <div class="ms-Grid-col ms-u-mdPush1 ms-u-md9 ms-u-lgPush1 ms-u-lg6">
        ...
            <div class="ms-TextField">
               <input class="ms-TextField-field" name="specified_email" value="<%= @email %>">
            </div>
            <button class="ms-Button">
            <span class="ms-Button-label"><i class="ms-Icon ms-Icon--mail" aria-hidden="true"></i><%= t('send_mail_button') %></span>
            </button> 
        ...
    ```

<span data-ttu-id="b014f-190">Em `app/controllers/pages_controller.rb`, substitua o método `send_mail` vazio pelo código a seguir.</span><span class="sxs-lookup"><span data-stu-id="b014f-190">In `app/controllers/pages_controller.rb`, replace the empty `send_mail` method with the following code.</span></span>

    ```
    def send_mail
        logger.debug "[send_mail] - Access token: #{session[:access_token]}"
        
        # Used in the template
        @name = session[:name]
        @email = params[:specified_email]
        @recipient = params[:specified_email]
        @mail_sent = false
        
        send_mail_endpoint = URI("#{GRAPH_RESOURCE}#{SENDMAIL_ENDPOINT}")
        content_type = CONTENT_TYPE
        http = Net::HTTP.new(send_mail_endpoint.host, send_mail_endpoint.port)
        http.use_ssl = true
        
        # If you want to use a sniffer tool, like Fiddler, to see the request
        # you might need to add this line to tell the engine not to verify the
        # certificate or you might see a "certificate verify failed" error
        # http.verify_mode = OpenSSL::SSL::VERIFY_NONE
        
        email_body = File.read('app/assets/MailTemplate.html')
        email_body.sub! '{given_name}', @name
        email_subject = t('email_subject')
        
        logger.debug email_body
    
        email_message = "{
            Message: {
            Subject: '#{email_subject}',
            Body: {
                ContentType: 'HTML',
                Content: '#{email_body}'
            },
            ToRecipients: [
                {
                    EmailAddress: {
                        Address: '#{@recipient}'
                    }
                }
            ]
            },
            SaveToSentItems: true
            }"
            
        response = http.post(
            SENDMAIL_ENDPOINT,
            email_message,
            'Authorization' => "Bearer #{session[:access_token]}",
            'Content-Type' => content_type
        )
        
        logger.debug "Code: #{response.code}"
        logger.debug "Message: #{response.message}"
        
        # The send mail endpoint returns a 202 - Accepted code on success
        if response.code == '202'
            @mail_sent = true
        else
            @mail_sent = false
            flash[:httpError] = "#{response.code} - #{response.message}"
        end
        
        render 'callback'
    end
    ```

<span data-ttu-id="b014f-191">Esse código constrói a solicitação HTTP, formata o email e, em seguida, chama o Microsoft Graph para enviar o email.</span><span class="sxs-lookup"><span data-stu-id="b014f-191">This code constructs the HTTP request, formats the email, and then calls Microsoft Graph to send the email.</span></span>

<span data-ttu-id="b014f-p119">Para criar o email, o código obtém o nome de usuário do token de sessão e o endereço de email do destinatário dos parâmetros passados do formulário. O código, em seguida, lê o corpo do email de um modelo incluído no projeto, interpola o endereço de email e o nome de usuário e anexa o texto do email como o corpo da solicitação HTTP.</span><span class="sxs-lookup"><span data-stu-id="b014f-p119">To create the email, the code pulls the user name from the session token and the recipient email address from the parameters passed from the form. The code then reads the email body from a template included in the project, interpolates the user name and email address, and attaches the email text as the HTTP request body.</span></span>

<span data-ttu-id="b014f-194">Para enviar o email, o código constrói a solicitação HTTP, anexa o token de acesso como um cabeçalho de autorização e, em seguida, envia a solicitação para o ponto de extremidade de enviar email.</span><span class="sxs-lookup"><span data-stu-id="b014f-194">To send the email, the code constructs the HTTP request, attaches the access token as an authorization header, and then posts the request to the send email endpoint.</span></span>

<span data-ttu-id="b014f-195">Por fim, o código usa o código de resposta de HTTP retornado para notificar o usuário se o email foi concluído com êxito ou não.</span><span class="sxs-lookup"><span data-stu-id="b014f-195">Finally, the code uses the HTTP response code returned to notify the user whether or not the email was successful.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="b014f-196">Executar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="b014f-196">Run the app</span></span>

1. <span data-ttu-id="b014f-197">Instale o aplicativo Rails e as dependências com o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="b014f-197">Install the Rails application and dependencies with the following command.</span></span>

    ```
    bundle install
    ```
2. <span data-ttu-id="b014f-198">Para iniciar o aplicativo Rails, digite o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="b014f-198">To start the Rails application, type the following command.</span></span>

    ```
    rackup -p 3000
    ```
3. <span data-ttu-id="b014f-199">Acesse `http://localhost:3000` no navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="b014f-199">Go to `http://localhost:3000` in your web browser.</span></span>

## <a name="see-also"></a><span data-ttu-id="b014f-200">Confira também</span><span class="sxs-lookup"><span data-stu-id="b014f-200">See also</span></span>
- <span data-ttu-id="b014f-201">Experimente a API REST usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="b014f-201">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="b014f-202">Explorar nossos outros [exemplos do Microsoft Graph](https://github.com/microsoftgraph) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="b014f-202">Explore our other [Microsoft Graph samples](https://github.com/microsoftgraph) on GitHub.</span></span>


