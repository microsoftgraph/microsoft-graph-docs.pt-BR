# <a name="get-started-with-microsoft-graph-in-an-objectve-c-ios-app"></a><span data-ttu-id="f8e10-101">Introdução ao Microsoft Graph em um aplicativo Objective C iOS</span><span class="sxs-lookup"><span data-stu-id="f8e10-101">Get started with Microsoft Graph in an Objectve C iOS App</span></span>

> <span data-ttu-id="f8e10-p101">**Criando aplicativos para clientes corporativos?** O aplicativo pode não funcionar caso o cliente corporativo habilite os recursos Enterprise Mobility + Security, como <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">acesso condicional ao dispositivo</a>. Nesse caso, pode ser que você não esteja ciente e seu cliente pode enfrentar problemas de erro.</span><span class="sxs-lookup"><span data-stu-id="f8e10-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="f8e10-p102">Para dar suporte a **todos os clientes corporativos**, em **todos os cenários corporativos**, use o ponto de extremidade do Microsoft Azure AD e gerencie seus aplicativos usando o [Portal do Azure](https://aka.ms/aadapplist). Para saber mais, confira o tópico [Decidindo entre os pontos de extremidade do Microsoft Azure AD e do Microsoft Azure AD versão 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="f8e10-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure Management Portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="f8e10-p103">Este artigo descreve as tarefas obrigatórias para obter um token de acesso do [ponto de extremidade do Azure AD v2.0](https://developer.microsoft.com/pt-BR/graph/docs/concepts/converged_auth) e chamar o Microsoft Graph. Ele orienta você em relação ao código dentro do [Exemplo de conexão com o Office 365 para iOS (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) para explicar os principais conceitos que você tem que implementar em um aplicativo que usa o Microsoft Graph. Ele descreve como acessar o Microsoft Graph usando [SDK do Microsoft Graph para iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span><span class="sxs-lookup"><span data-stu-id="f8e10-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/pt-BR/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) to explain the main concepts that you have to implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using the [Microsoft Graph SDK for iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).</span></span>

<span data-ttu-id="f8e10-110">Você pode baixar a versão do aplicativo que você criará a partir deste repositório do GitHub:</span><span class="sxs-lookup"><span data-stu-id="f8e10-110">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="f8e10-111">Exemplo de conexão com o Office 365 para iOS usando o SDK do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f8e10-111">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

<span data-ttu-id="f8e10-112">A imagem a seguir mostra o aplicativo que você criará.</span><span class="sxs-lookup"><span data-stu-id="f8e10-112">The following image shows the app you'll create.</span></span>

![O passo a passo do exemplo de conexão mostra como conectar e enviar um email no aplicativo](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="f8e10-114">O fluxo de trabalho será conectar/autenticar ao Microsoft Graph, entrar com sua conta pessoal ou corporativa e finalmente enviar um email para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="f8e10-114">The workflow will be to connect/authenticate to Microsoft Graph, sign in with your work or personal account, and finally send a mail to a recipient.</span></span>

<span data-ttu-id="f8e10-p104">**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://graph.microsoft.io/pt-BR/getting-started) para começar a usar rapidamente.</span><span class="sxs-lookup"><span data-stu-id="f8e10-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://graph.microsoft.io/pt-BR/getting-started) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8e10-117">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8e10-117">Prerequisites</span></span>

<span data-ttu-id="f8e10-118">Para começar, será necessário:</span><span class="sxs-lookup"><span data-stu-id="f8e10-118">To get started, you'll need:</span></span> 

* <span data-ttu-id="f8e10-119">[Xcode](https://developer.apple.com/xcode/downloads/) da Apple</span><span class="sxs-lookup"><span data-stu-id="f8e10-119">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="f8e10-120">Instalação do [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) como um gerente de dependências</span><span class="sxs-lookup"><span data-stu-id="f8e10-120">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="f8e10-121">Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](http://dev.office.com/devprogram)</span><span class="sxs-lookup"><span data-stu-id="f8e10-121">A [Microsoft account](https://www.outlook.com/) or a [work or school account](http://dev.office.com/devprogram)</span></span>
* <span data-ttu-id="f8e10-122">O [Projeto inicial do Microsoft Graph para iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="f8e10-122">The [Microsoft Graph Starter Project for iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> <span data-ttu-id="f8e10-123">Este modelo contém classes às quais você adicionará código.</span><span class="sxs-lookup"><span data-stu-id="f8e10-123">This template contains classes that you'll add code to.</span></span> <span data-ttu-id="f8e10-124">Para obter este projeto, clone ou baixe o exemplo de projeto deste local, e você trabalhará com o espaço de trabalho dentro da pasta **starter-project** (**ios-objectivec-connect-sample.xcworkspace**).</span><span class="sxs-lookup"><span data-stu-id="f8e10-124">To get this project, clone or download the sample project from this location, and you'll work with the workspace inside the **starter-project** folder (**ios-objectivec-connect-sample.xcworkspace**).</span></span>

## <a name="register-the-app"></a><span data-ttu-id="f8e10-125">Registrar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8e10-125">Register the app</span></span>
 
1. <span data-ttu-id="f8e10-126">Entre no [Portal de Registro do Aplicativo](https://apps.dev.microsoft.com/) usando sua conta pessoal ou sua conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="f8e10-126">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="f8e10-127">Selecione **Adicionar um aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="f8e10-127">Select **Add an app**.</span></span>
3. <span data-ttu-id="f8e10-128">Insira um nome para o aplicativo e selecione **Criar aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="f8e10-128">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="f8e10-129">A página de registro é exibida, listando as propriedades do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8e10-129">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="f8e10-130">Em **Plataformas**, selecione **Adicionar plataforma**.</span><span class="sxs-lookup"><span data-stu-id="f8e10-130">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="f8e10-131">Selecione **Plataforma nativa**.</span><span class="sxs-lookup"><span data-stu-id="f8e10-131">Select **Native platform**.</span></span>
6. <span data-ttu-id="f8e10-p106">Copie a ID de Cliente para a área de transferência. Você precisará inserir esse valor no exemplo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8e10-p106">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="f8e10-134">Essa ID de aplicativo é o identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8e10-134">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="f8e10-135">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="f8e10-135">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="f8e10-136">Importando as dependências do projeto</span><span class="sxs-lookup"><span data-stu-id="f8e10-136">Importing the project dependencies</span></span>

1. <span data-ttu-id="f8e10-137">Clonar este repositório, [Exemplo de conexão com o Office 365 para iOS usando o SDK do Microsoft Graph](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span><span class="sxs-lookup"><span data-stu-id="f8e10-137">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-objectivec-connect-sample).</span></span> 
><span data-ttu-id="f8e10-138">IMPORTANTE: Use o exemplo na pasta starter-project, não o exemplo na raiz do projeto.</span><span class="sxs-lookup"><span data-stu-id="f8e10-138">IMPORTANT: Use the sample in the starter-project folder and not the sample at the root of the project.</span></span>

2. <span data-ttu-id="f8e10-p107">Use o CocoaPods para importar as dependências de autenticação e o SDK do Microsoft Graph. Este aplicativo de exemplo já contém um podfile que colocará os pods no projeto. Navegue até a pasta **starter-project** no aplicativo **Terminal** e, do **Terminal**, execute:</span><span class="sxs-lookup"><span data-stu-id="f8e10-p107">Use CocoaPods to import the Microsoft Graph SDK and authentication dependencies. This sample app already contains a podfile that will get the pods into the project. Navigate to the folder **starter-project** in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="f8e10-p108">Você receberá a confirmação de que os pods foram importados para o projeto. Para saber mais, confira [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html).</span><span class="sxs-lookup"><span data-stu-id="f8e10-p108">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="f8e10-144">Habilitar o compartilhamento de chaves</span><span class="sxs-lookup"><span data-stu-id="f8e10-144">Enable keychain sharing</span></span>
 
<span data-ttu-id="f8e10-p109">Para o Xcode8, você deve adicionar o grupo de chaves para que o aplicativo não falhe ao acessar a chave. Para adicionar o grupo de chaves:</span><span class="sxs-lookup"><span data-stu-id="f8e10-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="f8e10-p110">Escolha o projeto, no painel do gerente de projetos do Xcode. (⌘ + 1).</span><span class="sxs-lookup"><span data-stu-id="f8e10-p110">Select the project on the project manager panel in Xcode. (⌘ + 1).</span></span>
 
2. <span data-ttu-id="f8e10-149">Selecione **iOS-ObjectiveC-Connect-Sample**.</span><span class="sxs-lookup"><span data-stu-id="f8e10-149">Select **iOS-ObjectiveC-Connect-Sample**.</span></span>
 
3. <span data-ttu-id="f8e10-150">Na guia Recursos, habilite o **Compartilhamento de chaves**.</span><span class="sxs-lookup"><span data-stu-id="f8e10-150">On the Capabilities tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="f8e10-151">Adicione **com.microsoft.ios-objectivec-connect-sample** aos Grupos de Chaves.</span><span class="sxs-lookup"><span data-stu-id="f8e10-151">Add **com.microsoft.ios-objectivec-connect-sample** to the Keychain Groups.</span></span>
 

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="f8e10-152">Autenticando com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f8e10-152">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="f8e10-p111">Para rever o fluxo de trabalho de interface do usuário, o aplicativo fará o usuário autenticar e, em seguida, ele terá a capacidade de enviar um email para um usuário especificado. Para realizar solicitações ao serviço do Microsoft Graph, um provedor de autenticação deverá ser fornecido para autenticar solicitações HTTPS com um token de portador OAuth 2.0 apropriado. No exemplo de projeto, há uma classe de autenticação já oculta chamada **AuthenticationProvider.m.** Vamos adicionar uma função para solicitar e adquirir um token de acesso para chamar a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f8e10-p111">To revisit the UI workflow, the app is going to have the user authenticate, and then they'll have the ability to send a mail to a specified user. To make requests against the Microsoft Graph service, an authentication provider must be supplied which is capable of authenticating HTTPS requests with an appropriate OAuth 2.0 bearer token. In the sample project there's an authentication class already stubbed out called **AuthenticationProvider.m.** We will add a function to request, and acquire, an access token for calling the Microsoft Graph API.</span></span> 

1. <span data-ttu-id="f8e10-157">Abra o espaço de trabalho do projeto Xcode (**iOS-ObjectiveC-Connect-Sample.xcworkspace**) na pasta **starter-project**, navegue até a pasta **Authentication** e abra o arquivo **AuthenticationProvider.m.**</span><span class="sxs-lookup"><span data-stu-id="f8e10-157">Open the Xcode project workspace (**iOS-ObjectiveC-Connect-Sample.xcworkspace**) in the **starter-project** folder, and navigate to the **Authentication** folder and open the file **AuthenticationProvider.m.**</span></span> <span data-ttu-id="f8e10-158">Adicione o código a seguir a essa classe.</span><span class="sxs-lookup"><span data-stu-id="f8e10-158">Add the following code to that class.</span></span>

```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId scopes:(NSArray *)scopes completion:(void (^)    (NSError *))completion{
      [NXOAuth2AuthenticationProvider setClientId:kClientId scopes:scopes];
      /**
      Obtains access token by performing login with UI, where viewController specifies the parent view controller.
      @param viewController The view controller to present the UI on.
      @param completionHandler The completion handler to be called when the authentication has completed.
      error should be non nil if there was no error, and should contain any error(s) that occurred.
      */

      if ([[NXOAuth2AuthenticationProvider sharedAuthProvider] loginSilent]) {
         completion(nil);
      }
      else {
         [[NXOAuth2AuthenticationProvider sharedAuthProvider] loginWithViewController:nil completion:^(NSError *error) {
            if (!error) {
               NSLog(@"Authentication successful.");
               completion(nil);
            }
            else {
               NSLog(@"Authentication failed - %@", error.localizedDescription);
               completion(error);
            }
         }];
      }
   }
```     

2. <span data-ttu-id="f8e10-p113">Em seguida, adicione o método ao arquivo de cabeçalho. Abra o arquivo **AuthenticationProvider.h** e adicione o código a seguir a esta classe.</span><span class="sxs-lookup"><span data-stu-id="f8e10-p113">Next add the method to the header file. Open the file **AuthenticationProvider.h** and add the following code to this class.</span></span>
   ```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId
                               scopes:(NSArray *)scopes
                           completion:(void (^)(NSError *error))completion;
   ```

2. <span data-ttu-id="f8e10-p114">Finalmente chamaremos esse método de **ConnectViewController.m**. Este controlador é a visualização padrão que o aplicativo carrega, e há um único botão chamado **Conectar** que o usuário toca que iniciará o processo de autenticação. Este método usa dois parâmetros, a **ID do cliente** e os **escopos**, que discutiremos de maneira mais detalhada abaixo. Adicione a ação a seguir a **ConnectViewController.m**.</span><span class="sxs-lookup"><span data-stu-id="f8e10-p114">Finally we'll call this method from **ConnectViewController.m**. This controller is the default view that the app loads, and there is a single button named **Connect** that the user will tap that will initiate the authentication process. This method takes in two parameters, the **Client ID** and **scopes**, we'll discuss these in more detail below. Add the following action to **ConnectViewController.m**.</span></span>

```objectivec
- (IBAction)connectTapped:(id)sender {
   [self showLoadingUI:YES];
   NSArray *scopes = [kScopes componentsSeparatedByString:@","];
   [self.authProvider connectToGraphWithClientId:kClientId scopes:scopes completion:^(NSError *error) {
   if (!error) {
      [self performSegueWithIdentifier:@"showSendMail" sender:nil];
      [self showLoadingUI:NO];
      NSLog(@"Authentication successful.");
   }
   else{
      NSLog(NSLocalizedString(@"CHECK_LOG_ERROR", error.localizedDescription));
      [self showLoadingUI:NO];
   };
  }];
}
```     

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="f8e10-165">Enviar um email com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f8e10-165">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="f8e10-p115">Depois de configurar o projeto para ser capaz de autenticar, as próximas tarefas são enviar um email para um usuário usando a API do Microsoft Graph. Por padrão, o usuário conectado será o destinatário, mas você tem a capacidade de alterá-lo para qualquer outro destinatário. O código com o qual trabalharemos aqui está localizado na pasta **Controllers** e na classe **SendMailViewController.m.** Você verá que há outro código representado aqui para a interface do usuário e um método auxiliar para recuperar informações de perfil de usuário do serviço do Microsoft Graph. Vamos nos concentrar nos métodos para criar uma mensagem de email e enviar essa mensagem.</span><span class="sxs-lookup"><span data-stu-id="f8e10-p115">After configuring the project to be able to authenticate, the next tasks are sending a mail to a user using the Microsoft Graph API. By default the logged in user will be the recipient, but you have the ability to change it to any other recipient. The code we'll work with here is located in the **Controllers** folder and in the class **SendMailViewController.m.** You'll see that there is other code represented here for the UI, and a helper method to retrieve user profile information from the Microsoft Graph service. We'll concentrate on the methods for creating a mail message and sending that message.</span></span>

1. <span data-ttu-id="f8e10-171">Abra **SendMailViewController.m** na pasta controladores e adicione o código a seguir para o método **viewDidLoad**, após `self.graphClient = [MSGraphClient client]`</span><span class="sxs-lookup"><span data-stu-id="f8e10-171">Open **SendMailViewController.m** in the Controllers folder and add the following code to the **viewDidLoad** method, after `self.graphClient = [MSGraphClient client]`</span></span>
   ```objectivec
       [self getUserInfo:(self.emailAddress) completion:^( NSError *error) {
        if (!error) {
            [self getUserPicture:(self.emailAddress)  completion:^(UIImage *image, NSError *error) {
                if (!error) {
                    self.userPicture = image;
                } else {
                    //get the test image out of the project resources
                    self.userPicture = [UIImage imageNamed:(@"test.png")];
                }
                [self uploadPictureToOneDrive:(self.userPicture) completion:^(NSString *webUrl, NSError *error) {
                    if (!error) {
                        self.pictureWebUrl = webUrl;
                        dispatch_async(dispatch_get_main_queue(), ^{
                            self.sendMailButton.enabled = true;
                        });
                    } else {
                        dispatch_async(dispatch_get_main_queue(), ^{
                            NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                            self.statusTextView.text = NSLocalizedString(@"PICTURE_UPLOAD_FAILURE", comment: "");
                        });
                    }
                }];
            }];
        }
    }];
   ```

1. <span data-ttu-id="f8e10-172">Abra **SendMailViewController.m.**</span><span class="sxs-lookup"><span data-stu-id="f8e10-172">Open **SendMailViewController.m.**</span></span> <span data-ttu-id="f8e10-173">na pasta Controladores e adicione o método auxiliar a seguir à classe</span><span class="sxs-lookup"><span data-stu-id="f8e10-173">in the Controllers folder and add the following helper method to the class</span></span>
```objectivec
  //Create a sample test message to send to specified user account
  -(MSGraphMessage*) getSampleMessage{
      MSGraphMessage *message = [[MSGraphMessage alloc]init];
      MSGraphRecipient *toRecipient = [[MSGraphRecipient alloc]init];
      MSGraphEmailAddress *email = [[MSGraphEmailAddress alloc]init];
    
      //need to get email text field for send to!
    
      email.address = self.emailAddress;
      toRecipient.emailAddress = email;
    
      NSMutableArray *toRecipients = [[NSMutableArray alloc]init];
      [toRecipients addObject:toRecipient];
    
      message.subject = NSLocalizedString(@"MAIL_SUBJECT", comment: "");
    
      MSGraphItemBody *emailBody = [[MSGraphItemBody alloc]init];
      NSString *htmlContentPath = [[NSBundle mainBundle] pathForResource:@"EmailBody" ofType:@"html"];
      NSString *htmlContentString = [NSString stringWithContentsOfFile:htmlContentPath encoding:NSUTF8StringEncoding error:nil];
    
      emailBody.content = htmlContentString;
      NSString *replaceString = @"a href=";
      replaceString = [replaceString stringByAppendingString:(self.pictureWebUrl)];
      emailBody.content = [emailBody.content stringByReplacingOccurrencesOfString:(@"a href=%s") withString:(replaceString)];
      emailBody.contentType = [MSGraphBodyType html];
      message.body = emailBody;
    
      message.toRecipients = toRecipients;
    
      MSGraphFileAttachment *fileAttachment= [[MSGraphFileAttachment alloc]init];
      fileAttachment.oDataType = @"#microsoft.graph.fileAttachment";
      fileAttachment.contentType = @"image/png";
    
      NSString *decodedString = [UIImagePNGRepresentation(self.userPicture) base64EncodedStringWithOptions:NSDataBase64EncodingEndLineWithCarriageReturn];
    
      fileAttachment.contentBytes = decodedString;
      fileAttachment.name = @"me.png";
      message.attachments = [message.attachments arrayByAddingObject:(fileAttachment)];
      return message;
    
    }
```
3. <span data-ttu-id="f8e10-174">Abra **SendMailViewController.m**. Adicione o método a seguir à classe.</span><span class="sxs-lookup"><span data-stu-id="f8e10-174">Open **SendMailViewController.m** Add the following method to the class.</span></span>
<span data-ttu-id="f8e10-175">**uploadPictureToOneDrive** carrega a imagem de perfil do [usuário](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user) de suas informações de [usuário](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user) e retorna a URL de compartilhamento da Web a ser inserida no corpo do email que é enviado pelo exemplo.</span><span class="sxs-lookup"><span data-stu-id="f8e10-175">**uploadPictureToOneDrive** uploads the [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user)'s profile picture from their [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user) information and returns the web sharing Url to be embedded in the body of the email that is sent by the sample.</span></span>

  ```objectivec
  -(void) uploadPictureToOneDrive: (UIImage *) image completion:(void(^) (NSString*, NSError*))completionBlock{
    
    NSData *data = UIImagePNGRepresentation(image);
    [[[[[[[self.graphClient me]
          drive]
         root]
        children]
       driveItem:(@"me.png")]
      contentRequest]
     uploadFromData:(data) completion:^(MSGraphDriveItem *response, NSError *error) {
         
         if (!error) {
             NSString *webUrl = response.webUrl;
             completionBlock(webUrl, error);
         } else {
             dispatch_async(dispatch_get_main_queue(), ^{
                 self.statusTextView.text =  NSLocalizedString(@"USER_GET_PICTURE_FAILURE", comment: "");
                 NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
             });
         }
     }];
    }
  ```
4. <span data-ttu-id="f8e10-176">Abra **SendMailViewController.m** e adicione o método a seguir à classe.</span><span class="sxs-lookup"><span data-stu-id="f8e10-176">Open **SendMailViewController.m** and add the following method to the class.</span></span> 
<span data-ttu-id="f8e10-177">**getUserPicture** retorna a imagem de perfil do [usuário](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user), caso esteja disponível.</span><span class="sxs-lookup"><span data-stu-id="f8e10-177">**getUserPicture** returns the [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user)'s profile picture if it is available.</span></span>
   ```objectivec
   -(void) getUserPicture: (NSString *)url completion:(void(^) (UIImage*, NSError*))completionBlock {
    
    [[[self.graphClient me] photoValue] downloadWithCompletion:^(NSURL *location, NSURLResponse *response, NSError *error) {
        //code
        if (!error) {
            NSData *data = [NSData dataWithContentsOfURL:location];
            UIImage *img = [[UIImage alloc] initWithData:data];
            completionBlock(img, error);
        } else{
            completionBlock(nil, error);

        }
    }];
    }

   ```
3. <span data-ttu-id="f8e10-178">Abra **SendMailViewcontroller.m** e adicione o método a seguir à classe.</span><span class="sxs-lookup"><span data-stu-id="f8e10-178">Open **SendMailViewcontroller.m** and add the following method to the class.</span></span>
<span data-ttu-id="f8e10-179">Esse método obtém o recurso [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user) que representa o usuário autenticado e armazena em cache os campos necessários para obter a imagem do perfil do usuário e enviar um email.</span><span class="sxs-lookup"><span data-stu-id="f8e10-179">This method gets the [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user) resource representing the authenticated user and caches the fields necessary to get the user's profile picture and send an email.</span></span>
   ```objectivec
   //Retrieve the logged in user's display name and email address
   -(void) getUserInfo: (NSString *)url completion:(void(^) ( NSError*))completionBlock{
    
    [[[self.graphClient me]request]getWithCompletion:^(MSGraphUser *response, NSError *error) {
        if(!error){
            dispatch_async(dispatch_get_main_queue(), ^{
                self.emailAddress = response.userPrincipalName;
                self.emailTextField.text = self.emailAddress;
                self.headerLabel.text = [NSString stringWithFormat:(NSLocalizedString(@"HI_USER", comment "")), response.displayName];
                self.statusTextView.text =  NSLocalizedString(@"USER_INFO_LOAD_SUCCESS", comment: "");
            });

            completionBlock(nil);
        }
        else{
            dispatch_async(dispatch_get_main_queue(), ^{
                self.statusTextView.text =  NSLocalizedString(@"USER_INFO_LOAD_FAILURE", comment: "");
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
            });
            completionBlock(error);
        }
    }];
    
   }

   ```
3. <span data-ttu-id="f8e10-180">Abra **SendMailViewController.m**. Adicione o método de email de envio a seguir à classe.</span><span class="sxs-lookup"><span data-stu-id="f8e10-180">Open **SendMailViewController.m** Add the following send mail method to the class.</span></span>
<span data-ttu-id="f8e10-181">**getSampleMessage** cria um exemplo de rascunho de email em HTML para fins de demonstração.</span><span class="sxs-lookup"><span data-stu-id="f8e10-181">**getSampleMessage** creates a draft HTML sample mail to use for demo purposes.</span></span> <span data-ttu-id="f8e10-182">O próximo método, **sendMail**, usa essa mensagem e executa a solicitação para enviá-la.</span><span class="sxs-lookup"><span data-stu-id="f8e10-182">The next method, **sendMail**, then takes that message and executes the request to send it.</span></span> <span data-ttu-id="f8e10-183">Novamente o destinatário padrão é o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="f8e10-183">Again the default recipient is the signed-in user.</span></span>


  ```objectivec
   //Send mail to the specified user in the email text field
   -(void) sendMail {
    MSGraphMessage *message = [self getSampleMessage];
    MSGraphUserSendMailRequestBuilder *requestBuilder = [[self.graphClient me]sendMailWithMessage:message saveToSentItems:true];
    NSLog(@"%@", requestBuilder);
    MSGraphUserSendMailRequest *mailRequest = [requestBuilder request];
    [mailRequest executeWithCompletion:^(NSDictionary *response, NSError *error) {
        if(!error){
            NSLog(@"response %@", response);
             dispatch_async(dispatch_get_main_queue(), ^{
                self.statusTextView.text = NSLocalizedString(@"SEND_SUCCESS", comment: "");
                self.descriptionLabel.text = @"Check your inbox. You have a new message :)";
            });
        }
        else {
            dispatch_async(dispatch_get_main_queue(), ^{
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                self.statusTextView.text = NSLocalizedString(@"SEND_FAILURE", comment: "");
            });
        }
    }];
   }
   ```



## <a name="run-the-app"></a><span data-ttu-id="f8e10-184">Executar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8e10-184">Run the app</span></span>
1. <span data-ttu-id="f8e10-p121">Antes de executar o exemplo, será necessário fornecer a identificação do cliente que você recebeu do processo de registro na seção **Registrar o aplicativo.** Abra **AuthenticationConstants.m** na pasta **Application**. Observe que você pode adicionar o valor de ClientID do processo de registro, na parte superior do arquivo.</span><span class="sxs-lookup"><span data-stu-id="f8e10-p121">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.** Open **AuthenticationConstants.m** under the **Application** folder. You'll see that the ClientID from the registration process can be added to the top of the file.:</span></span>  
   ```objectivec
   // You will set your application's clientId
   NSString * const kClientId    = @"ENTER_YOUR_CLIENT_ID";
   NSString * const kScopes = @"https://graph.microsoft.com/User.Read, https://graph.microsoft.com/Mail.ReadWrite, https://graph.microsoft.com/Mail.Send, https://graph.microsoft.com/Files.ReadWrite";
   ```      

><span data-ttu-id="f8e10-p122">Observação: Você notará que foram configurados os seguintes escopos de permissão para esse projeto: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. As chamadas de serviço usadas neste projeto, que enviam emails para sua conta de email e recuperam algumas informações de perfil (Nome de Exibição, Endereço de Email) exigem essas permissões para que o aplicativo seja executado corretamente.</span><span class="sxs-lookup"><span data-stu-id="f8e10-p122">Note: You'll notice that the following permission scopes have been configured for this project: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address) require these permissions for the app to run properly.</span></span>

2. <span data-ttu-id="f8e10-190">Execute o exemplo, toque em **Conexão**, entre com sua conta pessoal ou sua conta corporativa ou de estudante e conceda as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="f8e10-190">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="f8e10-p123">Escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão.</span><span class="sxs-lookup"><span data-stu-id="f8e10-p123">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f8e10-193">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f8e10-193">Next steps</span></span>
- <span data-ttu-id="f8e10-194">Experimente a API REST usando o [Explorador do Graph](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="f8e10-194">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="f8e10-195">Encontre exemplos de operações comuns para operações de REST e SDK no [Exemplo de trechos de código do iOS Objective C do Microsoft Graph](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span><span class="sxs-lookup"><span data-stu-id="f8e10-195">Find examples of common operations for both REST and SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="f8e10-196">Confira também</span><span class="sxs-lookup"><span data-stu-id="f8e10-196">See also</span></span>
- [<span data-ttu-id="f8e10-197">SDK do Microsoft Graph para iOS</span><span class="sxs-lookup"><span data-stu-id="f8e10-197">Microsoft Graph SDK for iOS</span></span>](https://github.com/microsoftgraph/msgraph-sdk-ios)
- [<span data-ttu-id="f8e10-198">Protocolos do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="f8e10-198">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="f8e10-199">Tokens do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="f8e10-199">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-tokens/)
