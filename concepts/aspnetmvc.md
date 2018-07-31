# <a name="get-started-with-microsoft-graph-in-an-aspnet-46-mvc-app"></a>Introdução ao Microsoft Graph em um aplicativo do ASP.NET 4.6 MVC

Este artigo descreve as tarefas obrigatórias para obter um token de acesso do ponto de extremidade do Azure AD v2.0 e chamar o Microsoft Graph. Ele o orienta sobre como criar um [Exemplo do Microsoft Graph Connect para ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample) e explica os principais conceitos que você implementa para usar o Microsoft Graph.

A imagem a seguir mostra o aplicativo que você criará. 

![O aplicativo Web com botões "Obter endereço de email" e "Enviar email"](images/aspnet-connect-sample.png "O aplicativo Web com botões 'Obter endereço de email' e 'Enviar email'")

O [Ponto de extremidade do Azure AD v2.0](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-appmodel-v2-overview) permite que os usuários entrem com uma MSA(conta da Microsoft) ou uma conta corporativa ou de estudante. O aplicativo usa o [ASP.Net OpenID Connect OWIN middleware](https://www.nuget.org/packages/Microsoft.Owin.Security.OpenIdConnect/) e a [MSAL (Biblioteca de Autenticação da Microsoft) para .NET](https://www.nuget.org/packages/Microsoft.Identity.Client) para entrada e gerenciamento de tokens.

**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://developer.microsoft.com/pt-BR/graph/quick-start) para agilizar o processo. Observe também que temos uma [Versão REST deste exemplo](https://github.com/microsoftgraph/aspnet-connect-rest-sample).

## <a name="prerequisites"></a>Pré-requisitos

Para começar, será necessário: 

- Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](https://docs.microsoft.com/pt-BR/office/developer-program/office-365-developer-program-faq#account-types)
- Visual Studio 2015 
- O [Exemplo do Microsoft Graph Connect para ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-connect-sample). Você usará a pasta **starter-project** nos exemplos de arquivo.


## <a name="register-the-application"></a>Registrar o aplicativo

Nesta etapa, você registrará um aplicativo no Portal de Registro de Aplicativos da Microsoft. Isso gera a ID do aplicativo e a senha que você usará para configurar o aplicativo no Visual Studio.

1. Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.

2. Escolha **Adicionar um aplicativo**.

3. Insira um nome para o aplicativo e escolha **Criar aplicativo**. 
    
    A página de registro é exibida, listando as propriedades do seu aplicativo.

4. Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo. 

5. Em **Segredos do Aplicativo**, escolha **Gerar Nova Senha**. Copie a senha da caixa de diálogo **Nova senha gerada**.

    Você usará a ID do aplicativo e a senha para configurar o aplicativo. 

6. Em **Plataformas**, escolha **Adicionar plataforma** > **Web**.

7. Não se esqueça de marcar a caixa **Permitir Fluxo Implícito** e insira *http://localhost:55065/* como o URI de redirecionamento. 

    A opção **Permitir Fluxo Implícito** habilita o fluxo híbrido do OpenID Connect. Durante a autenticação, isso permite que o aplicativo receba informações de entrada (o **id_token**) e artefatos (neste caso, um código de autorização) que o aplicativo usa para obter um token de acesso.

8. Escolha **Salvar**.

### <a name="configure-the-project"></a>Configurar o projeto

1. Abra o arquivo de solução para o projeto inicial no Visual Studio.

2. Abra o arquivo Web.config do projeto.

3. Localize as chaves de configuração do aplicativo no elemento **appSettings**. Substitua os valores de espaço reservado ENTER_YOUR_CLIENT_ID e ENTER_YOUR_SECRET pelos valores que você acabou de copiar.

O URI de redirecionamento é a URL do projeto que você registrou. Os [escopos de permissão](https://developer.microsoft.com/pt-BR/graph/docs/concepts/permission_scopes) solicitados permitem que o aplicativo obtenha informações de perfil de usuário e envie um email.

## <a name="call-microsoft-graph"></a>Chamar o Microsoft Graph

Nesta etapa, você se concentrará nas classes **SDKHelper**, **GraphService** e **HomeController**. 

 - O **SDKHelper** inicializa uma instância de **GraphServiceClient** da biblioteca antes de cada chamada ao Microsoft Graph. O token de acesso é adicionado à solicitação nesse momento. 
 - O **GraphService** cria e envia solicitações ao Microsoft Graph usando a biblioteca e processa as respostas.
 - **HomeController** contém ações que iniciam as chamadas à biblioteca em resposta a eventos da interface do usuário.

O projeto inicial já declara uma dependência para o pacote NuGet da Biblioteca de Cliente .NET do Microsoft Graph:  *Microsoft.Graph*.

1. Clique com o botão direito do mouse na pasta **Auxiliares** e escolha **Adicionar** > **Classe**. 

1. Nomeie a nova classe como *SDKHelper* e escolha **Adicionar**.

1. Substitua o conteúdo pelo código a seguir.

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

  Observe a chamada para **SampleAuthProvider** para obter o token quando o cliente é inicializado.

1. Na pasta **Modelos**, abra GraphService.cs. O serviço usa a biblioteca para interagir com o Microsoft Graph.

1. Adicione a instrução **using** a seguir.

        using Microsoft.Graph;

1. Substitua *// GetMyEmailAddress* pelo método a seguir. Isso obtém o endereço de email do usuário atual. 

        // Get the current user's email address from their profile.
        public async Task<string> GetMyEmailAddress(GraphServiceClient graphClient)
        {

            // Get the current user. 
            // The app only needs the user's email address, so select the mail and userPrincipalName properties.
            // If the mail property isn't defined, userPrincipalName should map to the email for all account types. 
            User me = await graphClient.Me.Request().Select("mail,userPrincipalName").GetAsync();
            return me.Mail ?? me.UserPrincipalName;
        }

  Observe o segmento **Select**, que solicita que apenas **mail** e **userPrincipalName** sejam retornados. Você pode usar **Select** e **Filter** para reduzir o tamanho da carga de dados de resposta.

1. Substitua *// SendEmail* pelos métodos a seguir para criar e enviar o email.

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

1. Na pasta **Controllers**, abra HomeController.cs.

1. Adicione a instrução **using** a seguir.

        using Microsoft.Graph;
  
1. Substitua *// Controller actions* pelas ações a seguir.

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

Agora você está pronto para [executar o aplicativo](#run-the-app).

## <a name="run-the-app"></a>Executar o aplicativo
1. Pressione F5 para criar e executar o aplicativo. 

2. Entre com sua conta pessoal, corporativa ou de estudante, e conceda as permissões solicitadas.

3. Escolha o botão **Obter endereço de email**. Quando a operação for concluída, o endereço de email do usuário conectado será exibido na página.

4. Como alternativa, edite a lista de destinatários e o assunto do email e, em seguida, escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão.


## <a name="next-steps"></a>Próximas etapas
- Experimente a API REST usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Obtenha exemplos de operações comuns em [Exemplo de trechos do Microsoft Graph para ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-snippets-sample) ou explore nossos outros [Exemplos do ASP.NET](http://aka.ms/aspnetgraphsamples) no GitHub.

## <a name="see-also"></a>Confira também
- [Biblioteca de cliente do .NET do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [Cenário de autenticação de aplicativo Web para API Web](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-authentication-scenarios/#web-application-to-web-api)
- [Integrar a Identidade da Microsoft e o Microsoft Graph em um aplicativo Web usando OpenID Connect](https://azure.microsoft.com/pt-BR/documentation/samples/active-directory-dotnet-webapp-openidconnect-v2/)
- [Protocolos do Azure AD v2.0](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-protocols/)
- [Tokens do Azure AD v2.0](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-tokens/)
