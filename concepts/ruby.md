# <a name="get-started-with-microsoft-graph-in-a-ruby-on-rails-app"></a>Introdução ao Microsoft Graph em um aplicativo Ruby on Rails

Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph. Ele orientará você em relação a como criar um [Exemplo de conexão da Microsoft para Ruby on Rails](https://github.com/microsoftgraph/ruby-connect-rest-sample) e explica os principais conceitos que você implementa para utilizar o Microsoft Graph. O artigo também descreve como acessar o Microsoft Graph usando chamadas diretas REST.

Para baixar uma versão do exemplo de conexão que usa o ponto de extremidade do Azure AD, confira [Exemplo de conexão da Microsoft para Ruby on Rails](https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth).

A imagem a seguir mostra o aplicativo que você criará. 

![Captura de tela do exemplo de conexão com o Microsoft Graph para Ruby on Rails](./images/Microsoft-Graph-Ruby-Connect-UI.png)

**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) para começar a usar ou baixe o [Exemplo de conexão REST para Ruby](https://github.com/microsoftgraph/ruby-connect-rest-sample) no qual este artigo se baseia.


## <a name="prerequisites"></a>Pré-requisitos

Para começar, será necessário: 

- Ruby 2.1 para executar o exemplo em um servidor de desenvolvimento.
- Estrutura do Rails (o exemplo foi testado nos Rails 4.2).
- Gerenciador de dependências do Bundler.
- Interface de servidor Web Rack para Ruby.
- Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](http://dev.office.com/devprogram)
- O Projeto inicial de conexão com o Microsoft Graph para Ruby on Rails. Baixe o [Exemplo de conexão com o Microsoft Graph para Ruby on Rails](https://github.com/microsoftgraph/ruby-connect-rest-sample). O projeto inicial está localizado na pasta _starter_.


## <a name="register-the-application"></a>Registrar o aplicativo

Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e o segredo que você usará para configurar o aplicativo para autenticação.

1. Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.

2. Escolha **Adicionar um aplicativo**.

3. Insira um nome para o aplicativo e escolha **Criar aplicativo**.

    A página de registro é exibida, listando as propriedades do seu aplicativo.

4. Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo.

5. Em **Segredos do Aplicativo**, escolha **Gerar Nova Senha**. Copie o segredo do aplicativo da caixa de diálogo **Nova senha gerada**.

    Você usará a ID do aplicativo e o segredo do aplicativo para configurar o aplicativo.

6. Em **Plataformas**, escolha **Adicionar plataforma** > **Web**.

7. Não deixe de marcar a caixa de diálogo **Permitir Fluxo Implícito** e inserir *http://localhost:3000/auth/microsoft_v2_auth/callback* como o URI de Redirecionamento.

    A opção Permitir Fluxo Implícito habilita o fluxo híbrido do OpenID Connect. Durante a autenticação, isso permite que o aplicativo receba informações de entrada (o id_token) e artefatos (neste caso, um código de autorização) que o aplicativo usa para obter um token de acesso.

    O URI de redirecionamento *http://localhost:3000/auth/microsoft_v2_auth/callback* é o valor que o middleware OmniAuth está configurado para usar quando tiver processado a solicitação de autenticação.

8. Escolha **Salvar**.

## <a name="configure-the-project"></a>Configurar o projeto

1. Baixe ou clone o [Exemplo de conexão com o Microsoft Graph para Ruby on Rails](https://github.com/microsoftgraph/ruby-connect-rest-sample). Abra a pasta _starter_ no editor de sua escolha.
1. Caso ainda não tenha os recursos Bundler e Rack, você pode instalá-los com o seguinte comando.

    ```
    gem install bundler rack
    ```
2. No arquivo config/environment.rb, faça o seguinte.
    - Substitua *ENTER_YOUR_CLIENT_ID* pela ID do cliente do aplicativo registrado.
    - Substitua *ENTER_YOUR_SECRET* pela chave do aplicativo registrado.

3. Instale o aplicativo Rails e as dependências com o seguinte comando.

    ```
    bundle install
    ```

## <a name="authenticate-the-user-and-get-an-access-token"></a>Autenticar o usuário e obter um token de acesso

Este aplicativo usa o fluxo de concessão do código de autorização com uma identidade de usuário delegada. Para um aplicativo Web, o fluxo exige a ID do aplicativo, o segredo e o URI de redirecionamento do aplicativo registrado. 

O fluxo de autenticação pode ser dividido nestas etapas básicas:

1. Redirecione o usuário para autenticação e autorização.
2. Obter um código de autorização
3. Resgatar o código de autorização para solicitar um token de acesso

>Para mais informações sobre esse fluxo de autenticação, confira [Aplicativo Web para API Web](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api) e [Integrar a identidade da Microsoft e o Microsoft Graph em um aplicativo Web usando OpenID Connect](https://azure.microsoft.com/en-us/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/) na documentação do Azure AD.

Usaremos uma pilha de três partes do middleware [Rack](http://rack.github.io/) para habilitar o aplicativo para autenticar no Microsoft Graph:

- [OmniAuth](https://rubygems.org/gems/omniauth), uma estrutura de Rack generalizada para autenticação de provedor múltiplo.
- [Omniauth-oauth2](https://rubygems.org/gems/omniauth-oauth2), uma estratégia abstrata de OAuth2 para OmniAuth. 
- O omniauth-microsoft_v2_auth, uma estratégia do OmniAuth que personaliza o Omniauth-oauth2 para fornecer autenticação especificamente no ponto de extremidade do Azure AD v2.0. Este projeto está incluído no exemplo de código.

### <a name="specify-gem-dependencies-for-authentication"></a>Especificar dependências gem para autenticação

No Gemfile, tire os comentários das seguintes gems para adicioná-las como dependências.

    ```
    gem 'omniauth'
    gem 'omniauth-oauth2'
    gem 'omniauth-microsoft_v2_auth', path: './omniauth-microsoft_v2_auth'
    ```

Observe que `omniauth-microsoft_v2_auth` está incluído no projeto do aplicativo e será instalado a partir do caminho especificado. 

### <a name="configure-the-authentication-middleware"></a>Configurar o middleware de autenticação

No `config/initializers/omniauth-microsoft_v2_auth.rb`, tire o comentário das linhas a seguir.

    ```
    Rails.application.config.middleware.use OmniAuth::Builder do
      provider :microsoft_v2_auth,
      ENV['CLIENT_ID'],
      ENV['CLIENT_SECRET'],
      :scope => ENV['SCOPE']
    end
    ```
Isso configura o middleware OmniAuth, incluindo a especificação da ID do aplicativo e o segredo do aplicativo a ser usado, bem como os escopos a serem solicitados para o usuário. Estes são os valores que você especificou anteriormente no `config/environment.rb`.

### <a name="specify-routes-for-authentication"></a>Especificar rotas para autenticação

Agora precisamos especificar duas rotas necessárias para o fluxo de autenticação. A primeira rota encaminha a solicitação de autenticação para o middleware OmniAuth e a segunda especifica o local no aplicativo para o qual o OmniAuth deve redirecionar após a autenticação ocorrer.

No `config/routes.rb`, tire o comentário da diretiva de rota a seguir.

    get '/login', to: 'pages#login'

Isso direciona as solicitações de logon para o método `login` do controlador de páginas, que por sua vez redireciona a solicitação para o middleware omniauth-microsoft_v2_auth.

    def login
        redirect_to '/auth/microsoft_v2_auth'
      end

Em seguida, precisamos especificar onde no aplicativo OmniAuth deve redirecionar após a autenticação ocorrer. Tire o comentário da rota a seguir.

    match '/auth/:provider/callback', to: 'pages#callback', via: [:get, :post]

Quando o OmniAuth tiver terminado de autenticar o usuário, ele chamará a URL de redirecionamento especificada no registro do aplicativo; nesse caso, *http://localhost:3000/auth/microsoft_v2_auth/callback*. O padrão de rota acima corresponde a essa URL e, portanto, encaminha a solicitação para o método `callback` do controlador da página.

### <a name="get-an-access-token"></a>Obter um token de acesso

Em seguida, adicionaremos o código que realmente inicia o processo de autenticação e recupera o token de acesso assim que o usuário tiver entrado com êxito.

Dê uma olhada em `app/views/pages/index.html.erb`, o modo de exibição da raiz do site. O modo de exibição inclui um único botão que permite que os usuários entrem.

    <button class="ms-Button" onclick="window.location.href = '/login'">
        <span class="ms-Button-label"><%= t('connect_button') %></span>
    </button>

Como mostrado anteriormente, o método de logon redireciona para o middleware OmniAuth, que foi configurado com a ID do aplicativo e o segredo do aplicativo, além dos escopos para a solicitação para o usuário. Depois que o usuário for autenticado com êxito, o OmniAuth retornará um hash com o token de acesso e outras informações do usuário para o aplicativo.

Agora vamos adicionar código para manipular o retorno de chamada OmniAuth e recuperar informações desse hash. 

Em `app/controllers/pages_controller.rb`, substitua o método `callback` vazio pelo código a seguir.

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

Este método recupera o hash de autenticação e, em seguida, armazena o token de acesso, o nome de usuário e o email na sessão atual.

> **Observação:** A autenticação simples e o tratamento do token neste projeto são apresentados somente para fins ilustrativos. Em um aplicativo de produção, você provavelmente deve construir uma maneira mais eficiente de tratamento de autenticação, incluindo o tratamento seguro de token e atualização de token.

## <a name="call-microsoft-graph"></a>Chamar o Microsoft Graph

Agora você está pronto para adicionar código para chamar o Microsoft Graph. 

O modo de exibição renderizado pelo método `callback` (`app/views/pages/callback.html.erb`) inclui um formulário simples com um único botão. O formulário posta em `send_mail` e inclui um único parâmetro, o endereço de email do destinatário.
    
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

Em `app/controllers/pages_controller.rb`, substitua o método `send_mail` vazio pelo código a seguir.

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

Esse código constrói a solicitação HTTP, formata o email e, em seguida, chama o Microsoft Graph para enviar o email.

Para criar o email, o código obtém o nome de usuário do token de sessão e o endereço de email do destinatário dos parâmetros passados do formulário. O código, em seguida, lê o corpo do email de um modelo incluído no projeto, interpola o endereço de email e o nome de usuário e anexa o texto do email como o corpo da solicitação HTTP.

Para enviar o email, o código constrói a solicitação HTTP, anexa o token de acesso como um cabeçalho de autorização e, em seguida, envia a solicitação para o ponto de extremidade de enviar email.

Por fim, o código usa o código de resposta de HTTP retornado para notificar o usuário se o email foi concluído com êxito ou não.

## <a name="run-the-app"></a>Executar o aplicativo

1. Instale o aplicativo Rails e as dependências com o seguinte comando.

    ```
    bundle install
    ```
2. Para iniciar o aplicativo Rails, digite o seguinte comando.

    ```
    rackup -p 3000
    ```
3. Acesse `http://localhost:3000` no navegador da Web.

## <a name="see-also"></a>Ver também
- Experimente a API REST, usando o [Explorador do Graph](https://graph.microsoft.io/graph-explorer).
- Explorar nossos outros [exemplos do Microsoft Graph](https://github.com/microsoftgraph) no GitHub.


