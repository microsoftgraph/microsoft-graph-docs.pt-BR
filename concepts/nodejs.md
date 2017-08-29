# <a name="get-started-with-microsoft-graph-in-a-nodejs-app"></a><span data-ttu-id="573b9-101">Introdução ao Microsoft Graph em um aplicativo Node.js</span><span class="sxs-lookup"><span data-stu-id="573b9-101">Get started with Microsoft Graph in a Node.js app</span></span>

<span data-ttu-id="573b9-p101">Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph. Ele orienta você em relação a como criar um [Exemplo de conexão da Microsoft para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) e explica os principais conceitos que você implementa para utilizar o Microsoft Graph. O artigo descreve como acessar a API do Microsoft Graph usando chamadas REST não processadas.</span><span class="sxs-lookup"><span data-stu-id="573b9-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) and explains the main concepts that you implement to use Microsoft Graph. The article describes how to access the Microsoft Graph API by using raw REST calls.</span></span>

<span data-ttu-id="573b9-105">A imagem a seguir mostra o aplicativo que você criará.</span><span class="sxs-lookup"><span data-stu-id="573b9-105">The following image shows is the app you'll create.</span></span> 

![O aplicativo Web após o login mostrando o botão "Enviar email"](./images/web-screenshot.png)


<span data-ttu-id="573b9-p102">**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) para começar a usar rapidamente.</span><span class="sxs-lookup"><span data-stu-id="573b9-p102">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/en-us/getting-started) to get up and running fast.</span></span>

<span data-ttu-id="573b9-109">Para baixar uma versão do exemplo de conexão que usa o ponto de extremidade do Azure AD, confira [Exemplo de conexão com o Microsoft Graph para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth).</span><span class="sxs-lookup"><span data-stu-id="573b9-109">To download a version of the Connect sample that uses the Azure AD endpoint, see [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth).</span></span>


## <a name="prerequisites"></a><span data-ttu-id="573b9-110">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="573b9-110">Prerequisites</span></span>

<span data-ttu-id="573b9-111">Para começar, será necessário:</span><span class="sxs-lookup"><span data-stu-id="573b9-111">To get started, you'll need:</span></span> 

- <span data-ttu-id="573b9-112">Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="573b9-112">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- [<span data-ttu-id="573b9-113">Node.js com npm</span><span class="sxs-lookup"><span data-stu-id="573b9-113">Node.js with npm</span></span>](https://nodejs.org/en/download/) 
- <span data-ttu-id="573b9-p103">O [Exemplo de conexão da Microsoft para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample). Você usará a pasta **starter-project** nos exemplos de arquivo para este passo a passo.</span><span class="sxs-lookup"><span data-stu-id="573b9-p103">The [Microsoft Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample). You'll use the **starter-project** folder in the sample files for this walkthrough.</span></span>

## <a name="register-the-application"></a><span data-ttu-id="573b9-116">Registrar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="573b9-116">Register the application</span></span>
<span data-ttu-id="573b9-p104">Registre um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e a senha que você usará para configurar o aplicativo no Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="573b9-p104">Register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="573b9-119">Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="573b9-119">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="573b9-120">Escolha **Adicionar um aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="573b9-120">Choose **Add an app**.</span></span>

3. <span data-ttu-id="573b9-121">Insira um nome para o aplicativo e escolha **Criar aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="573b9-121">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="573b9-122">A página de registro é exibida, listando as propriedades do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="573b9-122">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="573b9-p105">Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="573b9-p105">Copy the application ID. This is the unique identifier for your app.</span></span> 

5. <span data-ttu-id="573b9-p106">Em **Segredos do Aplicativo**, escolha **Gerar Nova Senha**. Copie a senha da caixa de diálogo **Nova senha gerada**.</span><span class="sxs-lookup"><span data-stu-id="573b9-p106">Under **Application Secrets**, choose **Generate New Password**. Copy the password from the **New password generated** dialog.</span></span>

    <span data-ttu-id="573b9-127">Você usará a ID do aplicativo e a senha do aplicativo (segredo) para configurar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="573b9-127">You'll use the application ID and application password (secret) to configure the app.</span></span> 

6. <span data-ttu-id="573b9-128">Em **Plataformas**, escolha **Adicionar plataforma** > **Web**.</span><span class="sxs-lookup"><span data-stu-id="573b9-128">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="573b9-129">Insira *http://localhost:3000/token* como o URI de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="573b9-129">Enter *http://localhost:3000/token* as the Redirect URI.</span></span> 

8. <span data-ttu-id="573b9-130">Escolha **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="573b9-130">Choose **Save**.</span></span>


## <a name="configure-the-project"></a><span data-ttu-id="573b9-131">Configurar o projeto</span><span class="sxs-lookup"><span data-stu-id="573b9-131">Configure the project</span></span>
1. <span data-ttu-id="573b9-132">Abra a pasta **starter-project** nos exemplos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="573b9-132">Open the **starter-project** folder in the sample files.</span></span>

1. <span data-ttu-id="573b9-p107">Em um prompt de comando, execute o seguinte comando no diretório raiz do projeto inicial. Isso instala as dependências do projeto.</span><span class="sxs-lookup"><span data-stu-id="573b9-p107">In a command prompt, run the following command in the root directory of the starter project. This installs the project dependencies.</span></span>

        npm install

1. <span data-ttu-id="573b9-135">Nos arquivos de projeto inicial, abra utils\config.js.</span><span class="sxs-lookup"><span data-stu-id="573b9-135">In the starter project files, open utils\config.js.</span></span>


1. <span data-ttu-id="573b9-136">No campo **Credenciais**, substitua os valores de espaço reservado **ENTER\_YOUR\_CLIENT\_ID** e **ENTER\_YOUR\_SECRET** pelos valores que você acabou de copiar.</span><span class="sxs-lookup"><span data-stu-id="573b9-136">In the **credentials** field, replace the **ENTER\_YOUR\_CLIENT\_ID** and **ENTER\_YOUR\_SECRET** placeholder values with the values you just copied.</span></span>

  
## <a name="authenticate-the-user-and-get-an-access-token"></a><span data-ttu-id="573b9-137">Autenticar o usuário e obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="573b9-137">Authenticate the user and get an access token</span></span>
<span data-ttu-id="573b9-p108">Nesta etapa, você adicionará o código de gerenciamento de conexão e token. Mas primeiro, vamos examinar mais detalhadamente o fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="573b9-p108">In this step, you'll add sign-in and token management code. But first, let's take a closer look at the auth flow.</span></span>

<span data-ttu-id="573b9-p109">Este aplicativo usa o fluxo de concessão do código de autorização com uma identidade de usuário delegada. Para um aplicativo Web, o fluxo exige a ID do aplicativo, o segredo e o URI de redirecionamento do aplicativo registrado.</span><span class="sxs-lookup"><span data-stu-id="573b9-p109">This app uses the authorization code grant flow with a delegated user identity. For a web application, the flow requires the application ID, secret, and redirect URI from the registered app.</span></span> 

<span data-ttu-id="573b9-142">O fluxo de autenticação pode ser dividido nestas etapas básicas:</span><span class="sxs-lookup"><span data-stu-id="573b9-142">The auth flow can be broken down into these basic steps:</span></span>

1. <span data-ttu-id="573b9-143">Redirecione o usuário para autenticação e autorização.</span><span class="sxs-lookup"><span data-stu-id="573b9-143">Redirect the user for authentication and consent</span></span>
2. <span data-ttu-id="573b9-144">Obter um código de autorização</span><span class="sxs-lookup"><span data-stu-id="573b9-144">Get an authorization code</span></span>
3. <span data-ttu-id="573b9-145">Resgatar o código de autorização para solicitar um token de acesso</span><span class="sxs-lookup"><span data-stu-id="573b9-145">Redeem the authorization code for an access token</span></span>
4. <span data-ttu-id="573b9-146">Use o token de atualização para obter um novo token de acesso quando o token de acesso expirar.</span><span class="sxs-lookup"><span data-stu-id="573b9-146">Use the refresh token to get a new access token when the access token expires</span></span>

<span data-ttu-id="573b9-p110">O aplicativo usa o middleware [oauth](https://www.npmjs.com/package/oauth) para autenticar e obter tokens. Ele usa o middleware [cookie-parser](https://www.npmjs.com/package/cookie-parser) para armazenar em cache informações de token em cookies. O código utilizado para armazenar e acessar informações de token é encontrado no controlador index.js.</span><span class="sxs-lookup"><span data-stu-id="573b9-p110">The app uses the [oauth](https://www.npmjs.com/package/oauth) middleware to authenticate and obtain tokens. It uses the [cookie-parser](https://www.npmjs.com/package/cookie-parser) middleware to cache token information in cookies. The code used to store and access token information is found in the index.js controller.</span></span>
    
   ><span data-ttu-id="573b9-p111">**Importante** O tratamento simples de autenticação e token neste projeto é apenas para fins de exemplo. Em um aplicativo de produção, você deve construir uma maneira mais eficiente de tratamento de autenticação, incluindo validação e tratamento seguro de token.</span><span class="sxs-lookup"><span data-stu-id="573b9-p111">**Important** The simple authentication and token handling in this project is for sample purposes only. In a production app, you should construct a more robust way of handling authentication, including validation and secure token handling.</span></span>

<span data-ttu-id="573b9-152">Agora você está pronto para adicionar código para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="573b9-152">Now you're ready to add code to call Microsoft Graph.</span></span> 

## <a name="call-microsoft-graph"></a><span data-ttu-id="573b9-153">Chamar o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="573b9-153">Call Microsoft Graph</span></span>
<span data-ttu-id="573b9-p112">O aplicativo chama o Microsoft Graph para obter informações sobre o usuário e enviar um email em nome do usuário. Essas chamadas são iniciadas pelo controlador index.js em resposta a eventos de interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="573b9-p112">The app calls Microsoft Graph to get user information and to send an email on the user's behalf. These calls are initiated from the index.js controller in response to UI events.</span></span>

1. <span data-ttu-id="573b9-156">Abra utils\graphHelper.js.</span><span class="sxs-lookup"><span data-stu-id="573b9-156">Open utils\graphHelper.js.</span></span>

1. <span data-ttu-id="573b9-p113">Substitua a função **getUserData** pelo seguinte código. Isso configura e envia a solicitação GET para o ponto de extremidade */me* e processa a resposta.</span><span class="sxs-lookup"><span data-stu-id="573b9-p113">Replace the **getUserData** function with the following code. This configures and sends the GET request to the */me* endpoint and processes the response.</span></span>

        function getUserData(accessToken, callback) {
          request
           .get('https://graph.microsoft.com/v1.0/me')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             callback(err, res);
           });
        }

1. <span data-ttu-id="573b9-p114">Substitua a função **getProfilePhoto** pelo seguinte código. Isso configura e envia a solicitação GET para o ponto de extremidade */me/photo/$value* e processa a resposta. Observe que as fotos do perfil não estão atualmente disponíveis para contas MSA.</span><span class="sxs-lookup"><span data-stu-id="573b9-p114">Replace the **getProfilePhoto** function with the following code. This configures and sends the GET request to the */me/photo/$value* endpoint and processes the response. Note that profile photos aren't currently available for MSA accounts.</span></span>
    
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

1. <span data-ttu-id="573b9-p115">Substitua a função **uploadFile** pelo seguinte código. Isso configura e envia a solicitação PUT para o ponto de extremidade */me/drive/root/children/mypic.jpg/content* e processa a resposta. Se o arquivo existir, essa solicitação atualiza o conteúdo. Se não existir, ela cria o arquivo e carrega o conteúdo da foto do perfil.</span><span class="sxs-lookup"><span data-stu-id="573b9-p115">Replace the **uploadFile** function with the following code. This configures and sends the PUT request to the */me/drive/root/children/mypic.jpg/content* endpoint. If the file exists, this requests updates the content. If it doesn't exist, it creates the file and uploads the contents of the profile photo.</span></span> 

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

1. <span data-ttu-id="573b9-p116">Substitua a função **getSharingLink** pelo seguinte código. Isso configura e envia a solicitação GET para o ponto de extremidade */me/drive/items/{file id}/createLink* e processa o resultado. O resultado é um link de compartilhamento para o arquivo que será incluído na mensagem.</span><span class="sxs-lookup"><span data-stu-id="573b9-p116">Replace the **getSharingLink** function with the following code. This configures and sends the GET request to the */me/drive/items/{file id}/createLink* endpoint and processes the result. The result is a sharing link to the file that will be included in the message.</span></span>

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

1. <span data-ttu-id="573b9-p117">Substitua a função **postSendMail** pelo seguinte código. Isso configura e envia a solicitação POST para o ponto de extremidade */me/sendMail* e processa a resposta.</span><span class="sxs-lookup"><span data-stu-id="573b9-p117">Replace the **postSendMail** function with the following code. This configures and sends the POST request to the */me/sendMail* endpoint and processes the response.</span></span>

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

1. <span data-ttu-id="573b9-171">Abra utils\emailer.js.</span><span class="sxs-lookup"><span data-stu-id="573b9-171">Open utils\emailer.js.</span></span>

1. <span data-ttu-id="573b9-p118">Substitua a função **wrapEmail** pelo seguinte código. Isso cria a carga que representa a mensagem de email a ser enviada.</span><span class="sxs-lookup"><span data-stu-id="573b9-p118">Replace the **wrapEmail** function with the following code. This builds the payload that represents the email message to send.</span></span>

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

## <a name="run-the-app"></a><span data-ttu-id="573b9-174">Executar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="573b9-174">Run the app</span></span>

1. <span data-ttu-id="573b9-175">Em um prompt de comando, execute o seguinte comando no diretório raiz do projeto inicial.</span><span class="sxs-lookup"><span data-stu-id="573b9-175">In a command prompt, run the following command in the root directory of the starter project.</span></span>


        npm start

1. <span data-ttu-id="573b9-176">Em um navegador, navegue até *http://localhost:3000* e escolha o botão **Conectar ao Office 365**.</span><span class="sxs-lookup"><span data-stu-id="573b9-176">In a browser, navigate to *http://localhost:3000* and choose the **Connect to Office 365** button.</span></span>

1. <span data-ttu-id="573b9-177">Entre e conceda as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="573b9-177">Sign in and grant the requested permissions.</span></span> 

1. <span data-ttu-id="573b9-p119">Como alternativa, edite o endereço de email do destinatário e escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão.</span><span class="sxs-lookup"><span data-stu-id="573b9-p119">Optionally edit the recipient's email address, and then choose the **Send mail** button. When the mail is sent, a Success message is displayed below the button.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="573b9-180">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="573b9-180">Next steps</span></span>
- <span data-ttu-id="573b9-181">Experimente a API REST usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="573b9-181">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="573b9-182">Explore nossos outros [exemplos de Node.js](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="573b9-182">Explore our other [Node.js samples](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) on GitHub.</span></span>


## <a name="see-also"></a><span data-ttu-id="573b9-183">Ver também</span><span class="sxs-lookup"><span data-stu-id="573b9-183">See also</span></span>
- [<span data-ttu-id="573b9-184">Protocolos do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="573b9-184">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="573b9-185">Tokens do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="573b9-185">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
