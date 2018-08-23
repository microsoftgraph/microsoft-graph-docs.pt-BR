# <a name="get-started-with-microsoft-graph-in-a-swift-ios-app"></a><span data-ttu-id="f4f9b-101">Introdução ao Microsoft Graph em um aplicativo Swift iOS</span><span class="sxs-lookup"><span data-stu-id="f4f9b-101">Get started with Microsoft Graph in a Swift iOS App</span></span>

> <span data-ttu-id="f4f9b-p101">**Criando aplicativos para clientes corporativos?** O aplicativo pode não funcionar caso o cliente corporativo habilite os recursos Enterprise Mobility + Security, como <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">acesso condicional ao dispositivo</a>. Nesse caso, pode ser que você não esteja ciente e seu cliente pode enfrentar problemas de erro.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-p101">**Building apps for enterprise customers?** Your app may not work if your enterprise customer turns on enterprise mobility security features like <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">conditional device access</a>. In this case, you may not know and your customers may experience errors.</span></span> 

> <span data-ttu-id="f4f9b-p102">Para dar suporte a **todos os clientes corporativos**, em **todos os cenários corporativos**, use o ponto de extremidade do Microsoft Azure AD e gerencie seus aplicativos usando o [Portal do Azure](https://aka.ms/aadapplist). Para saber mais, confira o tópico [Decidindo entre os pontos de extremidade do Microsoft Azure AD e do Microsoft Azure AD versão 2.0](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span><span class="sxs-lookup"><span data-stu-id="f4f9b-p102">To support **all enterprise customers** across **all enterprise scenarios**, you must use the Azure AD endpoint and manage your apps using the [Azure portal](https://aka.ms/aadapplist). For more information, see [Deciding between the Azure AD and Azure AD v2.0 endpoints](../concepts/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).</span></span>

<span data-ttu-id="f4f9b-p103">Este artigo descreve as tarefas obrigatórias para obter um token de acesso do [ponto de extremidade do Azure AD v2.0](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) e chamar o Microsoft Graph. Ele orienta você em relação ao código dentro do [Exemplo de conexão com o Office 365 para iOS (REST)](https://github.com/microsoftgraph/ios-swift-connect-rest-sample) para explicar os principais conceitos a serem implementados em um aplicativo que usa o Microsoft Graph. Ele descreve como acessar o Microsoft Graph usando operações REST em uma **cadeia de promessas** assíncrona. As promessas no exemplo são implementadas usando o CocoaPod [mxcl/PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/README.md).</span><span class="sxs-lookup"><span data-stu-id="f4f9b-p103">This article describes the tasks required to get an access token from the [Azure AD v2.0 endpoint](https://developer.microsoft.com/en-us/graph/docs/concepts/converged_auth) and call Microsoft Graph. It walks you through the code inside the [Office 365 Connect Sample for iOS (REST)](https://github.com/microsoftgraph/ios-swift-connect-rest-sample) to explain the main concepts that you implement in an app that uses Microsoft Graph. It describes how to access Microsoft Graph by using REST operations in an asynchronous **Promise chain** pattern.  Promises in the sample are implemented by using the [mxcl/PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/README.md) CocoaPod.</span></span> 

<span data-ttu-id="f4f9b-111">O exemplo foi criado usando **XCode 9.2** e **Swift 3.2**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-111">The sample was created using **XCode 9.2** and **Swift 3.2**.</span></span>

<span data-ttu-id="f4f9b-112">Você pode baixar a versão do aplicativo que você criará deste repositório do GitHub:</span><span class="sxs-lookup"><span data-stu-id="f4f9b-112">You can download the version of the app that you'll create from this GitHub repo:</span></span>

* [<span data-ttu-id="f4f9b-113">Exemplo de conexão com o Office 365 para iOS usando o SDK do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f4f9b-113">Office 365 Connect Sample for iOS Using the Microsoft Graph SDK</span></span>](https://github.com/microsoftgraph/ios-swift-connect-rest-sample)

<span data-ttu-id="f4f9b-114">A imagem a seguir mostra o aplicativo que você criará.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-114">The following image shows the app you'll create.</span></span>

![O passo a passo do exemplo de conexão mostra como conectar e enviar um email no aplicativo](./images/iOSConnectWalkthrough.png)


<span data-ttu-id="f4f9b-116">O fluxo de trabalho autentica e autoriza o exemplo a acessar os recursos do Microsoft Graph, entra com sua conta corporativa ou pessoal e, por fim, envia um email para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-116">The workflow authenticates and authorizes the sample to access  Microsoft Graph resources, signs in with your work or personal account, and finally sends a mail to a recipient.</span></span>

<span data-ttu-id="f4f9b-p104">**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://developer.microsoft.com/en-us/graph/quick-start) para agilizar o processo.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-p104">**Don't feel like building an app?** Use the [Microsoft Graph quick start](https://developer.microsoft.com/en-us/graph/quick-start) to get up and running fast.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4f9b-119">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4f9b-119">Prerequisites</span></span>

<span data-ttu-id="f4f9b-120">Para começar, será necessário:</span><span class="sxs-lookup"><span data-stu-id="f4f9b-120">To get started, you'll need:</span></span> 

* <span data-ttu-id="f4f9b-121">[Xcode](https://developer.apple.com/xcode/downloads/) da Apple</span><span class="sxs-lookup"><span data-stu-id="f4f9b-121">[Xcode](https://developer.apple.com/xcode/downloads/) from Apple</span></span>
* <span data-ttu-id="f4f9b-122">Instalação do [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) como um gerente de dependências</span><span class="sxs-lookup"><span data-stu-id="f4f9b-122">Installation of [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html) as a dependency manager</span></span>
* <span data-ttu-id="f4f9b-123">Instalação do [Carthage](https://github.com/Carthage/Carthage) para importar e criar a biblioteca **MSAL**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-123">Installation of [Carthage](https://github.com/Carthage/Carthage) to import and build the **MSAL** library.</span></span>
* <span data-ttu-id="f4f9b-124">Instalação do Cocoapod [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md).</span><span class="sxs-lookup"><span data-stu-id="f4f9b-124">Installation of the [PromiseKit 4.5.2](https://github.com/mxcl/PromiseKit/blob/master/Documentation/Installation.md) Cocoapod.</span></span> 
* <span data-ttu-id="f4f9b-125">Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span><span class="sxs-lookup"><span data-stu-id="f4f9b-125">A [Microsoft account](https://www.outlook.com/) or a [work or school account](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program-faq#account-types)</span></span>

## <a name="register-the-app"></a><span data-ttu-id="f4f9b-126">Registrar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4f9b-126">Register the app</span></span>
 
1. <span data-ttu-id="f4f9b-127">Entre no [Portal de Registro do Aplicativo](https://apps.dev.microsoft.com/) usando sua conta pessoal ou sua conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-127">Sign into the [App Registration Portal](https://apps.dev.microsoft.com/) using either your personal or work or school account.</span></span>
2. <span data-ttu-id="f4f9b-128">Selecione **Adicionar um aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-128">Select **Add an app**.</span></span>
3. <span data-ttu-id="f4f9b-129">Insira um nome para o aplicativo e selecione **Criar aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-129">Enter a name for the app, and select **Create application**.</span></span>
    
    <span data-ttu-id="f4f9b-130">A página de registro é exibida, listando as propriedades do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-130">The registration page displays, listing the properties of your app.</span></span>
 
4. <span data-ttu-id="f4f9b-131">Em **Plataformas**, selecione **Adicionar plataforma**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-131">Under **Platforms**, select **Add platform**.</span></span>
5. <span data-ttu-id="f4f9b-132">Selecione **Plataforma nativa**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-132">Select **Native platform**.</span></span>
6. <span data-ttu-id="f4f9b-p105">Copie a ID de Cliente para a área de transferência. Você precisará inserir esse valor no exemplo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-p105">Copy the Client Id to the clipboard. You'll need to enter this value into the sample app.</span></span>

    <span data-ttu-id="f4f9b-135">Essa ID de aplicativo é o identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-135">The app id is a unique identifier for your app.</span></span> 

7. <span data-ttu-id="f4f9b-136">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-136">Select **Save**.</span></span>

## <a name="importing-the-project-dependencies"></a><span data-ttu-id="f4f9b-137">Importando as dependências do projeto</span><span class="sxs-lookup"><span data-stu-id="f4f9b-137">Importing the project dependencies</span></span>

1. <span data-ttu-id="f4f9b-138">Clone este repositório, [Exemplo de conexão com o Office 365 para iOS usando o SDK do Microsoft Graph](https://github.com/microsoftgraph/ios-swift-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="f4f9b-138">Clone this repository, [Office 365 Connect Sample for iOS Using the Microsoft Graph SDK](https://github.com/microsoftgraph/ios-swift-connect-rest-sample).</span></span> 


2. <span data-ttu-id="f4f9b-139">Use o CocoaPods para importar as dependências do PromiseKit.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-139">Use CocoaPods to import the PromiseKit dependencies.</span></span> <span data-ttu-id="f4f9b-140">Este aplicativo de exemplo já contém um podfile que colocará os pods no projeto.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-140">This sample app already contains a podfile that will get the pods into the project.</span></span> <span data-ttu-id="f4f9b-141">Navegue até a pasta raiz do projeto no aplicativo **Terminal** e, do **Terminal**, execute:</span><span class="sxs-lookup"><span data-stu-id="f4f9b-141">Navigate to the root folder of the project in the **Terminal** app, and from **Terminal** run:</span></span>

        pod install

   <span data-ttu-id="f4f9b-p107">Você receberá a confirmação de que os pods foram importados para o projeto. Para saber mais, consulte [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html).</span><span class="sxs-lookup"><span data-stu-id="f4f9b-p107">You will receive confirmation that the pods have been imported into the project. For more information, see [CocoaPods](https://guides.cocoapods.org/using/using-cocoapods.html)</span></span>

## <a name="install-the-msal-authentication-framework"></a><span data-ttu-id="f4f9b-144">Instalar a estrutura de autenticação da MSAL</span><span class="sxs-lookup"><span data-stu-id="f4f9b-144">Install the MSAL authentication framework</span></span>

<span data-ttu-id="f4f9b-145">A versão de visualização da MSAL é distribuída como arquivos de cabeçalho e símbolos usando o Carthage.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-145">The preview version of MSAL is distributed as header and symbol files using Carthage.</span></span> <span data-ttu-id="f4f9b-146">Para instalar a MSAL no projeto, siga estas etapas:</span><span class="sxs-lookup"><span data-stu-id="f4f9b-146">To install MSAL in the project, do these steps:</span></span>

1. <span data-ttu-id="f4f9b-147">Abra o terminal Bash e vá para a pasta raiz do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-147">Open the Bash terminal and go to the app root folder.</span></span>
2. <span data-ttu-id="f4f9b-148">Crie um **cartfile**: copie `echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile` para o terminal e execute o comando.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-148">Create a **cartfile**: Copy `echo "github \"AzureAD/microsoft-authentication-library-for-objc\" \"master\"" > Cartfile`  into the terminal and run the command.</span></span>
3. <span data-ttu-id="f4f9b-149">Compile a biblioteca MSAL: copie `carthage update` para o terminal e execute o comando.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-149">Build the MSAL library: Copy `carthage update` into the terminal and run the command.</span></span>


## <a name="enable-keychain-sharing"></a><span data-ttu-id="f4f9b-150">Habilitar o compartilhamento de chaves</span><span class="sxs-lookup"><span data-stu-id="f4f9b-150">Enable keychain sharing</span></span>
 
<span data-ttu-id="f4f9b-p109">Para o Xcode8, você deve adicionar o grupo de chaves para que o aplicativo não falhe ao acessar a chave. Para adicionar o grupo de chaves:</span><span class="sxs-lookup"><span data-stu-id="f4f9b-p109">For Xcode8, you need to add the keychain group or your app will fail to access keychain. To add the keychain group:</span></span>
 
1. <span data-ttu-id="f4f9b-153">Escolha o projeto, no painel de gerenciamento de projetos do Xcode.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-153">Select the project on the project manager panel in XCode.</span></span> <span data-ttu-id="f4f9b-154">(⌘ + 1).</span><span class="sxs-lookup"><span data-stu-id="f4f9b-154">(⌘ + 1).</span></span>
 
2. <span data-ttu-id="f4f9b-155">Selecione o destino **O365-iOS-Microsoft-Graph-Connect-swift**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-155">Select the **O365-iOS-Microsoft-Graph-Connect-swift** target.</span></span>

3. <span data-ttu-id="f4f9b-156">Na guia **Geral** e na seção **Entrar**, verifique se a opção **Gerenciar entrada automaticamente** está marcada e se você tem um certificado de autenticação válido.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-156">On the **General** tab and **Signing** section, verify that **Automatically manage signing** is checked and you have a valid signing certificate.</span></span>
 
3. <span data-ttu-id="f4f9b-157">Na guia **Recursos**, habilite o **Compartilhamento de chaves**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-157">On the **Capabilities** tab, enable **Keychain Sharing**.</span></span>
 
4. <span data-ttu-id="f4f9b-158">Se **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** não estiver na lista de grupos de chaves, adicione-o.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-158">If **com.microsoft.O365-iOS-Microsoft-Graph-Connect-Swift-REST** is not in the list of Keychain Groups, add it.</span></span>

## <a name="authenticating-with-microsoft-graph"></a><span data-ttu-id="f4f9b-159">Autenticação com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f4f9b-159">Authenticating with Microsoft Graph</span></span>

<span data-ttu-id="f4f9b-160">O fluxo de trabalho da interface do usuário é o seguinte: o aplicativo solicita que o usuário se autentique.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-160">The UI workflow is as follows: The app asks the user to authenticate.</span></span> <span data-ttu-id="f4f9b-161">Depois da autenticação, o usuário pode enviar um email para outro usuário.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-161">After authentication, the user can send a mail to another user.</span></span> <span data-ttu-id="f4f9b-162">Para realizar solicitações para o Microsoft Graph, o exemplo usa a biblioteca de autenticação **MSAL** para autenticar solicitações HTTPS com um token de portador OAuth 2.0 apropriado.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-162">To make requests against Microsoft Graph, the sample uses the **MSAL** authentication library to authenticate HTTPS requests with an appropriate OAuth 2.0 bearer token.</span></span> <span data-ttu-id="f4f9b-163">No exemplo de projeto, a classe é **AuthenticationClass.swift**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-163">In the sample project the **AuthenticationClass.swift.**</span></span> <span data-ttu-id="f4f9b-164">A classe importa a biblioteca **MSAL** e adquire o token de acesso necessário para operações REST do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-164">class imports the **MSAL** library and acquires the access token needed for Microsoft Graph REST operations.</span></span>

1. <span data-ttu-id="f4f9b-165">Abra o espaço de trabalho do projeto **Xcode** (**Graph-iOS-Swift-Connect.xcworkspace**) e abra o arquivo da classe **AuthenticationClass.swift**. Encontre o código a seguir nessa classe.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-165">Open the **XCode** project workspace (**Graph-iOS-Swift-Connect.xcworkspace**), and open the class file **AuthenticationClass.swift** Find the following code in that class.</span></span>


  ```swift
     /**
     Authenticates to Microsoft Graph.
     If a user has previously signed in before and not disconnected, silent log in
     will take place.
     If not, authentication will ask for credentials
     */
    func connectToGraph(scopes: [String],
                        completion:@escaping (_ error: ApplicationConstants.MSGraphError?, _ accessToken: String) -> Bool)  {
        do {
            if let initError = self.lastInitError {
                if initError.lengthOfBytes(using: String.Encoding.ascii) > 1 {
                    throw NSError.init(domain: initError, code: 0, userInfo: nil)
                }
            }
            // We check to see if we have a current logged in user. If we don't, then we need to sign someone in.
            // We throw an interactionRequired so that we trigger the interactive signin.
            if  try authenticationProvider.users().isEmpty {
                throw NSError.init(domain: "MSALErrorDomain", code: MSALErrorCode.interactionRequired.rawValue, userInfo: nil)
            } else {
                // Acquire a token for an existing user silently
                try authenticationProvider.acquireTokenSilent(forScopes: scopes, user: authenticationProvider.users().first) { (result, error) in
                    if error == nil {
                        self.accessToken = (result?.accessToken)!
                        _ = completion(nil, self.accessToken);
                    } else {
                        //"Could not acquire token silently: \(error ?? "No error information" as! Error )"
                       var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error! as NSError), "");
                    }
                }
            }
        }  catch let error as NSError {
            // interactionRequired means we need to ask the user to sign-in. This usually happens
            // when the user's Refresh Token is expired or if the user has changed their password
            // among other possible reasons.
            if error.code == MSALErrorCode.interactionRequired.rawValue {
                authenticationProvider.acquireToken(forScopes: scopes) { (result, error) in
                    if error == nil {
                        self.accessToken = (result?.accessToken)!
                        var _ = completion(nil, self.accessToken);
                    } else  {
                        var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error! as NSError), "");
                    }
                }
            } else {
                var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error as NSError), error.localizedDescription);

            }
        } catch {
            // This is the catch all error.
            var _ = completion(ApplicationConstants.MSGraphError.nsErrorType(error: error as NSError), error.localizedDescription);
        }
    }

  ```


2. <span data-ttu-id="f4f9b-166">Chamaremos a função **connectToGraph** de **ConnectViewController.swift**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-166">We'll call the **connectToGraph** function from **ConnectViewController.swift**.</span></span> <span data-ttu-id="f4f9b-167">Esse controlador é a exibição padrão que o aplicativo carrega com um único botão chamado **Conectar**, no qual o usuário tocará para iniciar a autenticação.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-167">This controller is the default view that the app loads with a single button named **Connect** that the user taps to start authenticating.</span></span> 

  ```swift
// MARK: Authentication
private extension ConnectViewController {
    func authenticate() {
        loadingUI(show: true)
        let scopes = ApplicationConstants.kScopes
        AuthenticationClass.sharedInstance?.connectToGraph( scopes: scopes) {
            (result: ApplicationConstants.MSGraphError?, accessToken: String) -> Bool  in
            defer {self.loadingUI(show: false)}
            if let graphError = result {
                switch graphError {
                case .nsErrorType(let nsError):
                    print(NSLocalizedString("ERROR", comment: ""), nsError.userInfo)
                    self.showError(message: NSLocalizedString("CHECK_LOG_ERROR", comment: ""))
                }
                return false
            }
            else {
                // run on main thread!!
                DispatchQueue.main.async {
                    self.performSegue(withIdentifier: "sendMail", sender: nil)
                }
                return true
            }
        }
    }
}

  ```

## <a name="send-an-email-with-microsoft-graph"></a><span data-ttu-id="f4f9b-168">Enviar um email com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f4f9b-168">Send an email with Microsoft Graph</span></span>

<span data-ttu-id="f4f9b-169">Depois de conectar o usuário ao Microsoft Graph, o exemplo obtém o endereço de email, o nome de exibição e a foto de perfil do usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-169">After connecting the user to Microsoft Graph, the sample gets the authenticated user's email address, display name, and profile photo.</span></span> <span data-ttu-id="f4f9b-170">O exemplo carrega a foto de perfil na pasta raiz do OneDrive do usuário e solicita ao OneDrive a URL de compartilhamento da imagem.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-170">The sample uploads the profile photo to the user's OneDrive root folder and asks OneDrive for the sharing Url of the picture.</span></span> <span data-ttu-id="f4f9b-171">Por fim, o exemplo posta uma solicitação REST no Microsoft Graph para enviar uma mensagem de email ao endereço de email fornecido.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-171">Finally, the sample posts a REST request to Microsoft Graph to send a mail message to the provided email address.</span></span> 

<span data-ttu-id="f4f9b-172">O corpo da mensagem contém o link de compartilhamento da imagem e a própria imagem como um arquivo de anexo.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-172">The message body contains the picture sharing link and the picture itself as an attached image file.</span></span> <span data-ttu-id="f4f9b-173">O destinatário padrão é o usuário autenticado, mas o exemplo permite ao usuário fornecer o endereço de email de qualquer outro usuário.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-173">The default recipient is the authenticated user, but the sample allows the user to provide the email address of any other user.</span></span> 

<span data-ttu-id="f4f9b-174">O código com o qual trabalharemos aqui está na classe **SendMailViewController_WithPromise.swift**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-174">The code we'll work with here is in the class **SendMailViewController_WithPromise.swift.**</span></span> <span data-ttu-id="f4f9b-175">A função `viewDidLoad()` lê o valor `self.emailTextField.text` para obter o endereço de email do destinatário e, em seguida, inicia uma **cadeia de promessas** para obter a imagem de perfil do usuário autenticado.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-175">The `viewDidLoad()` function reads the `self.emailTextField.text` value to get the mail recipient's email address and then starts a **promise chain** to get the authenticated user's profile picture.</span></span> <span data-ttu-id="f4f9b-176">Se a promessa for rejeitada, `sendMailButton` não é habilitado.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-176">If the promise is rejected, the `sendMailButton` is not enabled.</span></span>

1. <span data-ttu-id="f4f9b-177">Abra **SendMailViewController_WithPromise.swift.**</span><span class="sxs-lookup"><span data-stu-id="f4f9b-177">Open **SendMailViewController_WithPromise.swift.**</span></span> <span data-ttu-id="f4f9b-178">e encontre a função `viewDidLoad`.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-178">and find the `viewDidLoad` function.</span></span> <span data-ttu-id="f4f9b-179">A função `self.userPictureWork` é chamada para iniciar a cadeia de promessas.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-179">The `self.userPictureWork` function is called to start the promise chain.</span></span>

   ```swift
    override func viewDidLoad() {
        super.viewDidLoad()
        //Get user state values before creating mail message to be sent
        do
        {
            try self.userName = AuthenticationClass.sharedInstance?.authenticationProvider.users()[0].name!
            try self.emailTextField.text = AuthenticationClass.sharedInstance?.authenticationProvider.users()[0].displayableId
            self.userEmailAddress = self.emailTextField.text
            self.headerLabel.text = "Hi, \(self.userName! )"
            
            updateUI(showActivityIndicator: true, statusText: "Getting picture", sendMail: true)

            //Important: Break out of async promise chain by declaring result returns Void
            _ = self.userPictureWork().then{
                result -> Void in
                    self.userPictureUrl = (result[1] as! String)
                    self.userProfilePicture = (result[0] as! UIImage)
                    self.updateUI(showActivityIndicator: false, statusText: "", sendMail: true)

            }.catch{err -> Void  in
                self.updateUI(showActivityIndicator: false, statusText: "", sendMail: false)

            }
        } catch _ as NSError{
            self.updateUI(showActivityIndicator: false,
                          statusText: "Error getting user profile picture.", sendMail: false)
        }
    }
  
   ```

   

1. <span data-ttu-id="f4f9b-180">Encontre a função para ajudar na criação de solicitação de email na classe:</span><span class="sxs-lookup"><span data-stu-id="f4f9b-180">Find the mail request creation helper function in the class:</span></span>

   ```swift
    /**
     Prepare mail content by loading the JSON request payload template and HTML message body template from resources and replacing placeholders in the templates with appropriate values.
     */
    func mailContent() -> Data? {
        if let emailFilePath = Bundle.main.path(forResource: "EmailPostContent", ofType: "json"),
            let emailBodyFilePath = Bundle.main.path(forResource: "EmailBody", ofType: "html")
        {
            do {
                // Prepare upload content
                let emailContent = try String(contentsOfFile: emailFilePath, encoding: String.Encoding.utf8)
                let emailBodyRaw = try String(contentsOfFile: emailBodyFilePath, encoding: String.Encoding.utf8)
                // Request doesn't accept a single quotation mark("), so change it to the acceptable form (\")
                var emailValidBody: String;
                emailValidBody = emailBodyRaw.replacingOccurrences(of: "\"", with: "\\\"")
                emailValidBody = emailValidBody.replacingOccurrences(of: "a href=%s", with: ("a href=" + self.userPictureUrl!))
                let imageData: NSData = UIImagePNGRepresentation(self.userProfilePicture!)! as NSData;
                let emailPostContent = emailContent.replacingOccurrences(of: "<EMAIL>", with: self.emailTextField.text!)
                    .replacingOccurrences(of: "<CONTENTTYPE>", with: "HTML")
                    .replacingOccurrences(of: "<CONTENT>", with: emailValidBody)
                    .replacingOccurrences(of: "<ODATA.TYPE>", with: "#microsoft.graph.fileAttachment")
                    .replacingOccurrences(of: "<IMAGE.TYPE>", with: "image\\/png")
                    .replacingOccurrences(of: "<CONTENTBYTES>", with: imageData.base64EncodedString())
                    .replacingOccurrences(of: "<NAME>", with: "me.png")
                // Return JSON payload with mail body as HTML string and attached picture as a file attachment of type NSData
                return emailPostContent.data(using: String.Encoding.utf8)
            }
            catch {
                // Error handling in case file loading fails.
                return nil
            }
        }
        // Error handling in case files aren't present.
        return nil
    }

   ```
2. <span data-ttu-id="f4f9b-181">Encontre as seguintes funções de ajuda para obter a imagem de perfil do usuário, carregar a foto no OneDrive e solicitar um link de compartilhamento para a imagem:</span><span class="sxs-lookup"><span data-stu-id="f4f9b-181">Find the following helper functions for getting the user's profile picture,  uploading the photograph to OneDrive, and requesting a sharing link for the picture:</span></span>

   ```swift
    /**
      Async func. Get user's profile photo, upload photo to OneDrive, and get sharing link
     - returns:
        Promise<UIImage>. The user's profile picture
     */
    func getUserPicture()->Promise<UIImage?>{
        return Promise{ fulfill, reject in
            let urlRequest = self.buildRequest(operation: "GET", resource: "photo/$value") as URLRequest
            let task = URLSession.shared.dataTask(with:urlRequest){ data , res , err in
                if let err:Error = err {
                    print(err.localizedDescription)
                    return reject(err)
                }
                if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                    return fulfill(self.getDefaultPicture())
                }
                if let data = data {
                    if let userImage: UIImage = UIImage(data:data) {
                        self.userProfilePicture = userImage
                        return fulfill(userImage)
                    } else {
                        return reject("no image" as! Error)
                    }
                } else {
                    return fulfill(self.getDefaultPicture())
                }
            }
            task.resume()
        }
    }
    
    /**
     Async func. Uploads a UIImage object to the signed in user's OneDrive root folder
     - Returns:
        A Promise encapsulating an array of AnyObject. Element 0 contains the user profile photo obtained in the previous chained async call
        Element 1 contains the web sharing URL of the photo in OneDrive as a String
     - Parameters:
     - UIImage: The image to upload to OneDrive
     */
    func uploadPicture(photo: UIImage) -> Promise<[AnyObject]> {
        return Promise<[AnyObject]>{ fulfill, reject in
            let uploadRequestUrl = self.buildRequest(operation: "PUT", resource: "drive/root:/me.jpg:/content", content: UIImageJPEGRepresentation(photo, 1.0)!) as URLRequest
            let task = URLSession.shared.dataTask(with:uploadRequestUrl){ data, res, err in
                if let err = err{
                    return reject(err)
                }
                if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                    return reject(HTTPError.InvalidRequest)
                }
                //data can be serialized to a DriveItem object
                //https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/driveitem
                var itemId: String = "";
                if let responseContent = data {
                    itemId = self.getValueFromResponse(json: responseContent, key: "id" )
                    var returnValues = [AnyObject]();
                    returnValues.append(photo as AnyObject)
                    returnValues.append(itemId as AnyObject)
                    return fulfill(returnValues)
                }
            }
            task.resume()
        }
    }

    /**
     Async func. Requests a new sharing link for the OneDrive item specified by the item id.
     - returns:
     - Promise<String: AnyObject>. The new sharing link and the image wrapped in a Promise
     */
    func createSharingLink(itemId: String, image: UIImage) ->Promise<[AnyObject]>{
        return Promise<[AnyObject]>{ fulfill, reject in
            //Create Data object for the JSON payload
            if let sharingLinkFilePath = Bundle.main.path(forResource: "CreateSharingLink", ofType: "json")
            {
                do {
                    let sharingLinkcontent = try String(contentsOfFile: sharingLinkFilePath, encoding: String.Encoding.utf8)
                    let jsonPayload: Data = sharingLinkcontent.data(using: String.Encoding.utf8)!
                    let uploadRequestUrl = self.buildRequest(
                        operation: "POST", resource: "drive/items/"+itemId+"/createLink", content: jsonPayload) as URLRequest
                    let task = URLSession.shared.dataTask(with:uploadRequestUrl){ data, res, err in
                        if let err = err{
                            return reject(err)
                        }
                        if ((self.checkResult(result: res!)) != HTTPError.NoError) {
                            return reject(HTTPError.InvalidRequest)
                        }
                        //data can be serialized to a DriveItem object
                        //https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/driveitem
                        var sharingLink: String = "";
                        if let responseContent = data {
                            do {
                                let resultJson = try JSONSerialization.jsonObject(
                                    with: responseContent, options: []) as? [String:AnyObject]
                                sharingLink = (OneDriveFileLink.init(json:resultJson!)?.webUrl)!

                            } catch let error as NSError {
                                print(error)
                            }
                            var returnValues = [AnyObject]();
                            returnValues.append(image as AnyObject)
                            returnValues.append(sharingLink as AnyObject)
                            return fulfill(returnValues)
                        }
                    }
                    task.resume()

                }
            }
        }
   ```

3. <span data-ttu-id="f4f9b-182">Encontre a seguinte função de envio de email na classe.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-182">Find the following send mail function in the class.</span></span>  
 
   ```swift
    /**
     POSTS a new message to the sendmail resource
     - parameters:
        - Data: The body of the message
     */
    func sendMailRESTWithContent(_ content: Data) {
        let _ = self.sendCRUDMessage(resource: "microsoft.graph.sendmail",
                                     operation: "POST",
                                     content: content)
    }
    
    /**
     Send a create, read, update, delete (CRUD) message.
     Create= POST, Update= PUT, Delete= DELETE.
     Read= GET. Use sendGETMessage(resource: String) to read Graph contents
     - returns:
     JSON response as Data
     - parameters:
        - String: The REST resource receiving the CRUD request
        - String: the REST operation requested
        - Data: The json (as Data) representing the values to update
     */
    func sendCRUDMessage(resource: String, operation:String, content: Data)->Data  {
        var returnData: Data;
        returnData = Data.init();
        if  (self.connectToGraph()){
            if (operation == "GET") {
                return self.sendGETMessage(resource: resource)
            }
            let request = self.buildRequest(operation: operation, resource: resource, content:content);
            let task = URLSession.shared.dataTask(with:request as URLRequest, completionHandler:{ data, res, err in
                if let err = err{
                    self.updateUI(showActivityIndicator: false,
                             statusText: "Error assembling the mail content." + err.localizedDescription, sendMail: false)
                }
                let nttpError = self.checkResult(result: res!)
                if (nttpError != HTTPError.NoError) {
                    self.updateUI(showActivityIndicator: false,
                                  statusText: "Error sending the mail.", sendMail: false)
                }
                else {
                    self.updateUI(showActivityIndicator: false, statusText: "", sendMail: true)
                }
            }) // let task
             task.resume()
        }
        return returnData;
    }

   ```


## <a name="run-the-app"></a><span data-ttu-id="f4f9b-183">Executar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4f9b-183">Run the app</span></span>
1. <span data-ttu-id="f4f9b-184">Antes de executar o exemplo, será necessário fornecer a identificação do cliente que você recebeu do processo de registro na seção **Registrar o aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-184">Before running the sample you'll need to supply the client ID you received from the registration process in the section **Register the app.**</span></span> <span data-ttu-id="f4f9b-185">Abra **Info.plist** como código-fonte.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-185">Open **Info.plist** as source code.</span></span> 

   - <span data-ttu-id="f4f9b-186">Substitua `ENTER_CLIENT_ID_HERE` pela **ClientID** do processo de registro.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-186">Replace  `ENTER_CLIENT_ID_HERE` with the **ClientID** from the registration process.</span></span> <span data-ttu-id="f4f9b-187">Certifique-se de que `msal` não seja substituído.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-187">Be sure that `msal` is not replaced.</span></span> <span data-ttu-id="f4f9b-188">Depois de substituir a cadeia de caracteres, o valor da cadeia de caracteres da matriz se parecerá com `msal48d31887-5fad-4d73-a9f5-3c356e68a038`, onde a parte da GUID é a **sua** ID de cliente:</span><span class="sxs-lookup"><span data-stu-id="f4f9b-188">After you replace the string, the array string value looks like `msal48d31887-5fad-4d73-a9f5-3c356e68a038` where the GUID portion is **your** client Id:</span></span>  

   <span data-ttu-id="f4f9b-189">Por exemplo,</span><span class="sxs-lookup"><span data-stu-id="f4f9b-189">For example,</span></span> 

  ```xml
    <key>CFBundleURLTypes</key>
    <array>
        <dict>
            <key>CFBundleTypeRole</key>
            <string>Editor</string>
            <key>CFBundleURLName</key>
            <string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
            <key>CFBundleURLSchemes</key>
            <array>
                <string>msalENTER_CLIENT_ID_HERE</string>
                <string>auth</string>
            </array>
        </dict>
    </array>
  ```

     <span data-ttu-id="f4f9b-190">se tornará...</span><span class="sxs-lookup"><span data-stu-id="f4f9b-190">becomes...</span></span> 

  ```xml
    <key>CFBundleURLTypes</key>
    <array>
        <dict>
            <key>CFBundleTypeRole</key>
            <string>Editor</string>
            <key>CFBundleURLName</key>
            <string>$(PRODUCT_BUNDLE_IDENTIFIER)</string>
            <key>CFBundleURLSchemes</key>
            <array>
                <string>msal48d31887-5fad-4d73-a9f5-3c356e68a038</string>
                <string>auth</string>
            </array>
        </dict>
    </array>
  ```

> <span data-ttu-id="f4f9b-191">**Observação:** os escopos de permissão a seguir foram configurados para esse projeto: `["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]` .</span><span class="sxs-lookup"><span data-stu-id="f4f9b-191">**Note:** You'll notice that the following permission scopes have been configured for this project: `["https://graph.microsoft.com/Mail.ReadWrite","https://graph.microsoft.com/Mail.Send","https://graph.microsoft.com/Files.ReadWrite","https://graph.microsoft.com/User.ReadBasic.All"]` .</span></span> <span data-ttu-id="f4f9b-192">As chamadas de serviço usadas neste projeto, o envio de emails para sua conta de email e a recuperação de algumas informações de perfil (nome de exibição e endereço de email), além da gravação na pasta raiz do OneDrive do usuário, exigem essas permissões para que o aplicativo seja executado sem erros de permissão.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-192">The service calls used in this project, sending a mail to your mail account and retrieving some profile information (Display Name, Email Address), and writing to the user's OneDrive root require these permissions for the app to run without a permissions error.</span></span>

2. <span data-ttu-id="f4f9b-193">Execute o exemplo, toque em **Conectar**, entre com sua conta pessoal, corporativa ou de estudante e conceda as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-193">Run the sample, tap **Connect,** sign in with your personal or work or school account, and grant the requested permissions.</span></span>

3. <span data-ttu-id="f4f9b-p120">Escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão.</span><span class="sxs-lookup"><span data-stu-id="f4f9b-p120">Choose the **Send email** button. When the mail is sent, a success message is displayed below the button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f4f9b-196">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f4f9b-196">Next steps</span></span>
- <span data-ttu-id="f4f9b-197">Experimente a API REST usando o [Explorador do Graph](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="f4f9b-197">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="f4f9b-198">Encontre exemplos de operações comuns para SDK no [Exemplo de trechos de código do iOS Objective C do Microsoft Graph](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span><span class="sxs-lookup"><span data-stu-id="f4f9b-198">Find examples of common operations for SDK operations in the [Microsoft Graph iOS Objective C Snippets Sample](https://github.com/microsoftgraph/ios-objectiveC-snippets-sample).</span></span>

## <a name="see-also"></a><span data-ttu-id="f4f9b-199">Confira também</span><span class="sxs-lookup"><span data-stu-id="f4f9b-199">See also</span></span>
- [<span data-ttu-id="f4f9b-200">Protocolos do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="f4f9b-200">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="f4f9b-201">Tokens do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="f4f9b-201">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
