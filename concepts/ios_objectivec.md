# <a name="get-started-with-microsoft-graph-in-an-objectve-c-ios-app"></a>Introdução ao Microsoft Graph em um aplicativo Objective C iOS

> **Criando aplicativos para clientes corporativos?** O aplicativo pode não funcionar caso o cliente corporativo habilite os recursos Enterprise Mobility + Security, como <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">acesso condicional ao dispositivo</a>. Nesse caso, pode ser que você não esteja ciente e seu cliente pode enfrentar problemas de erro. 

> Para dar suporte a **todos os clientes corporativos**, em **todos os cenários corporativos**, use o ponto de extremidade do Microsoft Azure AD e gerencie seus aplicativos usando o [Portal do Azure](https://aka.ms/aadapplist). Para saber mais, confira o tópico [Decidindo entre os pontos de extremidade do Microsoft Azure AD e do Microsoft Azure AD versão 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

Este artigo descreve as tarefas obrigatórias para obter um token de acesso do [ponto de extremidade do Azure AD v2.0](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) e chamar o Microsoft Graph. Ele orienta você em relação ao código dentro do [Exemplo de conexão com o Office 365 para iOS (SDK)](https://github.com/microsoftgraph/ios-objectivec-connect-sample) para explicar os principais conceitos que você tem que implementar em um aplicativo que usa o Microsoft Graph. Ele descreve como acessar o Microsoft Graph usando [SDK do Microsoft Graph para iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).

Você pode baixar a versão do aplicativo que você criará a partir deste repositório do GitHub:

* [Exemplo de conexão com o Office 365 para iOS usando o SDK do Microsoft Graph](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

A imagem a seguir mostra o aplicativo que você criará.

![O passo a passo do exemplo de conexão mostra como conectar e enviar um email no aplicativo](./images/iOSConnectWalkthrough.png)


O fluxo de trabalho será conectar/autenticar ao Microsoft Graph, entrar com sua conta pessoal ou corporativa e finalmente enviar um email para um destinatário.

**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) para começar a usar rapidamente.

## <a name="prerequisites"></a>Pré-requisitos

Para começar, será necessário: 

* [Xcode](https://developer.apple.com/xcode/downloads/) da Apple
* Instalação do [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) como um gerente de dependências
* Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)
* O [Projeto inicial do Microsoft Graph para iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample). Este modelo contém classes às quais você adicionará código. Para obter este projeto, clone ou baixe o exemplo de projeto deste local, e você trabalhará com o espaço de trabalho dentro da pasta **starter-project** (**ios-objectivec-connect-sample.xcworkspace**).

## <a name="register-the-app"></a>Registrar o aplicativo
 
1. Entre no [Portal de Registro do Aplicativo](https://apps.dev.microsoft.com/) usando sua conta pessoal ou sua conta corporativa ou de estudante.
2. Selecione **Adicionar um aplicativo**.
3. Insira um nome para o aplicativo e selecione **Criar aplicativo**.
    
    A página de registro é exibida, listando as propriedades do seu aplicativo.
 
4. Em **Plataformas**, selecione **Adicionar plataforma**.
5. Selecione **Plataforma nativa**.
6. Copie a ID de Cliente para a área de transferência. Você precisará inserir esse valor no exemplo de aplicativo.

    Essa ID de aplicativo é o identificador exclusivo do aplicativo. 

7. Selecione **Salvar**.

## <a name="importing-the-project-dependencies"></a>Importando as dependências do projeto

1. Clonar este repositório, [Exemplo de conexão com o Office 365 para iOS usando o SDK do Microsoft Graph](https://github.com/microsoftgraph/ios-objectivec-connect-sample). 
>IMPORTANTE: Use o exemplo na pasta starter-project, não o exemplo na raiz do projeto.

2. Use o CocoaPods para importar as dependências de autenticação e o SDK do Microsoft Graph. Este aplicativo de exemplo já contém um podfile que colocará os pods no projeto. Navegue até a pasta **starter-project** no aplicativo **Terminal** e, do **Terminal**, execute:

        pod install

   Você receberá a confirmação de que os pods foram importados para o projeto. Para saber mais, confira [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html).


## <a name="enable-keychain-sharing"></a>Habilitar o compartilhamento de chaves
 
Para o Xcode8, você deve adicionar o grupo de chaves para que o aplicativo não falhe ao acessar a chave. Para adicionar o grupo de chaves:
 
1. Escolha o projeto, no painel do gerente de projetos do Xcode. (⌘ + 1).
 
2. Selecione **iOS-ObjectiveC-Connect-Sample**.
 
3. Na guia Recursos, habilite o **Compartilhamento de chaves**.
 
4. Adicione **com.microsoft.ios-objectivec-connect-sample** aos Grupos de Chaves.
 

## <a name="authenticating-with-microsoft-graph"></a>Autenticando com o Microsoft Graph

Para rever o fluxo de trabalho de interface do usuário, o aplicativo fará o usuário autenticar e, em seguida, ele terá a capacidade de enviar um email para um usuário especificado. Para realizar solicitações ao serviço do Microsoft Graph, um provedor de autenticação deverá ser fornecido para autenticar solicitações HTTPS com um token de portador OAuth 2.0 apropriado. No exemplo de projeto, há uma classe de autenticação já oculta chamada **AuthenticationProvider.m.** Vamos adicionar uma função para solicitar e adquirir um token de acesso para chamar a API do Microsoft Graph. 

1. Abra o espaço de trabalho do projeto Xcode (**iOS-ObjectiveC-Connect-Sample.xcworkspace**) na pasta **starter-project**, navegue até a pasta **Authentication** e abra o arquivo **AuthenticationProvider.m.** Adicione o código a seguir a essa classe.

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

2. Em seguida, adicione o método ao arquivo de cabeçalho. Abra o arquivo **AuthenticationProvider.h** e adicione o código a seguir a esta classe.
   ```objectivec
   -(void) connectToGraphWithClientId:(NSString *)clientId
                               scopes:(NSArray *)scopes
                           completion:(void (^)(NSError *error))completion;
   ```

2. Finalmente chamaremos esse método de **ConnectViewController.m**. Este controlador é a visualização padrão que o aplicativo carrega, e há um único botão chamado **Conectar** que o usuário toca que iniciará o processo de autenticação. Este método usa dois parâmetros, a **ID do cliente** e os **escopos**, que discutiremos de maneira mais detalhada abaixo. Adicione a ação a seguir a **ConnectViewController.m**.

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

## <a name="send-an-email-with-microsoft-graph"></a>Enviar um email com o Microsoft Graph

Depois de configurar o projeto para ser capaz de autenticar, as próximas tarefas são enviar um email para um usuário usando a API do Microsoft Graph. Por padrão, o usuário conectado será o destinatário, mas você tem a capacidade de alterá-lo para qualquer outro destinatário. O código com o qual trabalharemos aqui está localizado na pasta **Controllers** e na classe **SendMailViewController.m.** Você verá que há outro código representado aqui para a interface do usuário e um método auxiliar para recuperar informações de perfil de usuário do serviço do Microsoft Graph. Vamos nos concentrar nos métodos para criar uma mensagem de email e enviar essa mensagem.

1. Abra **SendMailViewController.m** na pasta controladores e adicione o código a seguir para o método **viewDidLoad**, após `self.graphClient = [MSGraphClient client]`
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

1. Abra **SendMailViewController.m.** na pasta Controladores e adicione o método auxiliar a seguir à classe
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
3. Abra **SendMailViewController.m**. Adicione o método a seguir à classe.
**uploadPictureToOneDrive** carrega a imagem de perfil do [usuário](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) de suas informações de [usuário](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) e retorna a URL de compartilhamento da Web a ser inserida no corpo do email que é enviado pelo exemplo.

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
4. Abra **SendMailViewController.m** e adicione o método a seguir à classe. 
**getUserPicture** retorna a imagem de perfil do [usuário](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user), caso esteja disponível.
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
3. Abra **SendMailViewcontroller.m** e adicione o método a seguir à classe.
Esse método obtém o recurso [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) que representa o usuário autenticado e armazena em cache os campos necessários para obter a imagem do perfil do usuário e enviar um email.
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
3. Abra **SendMailViewController.m**. Adicione o método de email de envio a seguir à classe.
**getSampleMessage** cria um exemplo de rascunho de email em HTML para fins de demonstração. O próximo método, **sendMail**, usa essa mensagem e executa a solicitação para enviá-la. Novamente o destinatário padrão é o usuário conectado.


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



## <a name="run-the-app"></a>Executar o aplicativo
1. Antes de executar o exemplo, será necessário fornecer a identificação do cliente que você recebeu do processo de registro na seção **Registrar o aplicativo.** Abra **AuthenticationConstants.m** na pasta **Application**. Observe que você pode adicionar o valor de ClientID do processo de registro, na parte superior do arquivo.  
   ```objectivec
   // You will set your application's clientId
   NSString * const kClientId    = @"ENTER_YOUR_CLIENT_ID";
   NSString * const kScopes = @"https://graph.microsoft.com/User.Read, https://graph.microsoft.com/Mail.ReadWrite, https://graph.microsoft.com/Mail.Send, https://graph.microsoft.com/Files.ReadWrite";
   ```      

>Observação: Você notará que foram configurados os seguintes escopos de permissão para esse projeto: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. As chamadas de serviço usadas neste projeto, que enviam emails para sua conta de email e recuperam algumas informações de perfil (Nome de Exibição, Endereço de Email) exigem essas permissões para que o aplicativo seja executado corretamente.

2. Execute o exemplo, toque em **Conexão**, entre com sua conta pessoal ou sua conta corporativa ou de estudante e conceda as permissões solicitadas.

3. Escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão.

## <a name="next-steps"></a>Próximas etapas
- Experimente a API REST usando o [Explorador do Graph](https://graph.microsoft.io/graph-explorer).
- Encontre exemplos de operações comuns para operações de REST e SDK no [Exemplo de trechos de código do iOS Objective C do Microsoft Graph](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).

## <a name="see-also"></a>Confira também
- [SDK do Microsoft Graph para iOS](https://github.com/microsoftgraph/msgraph-sdk-ios)
- [Protocolos do Azure AD v2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Tokens do Azure AD v2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
