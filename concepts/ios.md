# <a name="get-started-with-microsoft-graph-in-an-ios-app"></a>Introdução ao Microsoft Graph em um aplicativo iOS

> **Criando aplicativos para clientes corporativos?** O aplicativo pode não funcionar caso o cliente corporativo habilite os recursos Enterprise Mobility + Security, como <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">acesso condicional ao dispositivo</a>. Nesse caso, pode ser que você não esteja ciente e seu cliente pode enfrentar problemas de erro. 

> Para fornecer suporte a **todos os clientes corporativos**, em **todos os cenários corporativos**, use o ponto de extremidade do Microsoft Azure AD e gerencie os aplicativos usando o [Portal de Gerenciamento do Microsoft Azure](https://aka.ms/aadapplist). Para saber mais, confira o tópico [Decidindo entre os pontos de extremidade do Azure AD e do Azure AD v2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

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
* Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](http://dev.office.com/devprogram)
* O [Projeto inicial do Microsoft Graph para iOS](https://github.com/microsoftgraph/ios-objectivec-connect-sample). Este modelo contém classes às quais você adicionará código. Para obter este projeto, clone ou baixe o exemplo de projeto deste local, e você trabalhará com o espaço de trabalho dentro da pasta **starter-project** (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**).

## <a name="register-the-app"></a>Registrar o aplicativo
 
1. Entre no [Portal de Registro do Aplicativo](https://apps.dev.microsoft.com/) usando sua conta pessoal ou sua conta corporativa ou de estudante.
2. Selecione **Adicionar um aplicativo**.
3. Insira um nome para o aplicativo e selecione **Criar aplicativo**.
    
    A página de registro é exibida, listando as propriedades do seu aplicativo.
 
4. Em **Plataformas**, selecione **Adicionar plataforma**.
5. Selecione **Plataforma móvel**.
6. Copie a ID de Cliente para a área de transferência. Você precisará inserir esse valor no exemplo de aplicativo.

    Essa ID de aplicativo é o identificador exclusivo do aplicativo. 

7. Selecione **Salvar**.

## <a name="importing-the-project-dependencies"></a>Importando as dependências do projeto

1. Clonar este repositório, [Exemplo de conexão com o Office 365 para iOS usando o SDK do Microsoft Graph](https://github.com/microsoftgraph/ios-objectivec-connect-sample). **Lembre-se de que você usará o exemplo na pasta starter-project e não o exemplo na raiz do projeto.**
2. Use o CocoaPods para importar as dependências de autenticação e o SDK do Microsoft Graph. Este aplicativo de exemplo já contém um podfile que colocará os pods no projeto. Navegue até a pasta **starter-project** no aplicativo **Terminal** e, do **Terminal**, execute:

        pod install

   Você receberá a confirmação de que os pods foram importados para o projeto. Para saber mais, confira [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html).


## <a name="enable-keychain-sharing"></a>Habilitar o compartilhamento de chaves
 
Para o Xcode8, você deve adicionar o grupo de chaves para que o aplicativo não falhe ao acessar a chave. Para adicionar o grupo de chaves:
 
1. Escolha o projeto, no painel do gerente de projetos do Xcode. (⌘ + 1).
 
2. Selecione **O365-iOS-Microsoft-Graph-SDK**.
 
3. Na guia Recursos, habilite o **Compartilhamento de chaves**.
 
4. Adicione **com.microsoft.O365-iOS-Microsoft-Graph-SDK** aos grupos de chaves.
 

## <a name="authenticating-with-microsoft-graph"></a>Autenticando com o Microsoft Graph

Para rever o fluxo de trabalho de interface do usuário, o aplicativo fará o usuário autenticar e, em seguida, ele terá a capacidade de enviar um email para um usuário especificado. Para realizar solicitações ao serviço do Microsoft Graph, um provedor de autenticação deverá ser fornecido para autenticar solicitações HTTPS com um token de portador OAuth 2.0 apropriado. No exemplo de projeto, há uma classe de autenticação já oculta chamada **AuthenticationProvider.m.** Vamos adicionar uma função para solicitar e adquirir um token de acesso para chamar a API do Microsoft Graph. 

1. Abra o espaço de trabalho do projeto Xcode (**O365-iOS-Microsoft-Graph-SDK.xcworkspace**) na pasta **starter-project** e navegue até a pasta **Authentication** e abra o arquivo **AuthenticationProvider.m.** Adicione o código a seguir a essa classe.

        -(void) connectToGraphWithClientId:(NSString *)clientId scopes:(NSArray *)scopes completion:(void (^)    (NSError *))completion{
            [NXOAuth2AuthenticationProvider setClientId:kClientId
                                              scopes:scopes];
    
    
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

2. Em seguida, adicione o método ao arquivo de cabeçalho. Abra o arquivo **AuthenticationProvider.h** e adicione o código a seguir a esta classe.

        -(void) connectToGraphWithClientId:(NSString *)clientId
                            scopes:(NSArray *)scopes
                        completion:(void (^)(NSError *error))completion;



2. Finalmente chamaremos esse método de **ConnectViewController.m**. Este controlador é a visualização padrão que o aplicativo carrega, e há um único botão chamado **Conectar** que o usuário toca que iniciará o processo de autenticação. Este método usa dois parâmetros, a **ID do cliente** e os **escopos**, que discutiremos de maneira mais detalhada abaixo. Adicione a ação a seguir a **ConnectViewController.m**.

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

## <a name="send-an-email-with-microsoft-graph"></a>Enviar um email com o Microsoft Graph

Depois de configurar o projeto para ser capaz de autenticar, as próximas tarefas são enviar um email para um usuário usando a API do Microsoft Graph. Por padrão, o usuário conectado será o destinatário, mas você tem a capacidade de alterá-lo para qualquer outro destinatário. O código com o qual trabalharemos aqui está localizado na pasta **Controllers** e na classe **SendMailViewController.m.** Você verá que há outro código representado aqui para a interface do usuário e um método auxiliar para recuperar informações de perfil de usuário do serviço do Microsoft Graph. Vamos nos concentrar nos métodos para criar uma mensagem de email e enviar essa mensagem.

1. Abra **SendMailViewController.m.** na pasta Controllers e adicione o seguinte método auxiliar à classe:

        // Create a sample test message to send to specified user account
        -(MSGraphMessage*) getSampleMessage{
            MSGraphMessage *message = [[MSGraphMessage alloc]init];
            MSGraphRecipient *toRecipient = [[MSGraphRecipient alloc]init];
            MSGraphEmailAddress *email = [[MSGraphEmailAddress alloc]init];
    
            email.address = self.emailAddress;
            toRecipient.emailAddress = email;
    
            NSMutableArray *toRecipients = [[NSMutableArray alloc]init];
            [toRecipients addObject:toRecipient];
    
            message.subject = NSLocalizedString(@"MAIL_SUBJECT", comment: "");
    
            MSGraphItemBody *emailBody = [[MSGraphItemBody alloc]init];
            NSString *htmlContentPath = [[NSBundle mainBundle] pathForResource:@"EmailBody" ofType:@"html"];
            NSString *htmlContentString = [NSString stringWithContentsOfFile:htmlContentPath encoding:NSUTF8StringEncoding error:nil];
    
            emailBody.content = htmlContentString;
            emailBody.contentType = [MSGraphBodyType html];
            message.body = emailBody;
    
            message.toRecipients = toRecipients;
    
            return message;
    
        }


2. Abra **SendMailViewController.m.** Adicione o método de email de envio a seguir à classe.  

        //Send mail to the specified user in the email text field
        -(void) sendMail {   
            MSGraphMessage *message = [self getSampleMessage];
            MSGraphUserSendMailRequestBuilder *requestBuilder = [[self.graphClient me]sendMailWithMessage:message saveToSentItems:true];
            NSLog(@"%@", requestBuilder);
            MSGraphUserSendMailRequest *mailRequest = [requestBuilder request];
            [mailRequest executeWithCompletion:^(NSDictionary *response, NSError *error) {
                if(!error){
                    NSLog(@"response %@", response);
                    NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
            
                    dispatch_async(dispatch_get_main_queue(), ^{
                        self.statusTextView.text = NSLocalizedString(@"SEND_SUCCESS", comment: "");
                });
            }
            else {
                NSLog(NSLocalizedString(@"ERROR", ""), error.localizedDescription);
                    self.statusTextView.text = NSLocalizedString(@"SEND_FAILURE", comment: "");
                }
            }];
    
        }

Então **getSampleMessage** cria um exemplo de rascunho de email em HTML para fins de demonstração. O próximo método **sendMail**, em seguida, usa essa mensagem e executa a solicitação para enviá-la. Novamente o destinatário padrão é o usuário conectado.


## <a name="run-the-app"></a>Executar o aplicativo
1. Antes de executar o exemplo, será necessário fornecer a identificação do cliente que você recebeu do processo de registro na seção **Registrar o aplicativo.** Abra **AuthenticationConstants.m** na pasta **Application**. Observe que você pode adicionar o valor de ClientID do processo de registro, na parte superior do arquivo.  

        // You will set your application's clientId
        NSString * const kClientId    = @"ENTER_CLIENT_ID_HERE";
        NSString * const kScopes = @"https://graph.microsoft.com/Mail.Send, https://graph.microsoft.com/User.Read, offline_access";
Observação: Você notará que foram configurados os seguintes escopos de permissão para esse projeto: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. As chamadas de serviço usadas neste projeto, que enviam emails para sua conta de email e recuperam algumas informações de perfil (Nome de Exibição, Endereço de Email) exigem essas permissões para que o aplicativo seja executado corretamente.

2. Execute o exemplo, toque em **Conexão**, entre com sua conta pessoal ou sua conta corporativa ou de estudante e conceda as permissões solicitadas.

3. Escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão.

## <a name="next-steps"></a>Próximas etapas
- Experimente a API REST, usando o [Explorador do Graph](https://graph.microsoft.io/graph-explorer).
- Encontre exemplos de operações comuns para operações de REST e SDK no [Exemplo de trechos de código do iOS Objective C do Microsoft Graph](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).

## <a name="see-also"></a>Ver também
- [SDK do Microsoft Graph para iOS](https://github.com/microsoftgraph/msgraph-sdk-ios)
- [Protocolos do Azure AD v2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Tokens do Azure AD v2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
