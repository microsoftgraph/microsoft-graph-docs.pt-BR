# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a>Introdução ao Microsoft Graph em um aplicativo Swift iOS

> **Criando aplicativos para clientes corporativos?** O aplicativo pode não funcionar caso o cliente corporativo habilite os recursos Enterprise Mobility + Security, como <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">acesso condicional ao dispositivo</a>. Nesse caso, pode ser que você não esteja ciente e seu cliente pode enfrentar problemas de erro. 

> Para dar suporte a **todos os clientes corporativos**, em **todos os cenários corporativos**, use o ponto de extremidade do Microsoft Azure AD e gerencie seus aplicativos usando o [Portal do Azure](https://aka.ms/aadapplist). Para saber mais, confira o tópico [Decidindo entre os pontos de extremidade do Microsoft Azure AD e do Microsoft Azure AD versão 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

Este artigo descreve as tarefas obrigatórias para obter um token de acesso do [ponto de extremidade do Azure AD v2.0](https://developer.microsoft.com/pt-BR/graph/docs/concepts/converged_auth) e chamar o Microsoft Graph. Ele orienta você em relação ao código dentro do [Exemplo de conexão com o Office 365 para iOS (SDK)](https://github.com/microsoftgraph/ios-swift-connect-sample) para explicar os principais conceitos que você tem que implementar em um aplicativo que usa o Microsoft Graph. Ele descreve como acessar o Microsoft Graph usando [SDK do Microsoft Graph para iOS](https://github.com/microsoftgraph/msgraph-sdk-ios).

Você pode baixar a versão do aplicativo que você criará a partir deste repositório do GitHub:

* [Exemplo de conexão com o Office 365 para iOS usando o SDK do Microsoft Graph](https://github.com/microsoftgraph/ios-objectivec-connect-sample)

A imagem a seguir mostra o aplicativo que você criará.

![O passo a passo do exemplo de conexão mostra como conectar e enviar um email no aplicativo](./images/iOSConnectWalkthrough.png)


O fluxo de trabalho será conectar/autenticar ao Microsoft Graph, entrar com sua conta pessoal ou corporativa e finalmente enviar um email para um destinatário.

**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://graph.microsoft.io/pt-BR/getting-started) para começar a usar rapidamente.

## <a name="prerequisites"></a>Pré-requisitos

Para começar, será necessário: 

* [Xcode](https://developer.apple.com/xcode/downloads/) da Apple
* Instalação do [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) como um gerente de dependências
* Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](http://dev.office.com/devprogram)
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

Para rever o fluxo de trabalho de interface do usuário, o aplicativo fará o usuário autenticar e, em seguida, ele terá a capacidade de enviar um email para um usuário especificado. Para realizar solicitações ao serviço do Microsoft Graph, um provedor de autenticação deverá ser fornecido para autenticar solicitações HTTPS com um token de portador OAuth 2.0 apropriado. No projeto de exemplo, há uma estrutura de autenticação já fragmentada chamada **Authentication.swift.** Vamos adicionar uma função para solicitar e adquirir um token de acesso para chamar a API do Microsoft Graph. 

1. Abra o espaço de trabalho do projeto Xcode (**Graph-iOS-Swift-Connect.xcworkspace**) e abra o arquivo de extensão de estrutura **Authentication.swift**. Encontre o código a seguir nessa extensão.


  ```swift
     /**
     Authenticates to Microsoft Graph. 
     If a user has previously signed in before and not disconnected, silent log in
     will take place. 
     If not, authentication will ask for credentials
     */
    func connectToGraph(withClientId clientId: String,
                                     scopes: [String],
                                     completion:@escaping (_ error: MSGraphError?) -> Void) {
    
        // Set client ID
        NXOAuth2AuthenticationProvider.setClientId(clientId, scopes: scopes)
        
        // Try silent log in. This will attempt to sign in if there is a previous successful
        // sign in user information.
        if NXOAuth2AuthenticationProvider.sharedAuth().loginSilent() == true {
            completion(nil)
        }
        // Otherwise, present log in controller.
        else {
            NXOAuth2AuthenticationProvider.sharedAuth()
                .login(with: nil) { (error: Error?) in
                    
                    if let nserror = error {
                        completion(MSGraphError.nsErrorType(error: nserror as NSError))
                    }
                    else {
                        completion(nil)
                    }
            }
        }
    }
  ```


2. Chamaremos esse método de **ConnectViewController.swift**. Este controlador é a exibição padrão que o aplicativo carrega, e há um único botão chamado **Conectar**, no qual o usuário tocará, que iniciará o processo de autenticação. Este método usa um parâmetro, **scopes**. Discutiremos scopes de forma mais detalhada abaixo. Adicione a ação a seguir a **ConnectViewController.swift**.

  ```swift
  // MARK: Authentication
  private extension ConnectViewController {
    func authenticate() {
        loadingUI(show: true)
        
        let clientId = ApplicationConstants.clientId
        let scopes = ApplicationConstants.scopes
        
        authentication.connectToGraph(withClientId: clientId, scopes: scopes) {
            (error) in
            
            defer {self.loadingUI(show: false)}
            
            if let graphError = error {
                switch graphError {
                case .nsErrorType(let nsError):
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    self.showError(message: NSLocalizedString("CHECK_LOG_ERROR", comment: ""))
                }
            }
            else {
                self.performSegue(withIdentifier: "showSendMail", sender: nil)
            }
        }
    }
  }

  ```

## <a name="send-an-email-with-microsoft-graph"></a>Enviar um email com o Microsoft Graph

Após configurar o projeto para fazer a autenticação, as próximas tarefas são obter o endereço de email, o nome de exibição e a foto do perfil do usuário autenticado. Depois que o exemplo obtém esses valores, carrega a imagem de perfil para o OneDrive e obtém a Url de compartilhamento da imagem. Por fim, ele envia um email a um usuário usando a API do Microsoft Graph. 

Por padrão, o usuário conectado será o destinatário, mas você tem a capacidade de alterá-lo para qualquer outro destinatário. O código com o qual trabalharemos aqui está na classe **SendMailViewController.swift.** Você verá que há outro código representado aqui para a interface do usuário e um método auxiliar para recuperar informações de perfil de usuário do serviço do Microsoft Graph. Vamos nos concentrar nos métodos para criar uma mensagem de email e enviar essa mensagem.

1. Abrir **SendMailViewController.swift.**  e localize o método auxiliar de criação de corpo de email na classe:

  ```swift
    /**
     Creates sample email message
     
     - parameter emailAddress: recipient email address
     
     - returns: MSGraphMessage object with given recipient. The body is created from EmailBody.html
     */
    func createSampleMessage(to emailAddress: String, picLink pictureUrl: String) -> MSGraphMessage? {
        let message = MSGraphMessage()
        
        // set recipients
        
        let _ = self.userPicture
        let toRecipient = MSGraphRecipient()
        let msEmailAddress = MSGraphEmailAddress()
        msEmailAddress.address = emailAddress
        toRecipient.emailAddress = msEmailAddress
        let toRecipientList = [toRecipient]
        message.toRecipients = toRecipientList
        message.subject = NSLocalizedString("MAIL_SUBJECT", comment: "")
        let messageBody = MSGraphItemBody()
        messageBody.contentType = MSGraphBodyType.html()
        guard let emailBodyFilePath = Bundle.main.path(forResource: "EmailBody", ofType: "html") else {return nil}
        messageBody.content = try! String(contentsOfFile: emailBodyFilePath, encoding: String.Encoding.utf8)
        messageBody.content = messageBody.content.replacingOccurrences(of: "a href=%s", with: ("a href=" + pictureUrl))
        message.body = messageBody

        if let unwrappedImage = self.userPicture {
            let fileAttachment = MSGraphFileAttachment()
            let data = UIImageJPEGRepresentation(unwrappedImage, 1.0)
            fileAttachment.contentType = "image/png"
            fileAttachment.oDataType = "#microsoft.graph.fileAttachment"
            fileAttachment.contentBytes = data?.base64EncodedString()
            fileAttachment.name = "me.png"
            message.attachments.append(fileAttachment)
        }
        return message
    }

  ```
2. encontre os métodos auxiliares a seguir para obter informações sobre o usuário, obter uma fotografia de perfil e carregar a fotografia no OneDrive:

  ```swift
      /**
     Fetches user information such as mail and display name
     */
    func getUserInfo() {
        self.sendButton.isEnabled = false
        self.statusTextView.text = NSLocalizedString("LOADING_USER_INFO", comment: "")
        
        self.graphClient.me().request().getWithCompletion {
            (user: MSGraphUser?, error: Error?) in
            if let graphError = error {
                print(NSLocalizedString("ERROR", comment: ""), graphError)
                DispatchQueue.main.async(execute: {
                    self.statusTextView.text = NSLocalizedString("GRAPH_ERROR", comment: "")
                })
            }
            else {
                guard let userInfo = user else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("USER_INFO_LOAD_FAILURE", comment: "")
                    })
                    return
                }
                DispatchQueue.main.async(execute: {
                    self.emailTextField.text = userInfo.mail
                    
                    if let displayName = userInfo.displayName {
                        self.headerLabel.text = "Hi " + displayName
                    }
                    else {
                        self.headerLabel.text = NSString(format: NSLocalizedString("HI_USER", comment: "") as NSString, "") as String
                    }
                    
                    self.statusTextView.text = NSLocalizedString("USER_INFO_LOAD_SUCCESS", comment: "")
                    self.sendButton.isEnabled = true
                })
            }
        }
    }
    
    /**
     Uploads the user's profile picture (obtained via the Graph API) to the user's OneDrive drive. The OneDrive sharing url is
     returned in the completion handler.
    */
    func uploadPictureToOneDrive(uploadFile image: UIImage?, with completion: @escaping (_ result: GraphResult<String, NSError>) ->Void) {
        
        var webUrl: String = ""
        guard let unwrappedImage = image else {
            return
        }
        let data = UIImageJPEGRepresentation(unwrappedImage, 1.0)
        self.graphClient
            .me()
            .drive()
            .root()
            .children()
            .driveItem("me.png")
            .contentRequest()
            .upload(from: data, completion: {
                (driveItem: MSGraphDriveItem?, error: Error?) in
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("UPLOAD_PICTURE_FAILURE", comment: nsError.localizedDescription)
                    })
                    return

                } else {
                    webUrl = (driveItem?.webUrl)!
                    completion(.success(webUrl))
                }
            })
    }


    /**
     Gets the user's profile picture. Returns the picture as a UIImage via completion handler
    */
    func getUserPicture(forUser upn: String, with completion: @escaping (_ result: GraphResult<UIImage, NSError>) -> Void) {
        
        //Asynchronous Graph call. Closure is invoked after getUserPicture completes. Requires @escaping attribute
        self.graphClient.me().photoValue().download {
            (url: URL?, response: URLResponse?, error: Error?) in
            
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: nsError.localizedDescription)
                    })
                    return
                }
                guard let picUrl = url else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: "User profile picture is nil")
                    })
                    return
                }
                print(picUrl)
            
                let picData = NSData(contentsOf: picUrl)
                let picImage = UIImage(data: picData! as Data)
            
                if let validPic = picImage {
                    completion(.success(validPic))
                }
                else {
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("GET_PICTURE_FAILURE", comment: "Picture data is invalid")
                    })
                }
            }
    }

  ```

3. Localize o método de envio de mail a seguir na classe.  

  ```swift
    @IBAction func sendMail(_ sender: AnyObject) {
        guard let toEmail = self.emailTextField.text else {return}
        guard let picUrl = self.userPictureUrl else {return}
        if let message = self.createSampleMessage(to: toEmail, picLink: picUrl) {
            
            let requestBuilder = graphClient.me().sendMail(with: message, saveToSentItems: false)
            let mailRequest = requestBuilder?.request()
            
            _ = mailRequest?.execute(completion: {
                (response: [AnyHashable: Any]?, error: Error?) in
                if let nsError = error {
                    print(NSLocalizedString("ERROR", comment: ""), nsError.localizedDescription)
                    DispatchQueue.main.async(execute: {
                        self.statusTextView.text = NSLocalizedString("SEND_FAILURE", comment: "")
                    })
                }
                else {
                    DispatchQueue.main.async(execute: {
                        self.descriptionLabel.text = "Check your inbox. You have a new message :)"
                        self.statusTextView.text = NSLocalizedString("SEND_SUCCESS", comment: "")
                    })
                }
            })
        }
    }

  ```


## <a name="run-the-app"></a>Executar o aplicativo
1. Antes de executar o exemplo, será necessário fornecer a identificação do cliente que você recebeu do processo de registro na seção **Registrar o aplicativo.** Abra **ApplicationConstants.swift**. Observe que você pode adicionar o valor de ClientID do processo de registro, na parte superior do arquivo.  

  ```swift
struct ApplicationConstants {
    static let clientId = "Enter_Client_Id_Here"
    static let scopes   = ["openid", "profile", "Mail.ReadWrite","mail.send","Files.ReadWrite","User.ReadBasic.All"]
}


  ```

> Observação: Você notará que foram configurados os seguintes escopos de permissão para esse projeto: **"https://graph.microsoft.com/Mail.Send", "https://graph.microsoft.com/User.Read", "offline_access"**. As chamadas de serviço usadas neste projeto, que enviam emails para sua conta de email e recuperam algumas informações de perfil (Nome de Exibição, Endereço de Email) exigem essas permissões para que o aplicativo seja executado corretamente.

2. Execute o exemplo, toque em **Conexão**, entre com sua conta pessoal ou sua conta corporativa ou de estudante e conceda as permissões solicitadas.

3. Escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão.

## <a name="next-steps"></a>Próximas etapas
- Experimente a API REST usando o [Explorador do Graph](https://graph.microsoft.io/graph-explorer).
- Encontre exemplos de operações comuns para operações de REST e SDK no [Exemplo de trechos de código do iOS Objective C do Microsoft Graph](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).

## <a name="see-also"></a>Confira também
- [Protocolos do Azure AD v2.0](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-protocols/)
- [Tokens do Azure AD v2.0](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-tokens/)
