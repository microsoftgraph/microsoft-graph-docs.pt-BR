# <a name="get-started-with-microsoft-graph-in-an-angularjs-app"></a>Introdução ao Microsoft Graph em um aplicativo AngularJS

Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph. Ele orienta você em relação a como criar um [Exemplo de Microsoft Connect para AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample) e explica os principais conceitos que você implementa para utilizar o Microsoft Graph. O artigo também descreve como acessar o Microsoft Graph usando o [SDK do JavaScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) ou chamadas REST não processadas.

A imagem a seguir mostra o aplicativo que você criará. 

![O aplicativo Web após o login mostrando o botão "Enviar email"](./images/angular-connect-sample.png)


**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://graph.microsoft.io/pt-BR/getting-started) para agilizar o processo.

Para baixar uma versão do exemplo de conexão que usa o ponto de extremidade do Azure AD, confira [Exemplo de conexão com o Microsoft Graph para AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth).


## <a name="prerequisites"></a>Pré-requisitos

Para começar, será necessário: 

- Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](https://docs.microsoft.com/pt-BR/office/developer-program/office-365-developer-program-faq#account-types)
- [Node.js com npm](https://nodejs.org/en/download/)
- [Bower](https://bower.io)
- O [Exemplo de conexão da Microsoft para AngularJS](https://github.com/microsoftgraph/angular-connect-sample). Você usará a pasta **starter-project** nos exemplos de arquivo para este passo a passo.

## <a name="register-the-application"></a>Registrar o aplicativo
Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e a senha que você usará para configurar o aplicativo no Visual Studio.

1. Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.

2. Escolha **Adicionar um aplicativo**.

3. Insira um nome para o aplicativo e escolha **Criar aplicativo**. 
    
    A página de registro é exibida, listando as propriedades do seu aplicativo.

4. Copie a ID do aplicativo. Este é o identificador exclusivo para o aplicativo que você usará para configurar o aplicativo.

5. Em **Plataformas**, escolha **Adicionar plataforma** > **Web**.

6. Não se esqueça de marcar a caixa **Permitir Fluxo Implícito** e insira *http://localhost:8080* como o URI de redirecionamento. 

7. Escolha **Salvar**.


## <a name="configure-the-project"></a>Configurar o projeto
1. Abra a pasta **starter-project** nos exemplos de arquivo.
2. Em um prompt de comando, execute os seguintes comandos no diretório raiz do projeto inicial. Isso instala as dependências do projeto.

        npm install  
        bower install
    
3. Nos arquivos do projeto inicial na pasta **public/scripts**, abra o config.js.
4. No campo **clientId**, substitua o valor do espaço reservado **ENTER_YOUR_CLIENT_ID** pela ID do aplicativo que você acabou de copiar.

## <a name="call-microsoft-graph-with-the-sdk"></a>Chamar o Microsoft Graph com o SDK
O aplicativo chama o Microsoft Graph para obter informações sobre o usuário e enviar um email em nome do usuário. Essas chamadas são iniciadas pelo MainController em resposta a eventos de interface do usuário.

Abra o app.js e adicione o código a seguir na parte inferior do arquivo. Isso inicializa o SDK.

    var authToken;
    var graphClient = MicrosoftGraph.Client.init({
        authProvider: function(done) {
        if (typeof authToken === "undefined") {
          done({err: "No auth token"})
        } else {
          done(null, authToken); //first parameter takes an error if you can't get an access token
        }
        }
    });

### <a name="using-the-sdk"></a>Usar o SDK
1. Em graphHelper.js, substitua *// Obter o perfil do usuário atual* pelo código a seguir. Isso configura e envia a solicitação GET para o ponto de extremidade */me* e processa a resposta.

        // Get the profile of the current user.
        me: function me() {
          return graphClient.api('/me').get();
        },
  
2. Substitua *// Enviar um email em nome do usuário atual* pelo código a seguir. Isso configura e envia a solicitação POST para o ponto de extremidade */me/sendMail* e processa a resposta.

        // Send an email on behalf of the current user.
        sendMail: function sendMail(email) {
          return graphClient.api('/me/sendMail').post({ 'message' : email, 'saveToSentItems': true });
        }

3. Na pasta **public/controllers**, abra mainController.js.

4. Substitua *// Definir os cabeçalhos padrão e as propriedades do usuário* pelo código a seguir. Isso adiciona o token de acesso à solicitação HTTP, chama **GraphHelper.me** para obter o perfil do usuário atual e processa a resposta.

        // Set the default headers and user properties.
        function processAuth() {

        // let the authProvider access the access token
        authToken = localStorage.token;

        if (localStorage.getItem('user') === null) {

          // Get the profile of the current user.
          GraphHelper.me().then(function(user) {

            // Save the user to localStorage.
            localStorage.setItem('user', angular.toJson(user));

            vm.displayName = user.displayName;
            vm.emailAddress = user.mail || user.userPrincipalName;
          });
        } else {
          let user = angular.fromJson(localStorage.user);

          vm.displayName = user.displayName;
          vm.emailAddress = user.mail || user.userPrincipalName;
        }

        }

5. Substitua *// Enviar um email em nome do usuário atual* pelo código a seguir. Isso cria a mensagem de email, chama **GraphHelper.sendMail** e processa a resposta.

        // Send an email on behalf of the current user.
        function sendMail() {

          authToken = localStorage.token;       

          // Build the HTTP request payload (the Message object).
          var email = {
          Subject: 'Welcome to Microsoft Graph development with Angular and the Microsoft Graph Connect sample',
          Body: {
            ContentType: 'HTML',
            Content: getEmailContent()
          },
          ToRecipients: [
            {
              EmailAddress: {
            Address: vm.emailAddress
              }
            }
          ]
          };

          // Save email address so it doesn't get lost with two way data binding.
          vm.emailAddressSent = vm.emailAddress;
          GraphHelper.sendMail(email)
        .then(function (response) {
          $log.debug('HTTP request to the Microsoft Graph API returned successfully.', response);
          vm.requestSuccess = true;
          vm.requestFinished = true;
          $scope.$apply();
        }, function (error) {
          $log.error('HTTP request to the Microsoft Graph API failed.');
          vm.requestSuccess = false;
          vm.requestFinished = true;
          $scope.$apply();
        });

        };

6. Salve todas as suas alterações.

## <a name="run-the-app"></a>Executar o aplicativo

1. Em um prompt de comando, execute o seguinte comando no diretório raiz do projeto inicial.

        npm start

2. Em um navegador, navegue até *http://localhost:8080* e escolha o botão **Conectar**.

3. Entre e conceda as permissões solicitadas. 

4. Como alternativa, edite o endereço de email do destinatário e escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão. 

## <a name="next-steps"></a>Próximas etapas
- Experimente a API REST usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Explorar nossos outros [exemplos de AngularJS](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) no GitHub.


## <a name="see-also"></a>Confira também
- [Protocolos do Azure AD v2.0](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-protocols/)
- [Tokens do Azure AD v2.0](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-tokens/)
