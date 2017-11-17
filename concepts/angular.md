# <a name="get-started-with-microsoft-graph-in-an-angularjs-app"></a><span data-ttu-id="b0087-101">Introdução ao Microsoft Graph em um aplicativo AngularJS</span><span class="sxs-lookup"><span data-stu-id="b0087-101">Get started with Microsoft Graph in an AngularJS app</span></span>

<span data-ttu-id="b0087-p101">Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph. Ele orienta você em relação a como criar um [Exemplo de Microsoft Connect para AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample) e explica os principais conceitos que você implementa para utilizar o Microsoft Graph. O artigo também descreve como acessar o Microsoft Graph usando o [SDK do JavaScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) ou chamadas REST não processadas.</span><span class="sxs-lookup"><span data-stu-id="b0087-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph. The article also describes how to access Microsoft Graph by using either the [Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) or raw REST calls.</span></span>

<span data-ttu-id="b0087-105">A imagem a seguir mostra o aplicativo que você criará.</span><span class="sxs-lookup"><span data-stu-id="b0087-105">The following image shows the app you'll create.</span></span> 

![O aplicativo Web após o login mostrando o botão "Enviar email"](./images/angular-connect-sample.png)


<span data-ttu-id="b0087-p102">**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) para começar a usar rapidamente.</span><span class="sxs-lookup"><span data-stu-id="b0087-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast.</span></span>

<span data-ttu-id="b0087-109">Para baixar uma versão do exemplo de conexão que usa o ponto de extremidade do Azure AD, confira [Exemplo de conexão com o Microsoft Graph para AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth).</span><span class="sxs-lookup"><span data-stu-id="b0087-109">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-rest-sample/releases/tag/last_v1_auth).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="b0087-110">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0087-110">Prerequisites</span></span>

<span data-ttu-id="b0087-111">Para começar, será necessário:</span><span class="sxs-lookup"><span data-stu-id="b0087-111">To get started, you'll need:</span></span> 

- <span data-ttu-id="b0087-112">Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="b0087-112">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- [<span data-ttu-id="b0087-113">Node.js com npm</span><span class="sxs-lookup"><span data-stu-id="b0087-113">Node.js with npm</span></span>](https://nodejs.org/en/download/)
- [<span data-ttu-id="b0087-114">Bower</span><span class="sxs-lookup"><span data-stu-id="b0087-114">Bower</span></span>](https://bower.io)
- <span data-ttu-id="b0087-p103">O [Exemplo de conexão da Microsoft para AngularJS](https://github.com/microsoftgraph/angular-connect-sample). Você usará a pasta **starter-project** nos exemplos de arquivo para este passo a passo.</span><span class="sxs-lookup"><span data-stu-id="b0087-p103">The [Microsoft Connect Sample for AngularJS](https://github.com/microsoftgraph/angular-connect-sample). You'll use the **starter-project** folder in the sample files for this walkthrough.</span></span>

## <a name="register-the-application"></a><span data-ttu-id="b0087-117">Registrar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0087-117">Register the application</span></span>
<span data-ttu-id="b0087-p104">Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e a senha que você usará para configurar o aplicativo no Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="b0087-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="b0087-120">Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="b0087-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="b0087-121">Escolha **Adicionar um aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="b0087-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="b0087-122">Insira um nome para o aplicativo e escolha **Criar aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="b0087-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="b0087-123">A página de registro é exibida, listando as propriedades do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0087-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="b0087-p105">Copie a ID do aplicativo. Este é o identificador exclusivo para o aplicativo que você usará para configurar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0087-p105">Copy the application ID. This is the unique identifier for your app that you'll use to configure the app.</span></span>

5. <span data-ttu-id="b0087-126">Em **Plataformas**, escolha **Adicionar plataforma** > **Web**.</span><span class="sxs-lookup"><span data-stu-id="b0087-126">Under **Platforms**, choose **Add Platform** > **Web**.</span></span>

6. <span data-ttu-id="b0087-127">Não deixe de marcar a caixa de diálogo **Permitir Fluxo Implícito** e insira *http://localhost:8080* como o URI de Redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="b0087-127">Make sure the **Allow Implicit Flow** check box is selected, and enter *http://localhost:8080* as the Redirect URI.</span></span> 

7. <span data-ttu-id="b0087-128">Escolha **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="b0087-128">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="b0087-129">Configurar o projeto</span><span class="sxs-lookup"><span data-stu-id="b0087-129">Configure the project</span></span>
1. <span data-ttu-id="b0087-130">Abra a pasta **starter-project** nos exemplos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="b0087-130">Open the **starter-project** folder in the sample files.</span></span>
2. <span data-ttu-id="b0087-p106">Em um prompt de comando, execute os seguintes comandos no diretório raiz do projeto inicial. Isso instala as dependências do projeto.</span><span class="sxs-lookup"><span data-stu-id="b0087-p106">In a command prompt, run the following commands in the root directory of the starter project. This installs the project dependencies.</span></span>

        npm install  
        bower install
    
3. <span data-ttu-id="b0087-133">Nos arquivos do projeto inicial na pasta **public/scripts**, abra o config.js.</span><span class="sxs-lookup"><span data-stu-id="b0087-133">In the starter project files, in the **public/scripts** folder, open config.js.</span></span>
4. <span data-ttu-id="b0087-134">No campo **clientId**, substitua o valor do espaço reservado **ENTER_YOUR_CLIENT_ID** pela ID do aplicativo que você acabou de copiar.</span><span class="sxs-lookup"><span data-stu-id="b0087-134">In the **clientID** field, replace the **ENTER_YOUR_CLIENT_ID** placeholder value with the application ID you just copied.</span></span>

## <a name="call-microsoft-graph-with-the-sdk"></a><span data-ttu-id="b0087-135">Chamar o Microsoft Graph com o SDK</span><span class="sxs-lookup"><span data-stu-id="b0087-135">Call Microsoft Graph with the SDK</span></span>
<span data-ttu-id="b0087-p107">O aplicativo chama o Microsoft Graph para obter informações sobre o usuário e enviar um email em nome do usuário. Essas chamadas são iniciadas pelo MainController em resposta a eventos de interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="b0087-p107">The app calls Microsoft Graph to get user information and to send an email on the user's behalf. These calls are initiated from the MainController in response to UI events.</span></span>

<span data-ttu-id="b0087-p108">Abra o app.js e adicione o código a seguir na parte inferior do arquivo. Isso inicializa o SDK.</span><span class="sxs-lookup"><span data-stu-id="b0087-p108">Open app.js and add the following code to the bottom of the file. This initializes the SDK.</span></span>

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

### <a name="using-the-sdk"></a><span data-ttu-id="b0087-140">Usar o SDK</span><span class="sxs-lookup"><span data-stu-id="b0087-140">Using the SDK</span></span>
1. <span data-ttu-id="b0087-p109">Em graphHelper.js, substitua *// Obter o perfil do usuário atual* pelo código a seguir. Isso configura e envia a solicitação GET para o ponto de extremidade */me* e processa a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0087-p109">In graphHelper.js, replace *// Get the profile of the current user* with the following code. This configures and sends the GET request to the */me* endpoint, and processes the response.</span></span>

        // Get the profile of the current user.
        me: function me() {
          return graphClient.api('/me').get();
        },
  
2. <span data-ttu-id="b0087-p110">Substitua *// Enviar um email em nome do usuário atual* pelo código a seguir. Isso configura e envia a solicitação POST para o ponto de extremidade */me/sendMail* e processa a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0087-p110">Replace *// Send an email on behalf of the current user* with the following code. This configures and sends the POST request to the */me/sendMail* endpoint, and processes the response.</span></span>

        // Send an email on behalf of the current user.
        sendMail: function sendMail(email) {
          return graphClient.api('/me/sendMail').post({ 'message' : email, 'saveToSentItems': true });
        }

3. <span data-ttu-id="b0087-145">Na pasta **public/controllers**, abra mainController.js.</span><span class="sxs-lookup"><span data-stu-id="b0087-145">In the **public/controllers** folder, open mainController.js.</span></span>

4. <span data-ttu-id="b0087-p111">Substitua *// Definir os cabeçalhos padrão e as propriedades do usuário* pelo código a seguir. Isso adiciona o token de acesso à solicitação HTTP, chama **GraphHelper.me** para obter o perfil do usuário atual e processa a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0087-p111">Replace *// Set the default headers and user properties* with the following code. This adds the access token to the HTTP request, calls **GraphHelper.me** to get the current user's profile, and processes the response.</span></span>

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

5. <span data-ttu-id="b0087-p112">Substitua *// Enviar um email em nome do usuário atual* pelo código a seguir. Isso cria a mensagem de email, chama **GraphHelper.sendMail** e processa a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0087-p112">Replace *// Send an email on behalf of the current user* with the following code. This builds the email message, calls **GraphHelper.sendMail**, and processes the response.</span></span>

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

6. <span data-ttu-id="b0087-150">Salve todas as suas alterações.</span><span class="sxs-lookup"><span data-stu-id="b0087-150">Save all your changes.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="b0087-151">Executar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0087-151">Run the app</span></span>

1. <span data-ttu-id="b0087-152">Em um prompt de comando, execute o seguinte comando no diretório raiz do projeto inicial.</span><span class="sxs-lookup"><span data-stu-id="b0087-152">In a command prompt, run the following command in the root directory of the starter project.</span></span>

        npm start

2. <span data-ttu-id="b0087-153">Em um navegador, acesse *http://localhost:8080* e escolha o botão **Connect**.</span><span class="sxs-lookup"><span data-stu-id="b0087-153">In a browser, navigate to *http://localhost:8080* and choose the **Connect** button.</span></span>

3. <span data-ttu-id="b0087-154">Entre e conceda as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="b0087-154">Sign in and grant the requested permissions.</span></span> 

4. <span data-ttu-id="b0087-p113">Como alternativa, edite o endereço de email do destinatário e escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão.</span><span class="sxs-lookup"><span data-stu-id="b0087-p113">Optionally edit the recipient's email address, and then choose the **Send mail** button. When the mail is sent, a Success message is displayed below the button.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="b0087-157">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="b0087-157">Next steps</span></span>
- <span data-ttu-id="b0087-158">Experimente a API REST usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="b0087-158">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="b0087-159">Explorar nossos outros [exemplos de AngularJS](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="b0087-159">Explore our other [AngularJS samples](https://github.com/search?utf8=%E2%9C%93&q=angular+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) on GitHub.</span></span>


## <a name="see-also"></a><span data-ttu-id="b0087-160">Ver também</span><span class="sxs-lookup"><span data-stu-id="b0087-160">See also</span></span>
- [<span data-ttu-id="b0087-161">Protocolos do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="b0087-161">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="b0087-162">Tokens do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="b0087-162">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
