# <a name="get-started-with-microsoft-graph-in-an-aspnet-46-mvc-app"></a><span data-ttu-id="9eb43-101">Introdução ao Microsoft Graph em um aplicativo do ASP.NET 4.6 MVC</span><span class="sxs-lookup"><span data-stu-id="9eb43-101">Get started with Microsoft Graph in an ASP.NET 4.6 MVC app</span></span>

<span data-ttu-id="9eb43-p101">Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph. Ele o orienta sobre como criar um [Exemplo do Microsoft Graph Connect para ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample) e explica os principais conceitos que você implementa para usar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p101">This article describes the tasks required to get an access token from the Azure AD v2.0 endpoint and call Microsoft Graph. It walks you through building the [Microsoft Graph Connect Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample) and explains the main concepts that you implement to use Microsoft Graph.</span></span>

<span data-ttu-id="9eb43-104">A imagem a seguir mostra o aplicativo que você criará.</span><span class="sxs-lookup"><span data-stu-id="9eb43-104">The following image shows the app you'll create.</span></span> 

<span data-ttu-id="9eb43-105">![O aplicativo Web com botões "Obter endereço de email" e "Enviar email"](images/aspnet-connect-sample.png "O aplicativo Web com botões 'Obter endereço de email' e 'Enviar email'")</span><span class="sxs-lookup"><span data-stu-id="9eb43-105">![The web app with "Get email address" and "Send email" buttons](images/aspnet-connect-sample.png "The web app with 'Get email address' and 'Send email' buttons")</span></span>

<span data-ttu-id="9eb43-p102">O [Ponto de extremidade do Azure AD v2.0](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-appmodel-v2-overview) permite que os usuários entrem com uma MSA(conta da Microsoft) ou uma conta corporativa ou de estudante. O aplicativo usa o [ASP.Net OpenID Connect OWIN middleware](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) e a [MSAL (Biblioteca de Autenticação da Microsoft) para .NET](https://www.nuget.org/packages/Microsoft.Identity.Client) para entrada e gerenciamento de tokens.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p102">The [Azure AD v2.0 endpoint](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-appmodel-v2-overview) lets users sign in with a Microsoft account (MSA) or a work or school account. The app uses the [ASP.Net OpenID Connect OWIN middleware](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) and the [Microsoft Authentication Library (MSAL) for .NET](https://www.nuget.org/packages/Microsoft.Identity.Client) for sign in and token management.</span></span>

<span data-ttu-id="9eb43-p103">**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://developer.microsoft.com/pt-BR/graph/quick-start) para começar a usar rapidamente. Observe também que temos uma [Versão REST deste exemplo](https://github.com/microsoftgraph/aspnet-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="9eb43-p103">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/pt-BR/graph/quick-start) to get up and running fast. Also note that we have a [REST version of this sample](https://github.com/microsoftgraph/aspnet-connect-rest-sample).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9eb43-111">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9eb43-111">Prerequisites</span></span>

<span data-ttu-id="9eb43-112">Para começar, será necessário:</span><span class="sxs-lookup"><span data-stu-id="9eb43-112">To get started, you'll need:</span></span> 

- <span data-ttu-id="9eb43-113">Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="9eb43-113">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
- <span data-ttu-id="9eb43-114">Visual Studio 2015</span><span class="sxs-lookup"><span data-stu-id="9eb43-114">Visual Studio 2015</span></span> 
- <span data-ttu-id="9eb43-p104">O [Exemplo do Microsoft Graph Connect para ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample). Você usará a pasta **starter-project** nos exemplos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p104">The [Microsoft Graph Connect Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample). You'll use the **starter-project** folder in the sample files.</span></span>


## <a name="register-the-application"></a><span data-ttu-id="9eb43-117">Registrar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="9eb43-117">Register the application</span></span>

<span data-ttu-id="9eb43-p105">Nesta etapa, você registrará um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e a senha que você usará para configurar o aplicativo no Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p105">In this step, you'll register an app on the Microsoft App Registration Portal. This generates the app ID and password that you'll use to configure the app in Visual Studio.</span></span>

1. <span data-ttu-id="9eb43-120">Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="9eb43-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>

2. <span data-ttu-id="9eb43-121">Escolha **Adicionar um aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="9eb43-121">Choose **Add an app**.</span></span>

3. <span data-ttu-id="9eb43-122">Insira um nome para o aplicativo e escolha **Criar aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="9eb43-122">Enter a name for the app, and choose **Create application**.</span></span> 
    
    <span data-ttu-id="9eb43-123">A página de registro é exibida, listando as propriedades do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9eb43-123">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="9eb43-p106">Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p106">Copy the application ID. This is the unique identifier for your app.</span></span> 

5. <span data-ttu-id="9eb43-p107">Em **Segredos do Aplicativo**, escolha **Gerar Nova Senha**. Copie a senha da caixa de diálogo **Nova senha gerada**.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p107">Under **Application Secrets**, choose **Generate New Password**. Copy the password from the **New password generated** dialog.</span></span>

    <span data-ttu-id="9eb43-128">Você usará a ID do aplicativo e a senha para configurar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9eb43-128">You'll use the application ID and password to configure the app.</span></span> 

6. <span data-ttu-id="9eb43-129">Em **Plataformas**, escolha **Adicionar plataforma** > **Web**.</span><span class="sxs-lookup"><span data-stu-id="9eb43-129">Under **Platforms**, choose **Add platform** > **Web**.</span></span>

7. <span data-ttu-id="9eb43-130">Não deixe de marcar a caixa de diálogo **Permitir Fluxo Implícito** e insira *http://localhost:55065/* como o URI de Redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="9eb43-130">Make sure the **Allow Implicit Flow** check box is selected, and enter *http://localhost:55065/* as the Redirect URI.</span></span> 

    <span data-ttu-id="9eb43-p108">A opção **Permitir Fluxo Implícito** habilita o fluxo híbrido do OpenID Connect. Durante a autenticação, isso permite que o aplicativo receba informações de entrada (o **id_token**) e artefatos (neste caso, um código de autorização) que o aplicativo usa para obter um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p108">The **Allow Implicit Flow** option enables the OpenID Connect hybrid flow. During authentication, this enables the app to receive both sign-in info (the **id_token**) and artifacts (in this case, an authorization code) that the app uses to obtain an access token.</span></span>

8. <span data-ttu-id="9eb43-133">Escolha **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="9eb43-133">Choose **Save**.</span></span>

### <a name="configure-the-project"></a><span data-ttu-id="9eb43-134">Configurar o projeto</span><span class="sxs-lookup"><span data-stu-id="9eb43-134">Configure the project</span></span>

1. <span data-ttu-id="9eb43-135">Abra o arquivo de solução para o projeto inicial no Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="9eb43-135">Open the solution file for the starter project in Visual Studio.</span></span>

2. <span data-ttu-id="9eb43-136">Abra o arquivo Web.config do projeto.</span><span class="sxs-lookup"><span data-stu-id="9eb43-136">Open the project's Web.config file.</span></span>

3. <span data-ttu-id="9eb43-p109">Localize as chaves de configuração do aplicativo no elemento **appSettings**. Substitua os valores de espaço reservado ENTER_YOUR_CLIENT_ID e ENTER_YOUR_SECRET pelos valores que você acabou de copiar.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p109">Locate the app configuration keys in the **appSettings** element. Replace the ENTER_YOUR_CLIENT_ID and ENTER_YOUR_SECRET placeholder values with the values you just copied.</span></span>

<span data-ttu-id="9eb43-p110">O URI de redirecionamento é a URL do projeto que você registrou. Os [escopos de permissão](https://developer.microsoft.com/pt-BR/graph/docs/concepts/permission_scopes) solicitados permitem que o aplicativo obtenha informações de perfil de usuário e envie um email.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p110">The redirect URI is the URL of the project that you registered. The requested [permission scopes](https://developer.microsoft.com/pt-BR/graph/docs/concepts/permission_scopes) allow the app to get user profile information and send an email.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="9eb43-141">Chamar o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9eb43-141">Call Microsoft Graph</span></span>

<span data-ttu-id="9eb43-142">Nesta etapa, você se concentrará nas classes **SDKHelper**, **GraphService** e **HomeController**.</span><span class="sxs-lookup"><span data-stu-id="9eb43-142">In this step, you'll focus on the **SDKHelper**, **GraphService**, and **HomeController** classes.</span></span> 

 - <span data-ttu-id="9eb43-p111">O **SDKHelper** inicializa uma instância de **GraphServiceClient** da biblioteca antes de cada chamada ao Microsoft Graph. O token de acesso é adicionado à solicitação nesse momento.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p111">**SDKHelper** intializes an instance of the **GraphServiceClient** from the library before each call to the Microsoft Graph. This is when the access token is added to the request.</span></span> 
 - <span data-ttu-id="9eb43-145">**GraphService** cria e envia solicitações ao Microsoft Graph usando a biblioteca e processa as respostas.</span><span class="sxs-lookup"><span data-stu-id="9eb43-145">**GraphService** builds and sends requests to the Microsoft Graph using the library, and processes the responses.</span></span>
 - <span data-ttu-id="9eb43-146">**HomeController** contém ações que iniciam as chamadas à biblioteca em resposta a eventos da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="9eb43-146">**HomeController** contains actions that initiate the calls to the library in response to UI events.</span></span>

<span data-ttu-id="9eb43-147">O projeto inicial já declara uma dependência para o pacote NuGet da Biblioteca de Cliente .NET do Microsoft Graph:  *Microsoft.Graph*.</span><span class="sxs-lookup"><span data-stu-id="9eb43-147">The starter project already declares a dependency for the Microsoft Graph .NET Client Library NuGet package:  *Microsoft.Graph*.</span></span>

1. <span data-ttu-id="9eb43-148">Clique com o botão direito do mouse na pasta **Auxiliares** e escolha **Adicionar** > **Classe**.</span><span class="sxs-lookup"><span data-stu-id="9eb43-148">Right-click the **Helpers** folder and choose **Add** > **Class**.</span></span> 

1. <span data-ttu-id="9eb43-149">Nomeie a nova classe como *SDKHelper* e escolha **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="9eb43-149">Name the new class *SDKHelper* and choose **Add**.</span></span>

1. <span data-ttu-id="9eb43-150">Substitua o conteúdo pelo código a seguir.</span><span class="sxs-lookup"><span data-stu-id="9eb43-150">Replace the contents with the following code.</span></span>

        using System.Net.Http.Headers;
        using Microsoft.Graph;

        namespace Microsoft_Graph_SDK_ASPNET_Connect.Helpers
        {
            public class SDKHelper
            {   
                private static GraphServiceClient graphClient = null;

                // Get an authenticated Microsoft Graph Service client.
                public static GraphServiceClient GetAuthenticatedClient()
                {
                    GraphServiceClient graphClient = new GraphServiceClient(
                        new DelegateAuthenticationProvider(
                            async (requestMessage) =>
                            {
                                string accessToken = await SampleAuthProvider.Instance.GetUserAccessTokenAsync();

                                // Append the access token to the request.
                                requestMessage.Headers.Authorization = new AuthenticationHeaderValue("bearer", accessToken);
                            }));
                    return graphClient;
                }

                public static void SignOutClient()
                {
                    graphClient = null;
                }
            }
        }

  <span data-ttu-id="9eb43-151">Observe a chamada para **SampleAuthProvider** para obter o token quando o cliente é inicializado.</span><span class="sxs-lookup"><span data-stu-id="9eb43-151">Note the call to **SampleAuthProvider** to get the token when the client is initialized.</span></span>

1. <span data-ttu-id="9eb43-p112">Na pasta **Modelos**, abra GraphService.cs. O serviço usa a biblioteca para interagir com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p112">In the **Models** folder, open GraphService.cs. The service uses the library to interact with the Microsoft Graph.</span></span>

1. <span data-ttu-id="9eb43-154">Adicione a instrução **using** a seguir.</span><span class="sxs-lookup"><span data-stu-id="9eb43-154">Add the following **using** statement.</span></span>

        using Microsoft.Graph;

1. <span data-ttu-id="9eb43-p113">Substitua *// GetMyEmailAddress* pelo método a seguir. Isso obtém o endereço de email do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p113">Replace *// GetMyEmailAddress* with the following method. This gets the current user's email address.</span></span> 

        // Get the current user's email address from their profile.
        public async Task<string> GetMyEmailAddress(GraphServiceClient graphClient)
        {

            // Get the current user. 
            // The app only needs the user's email address, so select the mail and userPrincipalName properties.
            // If the mail property isn't defined, userPrincipalName should map to the email for all account types. 
            User me = await graphClient.Me.Request().Select("mail,userPrincipalName").GetAsync();
            return me.Mail ?? me.UserPrincipalName;
        }

  <span data-ttu-id="9eb43-p114">Observe o segmento **Select**, que solicita que apenas **mail** e **userPrincipalName** sejam retornados. Você pode usar **Select** e **Filter** para reduzir o tamanho da carga de dados de resposta.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p114">Note the **Select** segment, which requests only the **mail** and **userPrinicipalName** to be returned. You can use **Select** and **Filter** to reduce the size of the response data payload.</span></span>

1. <span data-ttu-id="9eb43-159">Substitua *// SendEmail* pelos métodos a seguir para criar e enviar o email.</span><span class="sxs-lookup"><span data-stu-id="9eb43-159">Replace *// SendEmail* with the following methods to build and send the email.</span></span>

        // Send an email message from the current user.
        public async Task SendEmail(GraphServiceClient graphClient, Message message)
        {
            await graphClient.Me.SendMail(message, true).Request().PostAsync();
        }

        public async Task<Message> BuildEmailMessage(GraphServiceClient graphClient, string recipients, string subject)
        {

            // Get current user photo
            Stream photoStream = await GetCurrentUserPhotoStreamAsync(graphClient);


            // If the user doesn't have a photo, or if the user account is MSA, we use a default photo

            if ( photoStream == null)
            {
                photoStream = System.IO.File.OpenRead(System.Web.Hosting.HostingEnvironment.MapPath("/Content/test.jpg"));
            }

            MemoryStream photoStreamMS = new MemoryStream();
            // Copy stream to MemoryStream object so that it can be converted to byte array.
            photoStream.CopyTo(photoStreamMS);

            DriveItem photoFile = await UploadFileToOneDrive(graphClient, photoStreamMS.ToArray());

            MessageAttachmentsCollectionPage attachments = new MessageAttachmentsCollectionPage();
            attachments.Add(new FileAttachment
            {
                ODataType = "#microsoft.graph.fileAttachment",
                ContentBytes = photoStreamMS.ToArray(),
                ContentType = "image/png",
                Name = "me.png"
            });

            Permission sharingLink = await GetSharingLinkAsync(graphClient, photoFile.Id);

            // Add the sharing link to the email body.
            string bodyContent = string.Format(Resource.Graph_SendMail_Body_Content, sharingLink.Link.WebUrl);

            // Prepare the recipient list.
            string[] splitter = { ";" };
            string[] splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();
            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient
                {
                    EmailAddress = new EmailAddress
                    {
                        Address = recipient.Trim()
                    }
                });
            }

            // Build the email message.
            Message email = new Message
            {
                Body = new ItemBody
                {
                    Content = bodyContent,
                    ContentType = BodyType.Html,
                },
                Subject = subject,
                ToRecipients = recipientList,
                Attachments = attachments
            };
            return email;
        }

        // Gets the stream content of the signed-in user's photo. 
        // This snippet doesn't work with consumer accounts.
        public async Task<Stream> GetCurrentUserPhotoStreamAsync(GraphServiceClient graphClient)
        {
            Stream currentUserPhotoStream = null;

            try
            {
                currentUserPhotoStream = await graphClient.Me.Photo.Content.Request().GetAsync();

            }

            // If the user account is MSA (not work or school), the service will throw an exception.
            catch (ServiceException)
            {
                return null;
            }

            return currentUserPhotoStream;

        }

        // Uploads the specified file to the user's root OneDrive directory.
        public async Task<DriveItem> UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
        {
            DriveItem uploadedFile = null;

            try
            {
                MemoryStream fileStream = new MemoryStream(file);
                uploadedFile = await graphClient.Me.Drive.Root.ItemWithPath("me.png").Content.Request().PutAsync<DriveItem>(fileStream);

            }


            catch (ServiceException)
            {
                return null;
            }

            return uploadedFile;
        }

        public static async Task<Permission> GetSharingLinkAsync(GraphServiceClient graphClient, string Id)
        {
            Permission permission = null;

            try
            {
                permission = await graphClient.Me.Drive.Items[Id].CreateLink("view").Request().PostAsync();
            }

            catch (ServiceException)
            {
                return null;
            }

            return permission;
        }

1. <span data-ttu-id="9eb43-160">Na pasta **Controllers**, abra HomeController.cs.</span><span class="sxs-lookup"><span data-stu-id="9eb43-160">In the **Controllers** folder, open HomeController.cs.</span></span>

1. <span data-ttu-id="9eb43-161">Adicione a instrução **using** a seguir.</span><span class="sxs-lookup"><span data-stu-id="9eb43-161">Add the following **using** statement.</span></span>

        using Microsoft.Graph;
  
1. <span data-ttu-id="9eb43-162">Substitua *// Controller actions* pelas ações a seguir.</span><span class="sxs-lookup"><span data-stu-id="9eb43-162">Replace *// Controller actions* with the following actions.</span></span>

        [Authorize]
        // Get the current user's email address from their profile.
        public async Task<ActionResult> GetMyEmailAddress()
        {
            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Get the current user's email address. 
                ViewBag.Email = await graphService.GetMyEmailAddress(graphClient);
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Message == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
            }
        }

        [Authorize]
        // Send mail on behalf of the current user.
        public async Task<ActionResult> SendEmail()
        {
            if (string.IsNullOrEmpty(Request.Form["email-address"]))
            {
                ViewBag.Message = Resource.Graph_SendMail_Message_GetEmailFirst;
                return View("Graph");
            }

            try
            {

                // Initialize the GraphServiceClient.
                GraphServiceClient graphClient = SDKHelper.GetAuthenticatedClient();

                // Build the email message.
                Message message = await graphService.BuildEmailMessage(graphClient, Request.Form["recipients"], Request.Form["subject"]);

                // Send the email.
                await graphService.SendEmail(graphClient, message);

                // Reset the current user's email address and the status to display when the page reloads.
                ViewBag.Email = Request.Form["email-address"];
                ViewBag.Message = Resource.Graph_SendMail_Success_Result;
                return View("Graph");
            }
            catch (ServiceException se)
            {
                if (se.Error.Code == Resource.Error_AuthChallengeNeeded) return new EmptyResult();
                return RedirectToAction("Index", "Error", new { message = Resource.Error_Message + Request.RawUrl + ": " + se.Error.Message });
            }
        }

<span data-ttu-id="9eb43-163">Agora você está pronto para [executar o aplicativo](#run-the-app).</span><span class="sxs-lookup"><span data-stu-id="9eb43-163">Now you're ready to [run the app](#run-the-app).</span></span>

## <a name="run-the-app"></a><span data-ttu-id="9eb43-164">Executar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="9eb43-164">Run the app</span></span>
1. <span data-ttu-id="9eb43-165">Pressione F5 para criar e executar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9eb43-165">Press F5 to build and run the app.</span></span> 

2. <span data-ttu-id="9eb43-166">Entre com sua conta pessoal, comercial ou de estudante e conceda as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="9eb43-166">Sign in with your personal or work or school account and grant the requested permissions.</span></span>

3. <span data-ttu-id="9eb43-p115">Escolha o botão **Obter endereço de email**. Quando a operação for concluída, o endereço de email do usuário conectado será exibido na página.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p115">Choose the **Get email address** button. When the operation completes, the email address of the signed-in user is displayed on the page.</span></span>

4. <span data-ttu-id="9eb43-p116">Como alternativa, edite a lista de destinatários e o assunto do email e, em seguida, escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão.</span><span class="sxs-lookup"><span data-stu-id="9eb43-p116">Optionally edit the recipient list and email subject, and then choose the **Send email** button. When the mail is sent, a Success message is displayed below the button.</span></span>


## <a name="next-steps"></a><span data-ttu-id="9eb43-171">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9eb43-171">Next steps</span></span>
- <span data-ttu-id="9eb43-172">Experimente a API REST usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="9eb43-172">Try out the REST API using the [Graph explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="9eb43-173">Obtenha exemplos de operações comuns em [Exemplo de trechos do Microsoft Graph para ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-snippets-sample) ou explore nossos outros [Exemplos do ASP.NET](http://aka.ms/aspnetgraphsamples) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="9eb43-173">Find examples of common operations in the [Microsoft Graph Snippets Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-snippets-sample), or explore our other [ASP.NET samples](http://aka.ms/aspnetgraphsamples) on GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="9eb43-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="9eb43-174">See also</span></span>
- [<span data-ttu-id="9eb43-175">Biblioteca de cliente do .NET do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9eb43-175">Microsoft Graph .NET Client Library</span></span>](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [<span data-ttu-id="9eb43-176">Cenário de autenticação de aplicativo Web para API Web</span><span class="sxs-lookup"><span data-stu-id="9eb43-176">Web application to web API authentication scenario</span></span>](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api)
- [<span data-ttu-id="9eb43-177">Integrar a Identidade da Microsoft e o Microsoft Graph em um aplicativo Web usando OpenID Connect</span><span class="sxs-lookup"><span data-stu-id="9eb43-177">Integrate Microsoft identity and the Microsoft Graph into a web application using OpenID Connect</span></span>](https://azure.microsoft.com/pt-BR/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/)
- [<span data-ttu-id="9eb43-178">Protocolos do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="9eb43-178">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="9eb43-179">Tokens do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="9eb43-179">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-tokens/)
