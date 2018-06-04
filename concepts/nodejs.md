# <a name="get-started-with-microsoft-graph-in-a-nodejs-app"></a><span data-ttu-id="d3bc0-101">Introdução ao Microsoft Graph em um aplicativo Node.js</span><span class="sxs-lookup"><span data-stu-id="d3bc0-101">Get started with Microsoft Graph in a Node.js app</span></span>

<span data-ttu-id="d3bc0-102">Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-102">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph.</span></span> <span data-ttu-id="d3bc0-103">Ele orienta você em relação a como criar um [Exemplo de conexão da Microsoft para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) e explica os principais conceitos que você implementa para utilizar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-103">It walks you through building the [Microsoft Connect sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph.</span></span> <span data-ttu-id="d3bc0-104">O artigo descreve como acessar a API do Microsoft Graph usando chamadas REST não processadas.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-104">The article describes how to access the Microsoft Graph API by using raw REST calls.</span></span> <span data-ttu-id="d3bc0-105">Se você estiver interessado na criação de um aplicativo Node.js que se conecta ao Microsoft Graph com um SDK de JavaScript, confira nosso [Exemplo de conexão do Node.js do Microsoft Graph baseado em SDK](https://github.com/microsoftgraph/nodejs-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="d3bc0-105">If you're interested in building a Node.js app that connects to Microsoft Graph with the JavaScript SDK, see our [Microsoft Graph SDK-based Node.js Connect sample](https://github.com/microsoftgraph/nodejs-connect-sample).</span></span>

<span data-ttu-id="d3bc0-106">A imagem a seguir mostra o aplicativo que você criará.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-106">The following image shows is the app you'll create.</span></span> 

![O aplicativo Web após o login mostrando o botão "Enviar email"](./images/web-screenshot.png)


<span data-ttu-id="d3bc0-p102">**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://graph.microsoft.io/pt-BR/getting-started) para agilizar o processo.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/pt-BR/getting-started) to get up and running fast.</span></span>

<span data-ttu-id="d3bc0-110">Para baixar uma versão do exemplo de conexão que usa o ponto de extremidade do Azure AD, confira [Exemplo de conexão com o Microsoft Graph para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth).</span><span class="sxs-lookup"><span data-stu-id="d3bc0-110">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="d3bc0-111">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3bc0-111">Prerequisites</span></span>

<span data-ttu-id="d3bc0-112">Para começar, será necessário:</span><span class="sxs-lookup"><span data-stu-id="d3bc0-112">To get started, you'll need:</span></span> 

- <span data-ttu-id="d3bc0-113">Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](https://docs.microsoft.com/pt-BR/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="d3bc0-113">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/pt-BR/office/developer-program/office-365-developer-program-faq#account-types)</span></span>
- [<span data-ttu-id="d3bc0-114">Node.js com npm</span><span class="sxs-lookup"><span data-stu-id="d3bc0-114">Node.js with npm</span></span>](https://nodejs.org/en/download/) 
- <span data-ttu-id="d3bc0-115">O [Exemplo de conexão da Microsoft para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="d3bc0-115">The [Microsoft Connect sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span></span> <span data-ttu-id="d3bc0-116">Você usará a pasta **starter-project** nos exemplos de arquivo para este passo a passo.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-116">You'll use the **starter-project** folder in the sample files for this walkthrough.</span></span>

## <a name="register-the-application"></a><span data-ttu-id="d3bc0-117">Registrar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3bc0-117">Register the application</span></span>
<span data-ttu-id="d3bc0-p104">Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e a senha que você usará para configurar o aplicativo no Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="d3bc0-120">Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="d3bc0-121">Escolha **Adicionar um aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="d3bc0-122">Insira um nome para o aplicativo e escolha **Criar aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="d3bc0-123">A página de registro é exibida, listando as propriedades do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="d3bc0-p105">Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p105">Copy the application ID. This is the unique identifier for your app.</span></span> 

5. <span data-ttu-id="d3bc0-p106">Em **Segredos do Aplicativo**, escolha **Gerar Nova Senha**. Copie a senha da caixa de diálogo **Nova senha gerada**.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p106">Under **Application Secrets**, choose **Generate New Password**. Copy the password from the **New password generated** dialog.</span></span>

    <span data-ttu-id="d3bc0-128">Você usará a ID do aplicativo e a senha do aplicativo (segredo) para configurar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-128">You'll use the application ID and application password (secret) to configure the app.</span></span> 

6. <span data-ttu-id="d3bc0-129">Em **Plataformas**, escolha **Adicionar plataforma** > **Web**.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-129">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="d3bc0-130">Insira *http://localhost:3000/token* como o URI de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-130">Enter http://localhost:3000/token as the Redirect URI.</span></span> 

8. <span data-ttu-id="d3bc0-131">Escolha **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-131">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="d3bc0-132">Configurar o projeto</span><span class="sxs-lookup"><span data-stu-id="d3bc0-132">Configure the project</span></span>
1. <span data-ttu-id="d3bc0-133">Abra a pasta **starter-project** nos exemplos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-133">Open the **starter-project** folder in the sample files.</span></span>

1. <span data-ttu-id="d3bc0-p107">Em um prompt de comando, execute o seguinte comando no diretório raiz do projeto inicial. Isso instala as dependências do projeto.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p107">In a command prompt, run the following command in the root directory of the starter project. This installs the project dependencies.</span></span>

        npm install

1. <span data-ttu-id="d3bc0-136">Nos arquivos de projeto inicial, abra utils\config.js.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-136">In the starter project files, open utils\config.js.</span></span>


1. <span data-ttu-id="d3bc0-137">No campo **Credenciais**, substitua os valores de espaço reservado **ENTER\_YOUR\_CLIENT\_ID** e **ENTER\_YOUR\_SECRET** pelos valores que você acabou de copiar.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-137">In the **credentials** field, replace the **ENTER\_YOUR\_CLIENT\_ID** and **ENTER\_YOUR\_SECRET** placeholder values with the values you just copied.</span></span>

  
## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="d3bc0-138">Autenticar o usuário e obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="d3bc0-138">Authenticate the user and get an access token</span></span>
<span data-ttu-id="d3bc0-p108">Nesta etapa, você adicionará o código de gerenciamento de conexão e token. Mas primeiro, vamos examinar mais detalhadamente o fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p108">In this step, you'll add sign-in and token management code. But first, let's take a closer look at the auth flow.</span></span>

<span data-ttu-id="d3bc0-p109">Este aplicativo usa o fluxo de concessão do código de autorização com uma identidade de usuário delegada. Para um aplicativo Web, o fluxo exige a ID do aplicativo, o segredo e o URI de redirecionamento do aplicativo registrado.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p109">This app uses the authorization code grant flow with a delegated user identity. For a web application, the flow requires the application ID, secret, and redirect URI from the registered app.</span></span> 

<span data-ttu-id="d3bc0-143">O fluxo de autenticação pode ser dividido nestas etapas básicas:</span><span class="sxs-lookup"><span data-stu-id="d3bc0-143">The auth flow can be broken down into these basic steps:</span></span>

1. <span data-ttu-id="d3bc0-144">Redirecione o usuário para autenticação e autorização.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-144">Redirect the user for authentication and consent</span></span>
2. <span data-ttu-id="d3bc0-145">Obter um código de autorização</span><span class="sxs-lookup"><span data-stu-id="d3bc0-145">Get an authorization code</span></span>
3. <span data-ttu-id="d3bc0-146">Resgatar o código de autorização para solicitar um token de acesso</span><span class="sxs-lookup"><span data-stu-id="d3bc0-146">Redeem the authorization code for an access token</span></span>
4. <span data-ttu-id="d3bc0-147">Use o token de atualização para obter um novo token de acesso quando o token de acesso expirar.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-147">Use the refresh token to get a new access token when the access token expires</span></span>

<span data-ttu-id="d3bc0-p110">O aplicativo usa o middleware [oauth](https://www.npmjs.com/package/oauth) para autenticar e obter tokens. Ele usa o middleware [cookie-parser](https://www.npmjs.com/package/cookie-parser) para armazenar em cache informações de token em cookies. O código utilizado para armazenar e acessar informações de token é encontrado no controlador index.js.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p110">The app uses the [oauth](https://www.npmjs.com/package/oauth) middleware to authenticate and obtain tokens. It uses the [cookie-parser](https://www.npmjs.com/package/cookie-parser) middleware to cache token information in cookies. The code used to store and access token information is found in the index.js controller.</span></span>
    
   ><span data-ttu-id="d3bc0-p111">**Importante** O tratamento simples de autenticação e token neste projeto é apenas para fins de exemplo. Em um aplicativo de produção, você deve construir uma maneira mais eficiente de tratamento de autenticação, incluindo validação e tratamento seguro de token.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p111">**Important** The simple authentication and token handling in this project is for sample purposes only. In a production app, you should construct a more robust way of handling authentication, including validation and secure token handling.</span></span>

<span data-ttu-id="d3bc0-153">Agora você está pronto para adicionar código para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-153">Now you're ready to add code to call Microsoft Graph.</span></span> 

## <a name="call-microsoft-graph"></a><span data-ttu-id="d3bc0-154">Chamar o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d3bc0-154">Call Microsoft Graph</span></span>
<span data-ttu-id="d3bc0-p112">O aplicativo chama o Microsoft Graph para obter informações sobre o usuário e enviar um email em nome do usuário. Essas chamadas são iniciadas pelo controlador index.js em resposta a eventos de interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p112">The app calls Microsoft Graph to get user information and to send an email on the user's behalf. These calls are initiated from the index.js controller in response to UI events.</span></span>

1. <span data-ttu-id="d3bc0-157">Abra utils\graphHelper.js.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-157">Open utils\graphHelper.js.</span></span>

1. <span data-ttu-id="d3bc0-p113">Substitua a função **getUserData** pelo seguinte código. Isso configura e envia a solicitação GET para o ponto de extremidade */me* e processa a resposta.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p113">Replace the **getUserData** function with the following code. This configures and sends the GET request to the */me* endpoint and processes the response.</span></span>

        function getUserData(accessToken, callback) {
          request
           .get('https://graph.microsoft.com/v1.0/me')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             callback(err, res);
           });
        }

1. <span data-ttu-id="d3bc0-p114">Substitua a função **getProfilePhoto** pelo seguinte código. Isso configura e envia a solicitação GET para o ponto de extremidade */me/photo/$value* e processa a resposta. Observe que as fotos do perfil não estão atualmente disponíveis para contas MSA.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p114">Replace the **getProfilePhoto** function with the following code. This configures and sends the GET request to the */me/photo/$value* endpoint and processes the response. Note that profile photos aren't currently available for MSA accounts.</span></span>
    
        function getProfilePhoto(accessToken, callback) {
          // Get the profile photo of the current user (from the user's mailbox on Exchange Online).
          // This operation in version 1.0 supports only work or school mailboxes, not personal mailboxes.
          request
           .get('https://graph.microsoft.com/v1.0/me/photo/$value')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             // Returns 200 OK and the photo in the body. If no photo exists, returns 404 Not Found.
             callback(err, res.body);
           });
        }

1. <span data-ttu-id="d3bc0-p115">Substitua a função **uploadFile** pelo seguinte código. Isso configura e envia a solicitação PUT para o ponto de extremidade */me/drive/root/children/mypic.jpg/content* e processa a resposta. Se o arquivo existir, essa solicitação atualiza o conteúdo. Se não existir, ela cria o arquivo e carrega o conteúdo da foto do perfil.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p115">Replace the **uploadFile** function with the following code. This configures and sends the PUT request to the */me/drive/root/children/mypic.jpg/content* endpoint. If the file exists, this requests updates the content. If it doesn't exist, it creates the file and uploads the contents of the profile photo.</span></span> 

        function uploadFile(accessToken, file, callback) {
          // This operation only supports files up to 4MB in size.
          // To upload larger files, see `https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/item_createUploadSession`.
          request
           .put('https://graph.microsoft.com/v1.0/me/drive/root/children/mypic.jpg/content')
           .send(file)
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'image/jpg')
           .end((err, res) => {
             // Returns 200 OK and the file metadata in the body.
             callback(err, res.body);
           });
        }

1. <span data-ttu-id="d3bc0-p116">Substitua a função **getSharingLink** pelo seguinte código. Isso configura e envia a solicitação GET para o ponto de extremidade */me/drive/items/{file id}/createLink* e processa o resultado. O resultado é um link de compartilhamento para o arquivo que será incluído na mensagem.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p116">Replace the **getSharingLink** function with the following code. This configures and sends the GET request to the */me/drive/items/{file id}/createLink* endpoint and processes the result. The result is a sharing link to the file that will be included in the message.</span></span>

        function getSharingLink(accessToken, id, callback) {
          request
           .post('https://graph.microsoft.com/v1.0/me/drive/items/' + id + '/createLink')
           .send({ type: 'view' })
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'application/json')
           .end((err, res) => {
             // Returns 200 OK and the permission with the link in the body.
             callback(err, res.body.link);
           });
        }

1. <span data-ttu-id="d3bc0-p117">Substitua a função **postSendMail** pelo seguinte código. Isso configura e envia a solicitação POST para o ponto de extremidade */me/sendMail* e processa a resposta.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p117">Replace the **postSendMail** function with the following code. This configures and sends the POST request to the */me/sendMail* endpoint and processes the response.</span></span>

        function postSendMail(accessToken, message, callback) {
          request
           .post('https://graph.microsoft.com/v1.0/me/sendMail')
           .send(message)
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'application/json')
           .set('Content-Length', message.length)
           .end((err, res) => {
             // Returns 202 if successful.
             // Note: If you receive a 500 - Internal Server Error
             // while using a Microsoft account (outlook.com, hotmail.com or live.com),
             // it's possible that your account has not been migrated to support this flow.
             // Check the inner error object for code 'ErrorInternalServerTransientError'.
             // You can try using a newly created Microsoft account or contact support.
             callback(err, res);
           });
        }

1. <span data-ttu-id="d3bc0-172">Abra utils\emailer.js.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-172">Open utils\emailer.js.</span></span>

1. <span data-ttu-id="d3bc0-p118">Substitua a função **wrapEmail** pelo seguinte código. Isso cria a carga que representa a mensagem de email a ser enviada.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p118">Replace the **wrapEmail** function with the following code. This builds the payload that represents the email message to send.</span></span>

        function wrapEmail(content, recipient, file) {
          const attachments = [{
            '@odata.type': '#microsoft.graph.fileAttachment',
            ContentBytes: file,
            Name: 'mypic.jpg'
          }];
          const emailAsPayload = {
            Message: {
              Subject: 'Welcome to Microsoft Graph development with Node.js and the Microsoft Graph Connect sample',
              Body: {
                ContentType: 'HTML',
                Content: content
              },
              ToRecipients: [
                {
                  EmailAddress: {
                    Address: recipient
                  }
                }
              ]
            },
            SaveToSentItems: true,
            Attachments: attachments
          };
          return emailAsPayload;
        }

## <a name="run-the-app"></a><span data-ttu-id="d3bc0-175">Executar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3bc0-175">Run the app</span></span>

1. <span data-ttu-id="d3bc0-176">Em um prompt de comando, execute o seguinte comando no diretório raiz do projeto inicial.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-176">In a command prompt, run the following command in the root directory of the starter project.</span></span>


        npm start

1. <span data-ttu-id="d3bc0-177">Em um navegador, navegue até *http://localhost:3000* e escolha o botão **Conectar ao Office 365**.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-177">In a browser, navigate to http://localhost:3000 and choose the Connect to Office 365 button.</span></span>

1. <span data-ttu-id="d3bc0-178">Entre e conceda as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-178">Sign in and grant the requested permissions.</span></span> 

1. <span data-ttu-id="d3bc0-p119">Como alternativa, edite o endereço de email do destinatário e escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-p119">Optionally edit the recipient's email address, and then choose the **Send mail** button. When the mail is sent, a Success message is displayed below the button.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="d3bc0-181">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="d3bc0-181">Next steps</span></span>
- <span data-ttu-id="d3bc0-182">Experimente a API REST usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="d3bc0-182">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="d3bc0-183">Explore nossos outros [exemplos de Node.js](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="d3bc0-183">Explore our other [Node.js samples](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) on GitHub.</span></span>
- <span data-ttu-id="d3bc0-184">Use os [tipos de TypeScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-typescript-typings)</span><span class="sxs-lookup"><span data-stu-id="d3bc0-184">Use the [Microsoft Graph TypeScript types](https://github.com/microsoftgraph/msgraph-typescript-typings)</span></span>
- <span data-ttu-id="d3bc0-185">Experimente a [SDK de JavaScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript)</span><span class="sxs-lookup"><span data-stu-id="d3bc0-185">Try the [Microsoft Graph JavaScript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript)</span></span>

## <a name="see-also"></a><span data-ttu-id="d3bc0-186">Confira também</span><span class="sxs-lookup"><span data-stu-id="d3bc0-186">See also</span></span>
- [<span data-ttu-id="d3bc0-187">Protocolos do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="d3bc0-187">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="d3bc0-188">Tokens do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="d3bc0-188">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-tokens/)
- [<span data-ttu-id="d3bc0-189">Exemplo de conexão do Node.js do Microsoft Graph baseado na SDK de JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3bc0-189">Microsoft Graph JavaScript SDK Node.js Connect sample</span></span>](https://github.com/microsoftgraph/nodejs-connect-sample)
