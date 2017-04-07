# <a name="get-started-with-microsoft-graph-in-a-universal-windows-10-app"></a>Introdução ao Microsoft Graph em um aplicativo universal do Windows 10

> **Criando aplicativos para clientes corporativos?** O aplicativo pode não funcionar caso o cliente corporativo habilite os recursos Enterprise Mobility + Security, como <a href="https://azure.microsoft.com/en-us/documentation/articles/active-directory-conditional-access-device-policies/" target="_newtab">acesso condicional ao dispositivo</a>. Nesse caso, pode ser que você não esteja ciente e seu cliente pode enfrentar problemas de erro. 

> Para fornecer suporte a **todos os clientes corporativos**, em **todos os cenários corporativos**, use o ponto de extremidade do Microsoft Azure AD e gerencie os aplicativos usando o [Portal de Gerenciamento do Microsoft Azure](https://aka.ms/aadapplist). Para saber mais, confira o tópico [Decidindo entre os pontos de extremidade do Azure AD e do Azure AD v2.0](../authorization/auth_overview.md#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints).

Este artigo descreve as tarefas obrigatórias para obter um token de acesso do [ponto de extremidade do Azure AD v2.0](https://developer.microsoft.com/en-us/graph/docs/authorization/converged_auth) e chamar o Microsoft Graph. Ele o orientará por meio do código dentro de exemplos de [conexão usando o Microsoft Graph para UWP (REST)](https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample) e [conexão usando o Microsoft Graph para UWP (biblioteca)](https://github.com/microsoftgraph/uwp-csharp-connect-sample) para explicar os principais conceitos que você tem que implementar em um aplicativo que usa o Microsoft Graph. O artigo também descreve como acessar o Microsoft Graph, usando chamadas REST não processadas e a [Biblioteca de cliente do Microsoft Graph](http://www.nuget.org/packages/Microsoft.Graph/).

Você pode baixar as duas versões do aplicativo que você criará nesta explicação desses repositórios do GitHub:

* [Exemplo de conexão com o Microsoft Graph para UWP (REST)](https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample)
* [Exemplo de conexão com o Microsoft Graph para UWP (biblioteca)](https://github.com/microsoftgraph/uwp-csharp-connect-sample)

**Não está com vontade de criar um aplicativo?** Use o [Início rápido do Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) para começar a usar rapidamente.

## <a name="sample-user-interface"></a>Exemplo de interface do usuário

O exemplo contém uma interface do usuário muito simples, que consiste em uma barra de comando superior, um botão **Conectar**, um botão **Enviar email** e uma caixa de texto que é preenchida automaticamente com o endereço de email do usuário conectado, mas que pode ser editada.

O botão **Enviar email** é desabilitado quando o usuário não está conectado:

![Tela mostrando o botão Conectar habilitado e o botão Enviar email desabilitado](images/SignedOut.png)

A barra de comando superior contém um botão Desconectar quando o usuário está conectado:

![Tela mostrando o endereço de email do usuário conectado e o botão Enviar email habilitado](images/SignedIn.png)

Todas as cadeias de caracteres de interface do usuário do exemplo são armazenadas no arquivo Resources.resw dentro da pasta Ativos.

## <a name="prerequisites"></a>Pré-requisitos

Para começar, será necessário: 

- Uma [conta da Microsoft](https://www.outlook.com/) ou uma [conta corporativa ou de estudante](http://dev.office.com/devprogram)
- Visual Studio 2015 
- O [Projeto inicial do Microsoft Graph para UWP (biblioteca)](https://github.com/microsoftgraph/uwp-csharp-connect-sample/tree/master/starter) ou [Projeto inicial do Microsoft Graph para UWP (REST)](https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/master/starter). Ambos os modelos contêm classes vazias às quais você adicionará código. Ele também contém cadeias de recursos. Para obter um ou ambos os projetos, clone ou baixe o [Exemplo de conexão com o Microsoft Graph para UWP (biblioteca)](https://github.com/microsoftgraph/uwp-csharp-connect-sample) e/ou [Exemplo de conexão com o Microsoft Graph para UWP (REST)](https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample) e, em seguida, abra a solução dentro da pasta **starter**.


## <a name="register-the-app"></a>Registrar o aplicativo
 
1. Entre no [Portal de Registro do Aplicativo](https://apps.dev.microsoft.com/) usando sua conta pessoal ou sua conta corporativa ou de estudante.
2. Selecione **Adicionar um aplicativo**.
3. Insira um nome para o aplicativo e selecione **Criar aplicativo**.
    
    A página de registro é exibida, listando as propriedades do seu aplicativo.
 
4. Em **Plataformas**, selecione **Adicionar plataforma**.
5. Selecione **Plataforma móvel**.
6. Copie a ID de cliente (ID de aplicativo) e os valores do URI de redirecionamento para a área de transferência. Você precisará inserir esses valores no exemplo de aplicativo.

    Essa ID de aplicativo é o identificador exclusivo do aplicativo. Um URI de redirecionamento é um URI exclusivo fornecido pelo Windows 10 para cada aplicativo para garantir que as mensagens enviadas para esse URI sejam enviadas somente para esse aplicativo. 

7. Selecione **Salvar**.

## <a name="configure-the-project"></a>Configurar o projeto

1. Abra o arquivo de solução para o projeto inicial no Visual Studio.
2. Abra o arquivo **App.xaml** do projeto e localize o nó `Application.Resources`. Substitua a ID do aplicativo e redirecione espaços reservados do URI com os valores correspondentes do aplicativo que você registrou.


```xml
    <Application.Resources>
        <!-- Add your Client Id here. -->
        <x:String x:Key="ida:ClientID">ENTER_YOUR_CLIENT_ID</x:String>
        <!-- Add your Redirect URI here. -->
        <x:String x:Key="ida:ReturnUrl">ENTER_YOUR_REDIRECT_URI</x:String>
    </Application.Resources>
```

## <a name="install-the-microsoft-authentication-library-msal"></a>Instale a Biblioteca de Autenticação da Microsoft (MSAL)

A [Biblioteca de Autenticação da Microsoft](https://www.nuget.org/packages/Microsoft.Identity.Client) contém classes e métodos que facilitam a autenticação de usuários através do ponto de extremidade do Azure AD v2.0.

1. No Gerenciador de soluções, clique com botão direito no nome do projeto e selecione **Gerenciar pacotes NuGet...**
2. Clique em Procurar e pesquise Microsoft.Identity.Client.
3. Selecione a versão mais recente da Biblioteca de Autenticação da Microsoft e clique em **Instalar**.

## <a name="install-the-microsoft-graph-client-library"></a>Instalar a Biblioteca de Cliente do Microsoft Graph

> **Observação** Se você vai usar chamadas REST não processadas para acessar o Microsoft Graph, ignore esta seção.

1. No Gerenciador de Soluções, clique com botão direito no nome do projeto e selecione **Gerenciar pacotes NuGet...**
2. Clique em Procurar e pesquise Microsoft.Graph.
3. Selecione a versão mais recente da Biblioteca de Cliente do Microsoft Graph e clique em **Instalar**.

## <a name="create-the-authenticationhelpercs-class"></a>Criar a classe AuthenticationHelper.cs

Abra o arquivo AuthenticationHelper.cs no projeto inicial. Este arquivo contém todo o código de autenticação, juntamente com a lógica adicional que armazena informações do usuário e força a autenticação somente quando o usuário se desconecta do aplicativo. Essa classe contém pelo menos dois métodos: `GetTokenForUserAsync` e `Signout`. Se você estiver usando a Biblioteca de Cliente do Microsoft Graph, precisará adicionar um terceiro método: `GetAuthenticatedClient`.

O método ``GetTokenHelperAsync`` é executado quando o usuário autentica e toda vez que o aplicativo faz uma chamada ao Microsoft Graph depois disso.

**Usando declarações**

***Versão de biblioteca de cliente***

Se você estiver usando a Biblioteca de Cliente do Microsoft Graph, precisará dessas declarações:

```c#
using System;
using System.Diagnostics;
using System.Net.Http.Headers;
using System.Threading.Tasks;
using Microsoft.Graph;
using Microsoft.Identity.Client;
```

***Versão REST***

Se você estiver usando chamadas REST não processadas para acessar o Microsoft Graph, precisará dessas declarações `using` na classe AuthenticationHelper:

```c#
using System;
using System.Threading.Tasks;
using Windows.Storage;
using Microsoft.Identity.Client;
```

**Campos de classe**

As duas versões da classe AuthenticationHelper precisarão desses campos:

```c#
// The Client ID is used by the application to uniquely identify itself to the Azure AD v2.0 endpoint.
static string clientId = App.Current.Resources["ida:ClientID"].ToString();
public static string[] Scopes = { "User.Read", "Mail.Send" };
public static PublicClientApplication IdentityClientApp = new PublicClientApplication(clientId);
public static string TokenForUser = null;
public static DateTimeOffset Expiration;
```

Observe que ambas as versões usam a classe `PublicClientApplication` do MSAL para autenticar o usuário. O campo `Scopes` armazena os escopos de permissão do Microsoft Graph que o aplicativo precisará solicitar quando o usuário autenticar. 

***Versão de biblioteca de cliente***

Se você estiver usando a biblioteca de cliente, armazene o `GraphServicesClient` como um campo para que você tenha que construí-lo apenas uma vez:

```c#
private static GraphServiceClient graphClient = null;
```

***Versão REST***

Se você estiver usando chamadas REST, precisará armazenar alguns valores nas configurações de roaming do aplicativo, porque precisará armazenar informações sobre o usuário. A biblioteca de cliente fornece estas informações na outra versão.

```c#
public static ApplicationDataContainer _settings = ApplicationData.Current.RoamingSettings;
```

**GetTokenForUserAsync**

***Versão de biblioteca de cliente***

O método `GetTokenForUserAsync` usa a configuração PublicClientApplicationClass e ClientId para obter acesso a um token para o usuário. Se o usuário ainda não autenticou, ele abre a interface de usuário da autenticação. Essa é a versão do método a ser usada se você estiver usando a biblioteca de cliente.

```c#
        public static async Task<string> GetTokenForUserAsync()
        {
            AuthenticationResult authResult;
            try
            {
                authResult = await IdentityClientApp.AcquireTokenSilentAsync(Scopes);
                TokenForUser = authResult.Token;
            }

            catch (Exception)
            {
                if (TokenForUser == null || Expiration <= DateTimeOffset.UtcNow.AddMinutes(5))
                {
                    authResult = await IdentityClientApp.AcquireTokenAsync(Scopes);

                    TokenForUser = authResult.Token;
                    Expiration = authResult.ExpiresOn;
                }
            }

            return TokenForUser;
        }
```

***Versão REST***

A versão REST do método `GetTokenForUserAsync` faz um pouco mais de trabalho, porque ela também precisa armazenar algumas informações sobre o usuário conectado.

```c#
        public static async Task<string> GetTokenForUserAsync()
        {
            AuthenticationResult authResult;
            try
            {
                authResult = await IdentityClientApp.AcquireTokenSilentAsync(Scopes);
                TokenForUser = authResult.Token;
                // save user ID in local storage
                _settings.Values["userID"] = authResult.User.UniqueId;
                _settings.Values["userEmail"] = authResult.User.DisplayableId;
                _settings.Values["userName"] = authResult.User.Name;
            }

            catch (Exception)
            {
                if (TokenForUser == null || Expiration <= DateTimeOffset.UtcNow.AddMinutes(5))
                {
                    authResult = await IdentityClientApp.AcquireTokenAsync(Scopes);

                    TokenForUser = authResult.Token;
                    Expiration = authResult.ExpiresOn;

                    // save user ID in local storage
                    _settings.Values["userID"] = authResult.User.UniqueId;
                    _settings.Values["userEmail"] = authResult.User.DisplayableId;
                    _settings.Values["userName"] = authResult.User.Name;
                }
            }

            return TokenForUser;
        }
```

**SignOut**

O método `Signout` em ambas as versões desconecta todos os usuários conectados através do `PublicClientApplication` (somente um usuário, neste caso) e anula o valor `TokenForUser`. A versão que usa a biblioteca de cliente também anula o `GraphServicesClient` armazenado, e a versão REST anula os valores armazenados nas configurações de roaming do aplicativo.

***Versão de biblioteca de cliente***

Esta é a versão da biblioteca do cliente do método `Signout`.

```c#
        public static void SignOut()
        {
            foreach (var user in IdentityClientApp.Users)
            {
                user.SignOut();
            }
            graphClient = null;
            TokenForUser = null;

        }
``` 

***Versão REST***

Esta é a versão REST do método `Signout`.

```c#
        public static void SignOut()
        {
            foreach (var user in IdentityClientApp.Users)
            {
                user.SignOut();
            }

            TokenForUser = null;

            //Clear stored values from last authentication.
            _settings.Values["userID"] = null;
            _settings.Values["userEmail"] = null;
            _settings.Values["userName"] = null;

        }
```

**GetAuthenticatedClient (somente para a biblioteca de cliente)**

Por fim, se você estiver usando a biblioteca de cliente, precisará de um método que cria um `GraphServicesClient`. Este método cria um cliente que usa o método `GetTokenForUserAsync` para cada chamada por meio do cliente para o Microsoft Graph.

```c#
        public static GraphServiceClient GetAuthenticatedClient()
        {
            if (graphClient == null)
            {
                // Create Microsoft Graph client.
                try
                {
                    graphClient = new GraphServiceClient(
                        "https://graph.microsoft.com/v1.0",
                        new DelegateAuthenticationProvider(
                            async (requestMessage) =>
                            {
                                var token = await GetTokenForUserAsync();
                                requestMessage.Headers.Authorization = new AuthenticationHeaderValue("bearer", token);
                            }));
                    return graphClient;
                }

                catch (Exception ex)
                {
                    Debug.WriteLine("Could not create a graph client: " + ex.Message);
                }
            }

            return graphClient;
        }
```

## <a name="send-an-email-with-microsoft-graph"></a>Enviar um email com o Microsoft Graph

Abra o arquivo MailHelper.cs em seu projeto inicial. Este arquivo contém o código que constrói e envia um email. Consiste em um único método -- ``ComposeAndSendMailAsync`` -- que constrói e envia uma solicitação POST para o ponto de extremidade **https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail**. 

O método ``ComposeAndSendMailAsync`` tem três valores de cadeia de caracteres, ou seja, ``subject``, ``bodyContent`` e ``recipients``, que são passados para ele pelo arquivo MainPage.xaml.cs. As cadeias de caracteres ``subject`` e ``bodyContent`` são armazenadas, juntamente com todos os outras cadeias de caracteres de interface do usuário, no arquivo Resources.resw. A cadeia de caracteres ``recipients`` vem da caixa de endereço na interface do aplicativo. 

**Versão REST**

A versão REST deste arquivo exige as seguintes declarações `using`:

```c#
using System;
using System.Threading.Tasks;
```

Já que o usuário pode passar mais de um endereço, a primeira tarefa é dividir a cadeia de caracteres ``recipients`` em uma coleção de objetos EmailAddress que podem ser passados no corpo POST da solicitação:

```c#
            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            string recipientsJSON = null;

            int n = 0;
            foreach (string recipient in splitRecipientsString)
            {
                if ( n==0)
                recipientsJSON += "{'EmailAddress':{'Address':'" + recipient.Trim() + "'}}";
                else
                {
                    recipientsJSON += ", {'EmailAddress':{'Address':'" + recipient.Trim() + "'}}";
                }
                n++;
            }
```

A segunda tarefa é construir um objeto de mensagem JSON válido e enviá-lo para o ponto de extremidade **me/microsoft.graph.SendMail** por meio de uma solicitação HTTP POST. Já que a cadeia de caracteres ``bodyContent`` é um documento HTML, a solicitação define o valor **ContentType** como HTML. Além disso, anote a chamada a ``AuthenticationHelper.GetTokenHelperAsync`` para garantir um token de acesso atualizado a fim de passar na solicitação.

```c#
                HttpClient client = new HttpClient();
                var token = await AuthenticationHelper.GetTokenHelperAsync();
                client.DefaultRequestHeaders.Add("Authorization", "Bearer " + token);

                // Build contents of post body and convert to StringContent object.
                // Using line breaks for readability.
                string postBody = "{'Message':{" 
                    +  "'Body':{ " 
                    + "'Content': '" + bodyContent + "'," 
                    + "'ContentType':'HTML'}," 
                    + "'Subject':'" + subject + "'," 
                    + "'ToRecipients':[" + recipientsJSON +  "]}," 
                    + "'SaveToSentItems':true}";

                var emailBody = new StringContent(postBody, System.Text.Encoding.UTF8, "application/json");

                HttpResponseMessage response = await client.PostAsync(new Uri("https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail"), emailBody);

                if ( !response.IsSuccessStatusCode)
                {

                    throw new Exception("We could not send the message: " + response.StatusCode.ToString());
                }
```

A classe completa terá a seguinte aparência:

```c#
    class MailHelper
    {
        /// <summary>
        /// Compose and send a new email.
        /// </summary>
        /// <param name="subject">The subject line of the email.</param>
        /// <param name="bodyContent">The body of the email.</param>
        /// <param name="recipients">A semicolon-separated list of email addresses.</param>
        /// <returns></returns>
        internal async Task ComposeAndSendMailAsync(string subject,
                                                            string bodyContent,
                                                            string recipients)
        {

            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            string recipientsJSON = null;

            int n = 0;
            foreach (string recipient in splitRecipientsString)
            {
                if ( n==0)
                recipientsJSON += "{'EmailAddress':{'Address':'" + recipient.Trim() + "'}}";
                else
                {
                    recipientsJSON += ", {'EmailAddress':{'Address':'" + recipient.Trim() + "'}}";
                }
                n++;
            }

            try
            {

                HttpClient client = new HttpClient();
                var token = await AuthenticationHelper.GetTokenForUserAsync();
                client.DefaultRequestHeaders.Add("Authorization", "Bearer " + token);

                // Build contents of post body and convert to StringContent object.
                // Using line breaks for readability.
                string postBody = "{'Message':{" 
                    +  "'Body':{ " 
                    + "'Content': '" + bodyContent + "'," 
                    + "'ContentType':'HTML'}," 
                    + "'Subject':'" + subject + "'," 
                    + "'ToRecipients':[" + recipientsJSON +  "]}," 
                    + "'SaveToSentItems':true}";

                var emailBody = new StringContent(postBody, System.Text.Encoding.UTF8, "application/json");

                HttpResponseMessage response = await client.PostAsync(new Uri("https://graph.microsoft.com/v1.0/me/microsoft.graph.SendMail"), emailBody);

                if ( !response.IsSuccessStatusCode)
                {

                    throw new Exception("We could not send the message: " + response.StatusCode.ToString());
                }


            }

            catch (Exception e)
            {
                throw new Exception("We could not send the message: " + e.Message);
            }
        }
    }
```

**Versão de biblioteca de cliente**

A versão da biblioteca de cliente deste arquivo exige as seguintes declarações `using`:

```c#
using System;
using System.Collections.Generic;
using System.Threading.Tasks;
```

O código para enviar uma mensagem com a biblioteca de cliente parece muito com o código que utiliza chamadas REST. Em vez de criar objetos JSON e passá-los diretamente para o ponto de extremidade **SendMail** em uma solicitação de HTTP POST, crie objetos equivalentes que são definidos na biblioteca de cliente e passe o objeto `Message` resultante para o método `SendMail` do `GraphServiceClient`. O cliente faz o trabalho de buscar o token de acesso e passar a solicitação para o ponto de extremidade **SendMail**.

A classe completa terá a seguinte aparência:

```c#
    public class MailHelper
    {
        /// <summary>
        /// Compose and send a new email.
        /// </summary>
        /// <param name="subject">The subject line of the email.</param>
        /// <param name="bodyContent">The body of the email.</param>
        /// <param name="recipients">A semicolon-separated list of email addresses.</param>
        /// <returns></returns>
        public async Task ComposeAndSendMailAsync(string subject,
                                                            string bodyContent,
                                                            string recipients)
        {

            // Prepare the recipient list
            string[] splitter = { ";" };
            var splitRecipientsString = recipients.Split(splitter, StringSplitOptions.RemoveEmptyEntries);
            List<Recipient> recipientList = new List<Recipient>();

            foreach (string recipient in splitRecipientsString)
            {
                recipientList.Add(new Recipient { EmailAddress = new EmailAddress { Address = recipient.Trim() } });
            }

            try
            {
                var graphClient = AuthenticationHelper.GetAuthenticatedClient();

                var email = new Message
                {
                    Body = new ItemBody
                    {
                        Content = bodyContent,
                        ContentType = BodyType.Html,
                    },
                    Subject = subject,
                    ToRecipients = recipientList,
                };

                try
                {
                    await graphClient.Me.SendMail(email, true).Request().PostAsync();
                }
                catch (ServiceException exception)
                {
                    throw new Exception("We could not send the message: " + exception.Error == null ? "No error message returned." : exception.Error.Message);
                }


            }

            catch (Exception e)
            {
                throw new Exception("We could not send the message: " + e.Message);
            }
        }
    }
``` 

##<a name="create-the-user-interface-in-mainpagexaml"></a>Criar a interface de usuário no MainPage.xaml

Agora que você escreveu o código que faz todo o trabalho de autenticar o usuário e enviar uma mensagem por meio do Microsoft Graph, tudo o que você precisa fazer é criar a interface simples descrita acima. 

O arquivo MainPage.xaml em seu projeto inicial já inclui todo o XAML necessário. Basta adicionar o código que orienta a interface para o arquivo MainPage.xaml.cs. Localize o arquivo no seu projeto e abra-o.

Este arquivo já contém todas as declarações `using` obrigatórias à biblioteca de cliente e às versões REST do exemplo.

***Versão de biblioteca de cliente***

A versão de biblioteca de cliente do aplicativo cria um `GraphServiceClient` quando o usuário autentica. 

Adicione esse código dentro do seu namespace para concluir a versão da biblioteca do cliente da classe MainPage em MainPage.xaml.cs:

```c#
    public sealed partial class MainPage : Page
    {
        private string _mailAddress;
        private string _displayName = null;
        private MailHelper _mailHelper = new MailHelper();

        public MainPage()
        {
            this.InitializeComponent();
        }

        protected override void OnNavigatedTo(NavigationEventArgs e)
        {
            // Developer code - if you haven't registered the app yet, we warn you. 
            if (!App.Current.Resources.ContainsKey("ida:ClientID"))
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("NoClientIdMessage");
                ConnectButton.IsEnabled = false;
            }
            else
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("ConnectPrompt");
                ConnectButton.IsEnabled = true;
            }
        }

        /// <summary>
        /// Signs in the current user.
        /// </summary>
        /// <returns></returns>
        public async Task<bool> SignInCurrentUserAsync()
        {
            var graphClient = AuthenticationHelper.GetAuthenticatedClient();

            if (graphClient != null)
            {
                var user = await graphClient.Me.Request().GetAsync();
                string userId = user.Id;
                _mailAddress = user.UserPrincipalName;
                _displayName = user.DisplayName;
                return true;
            }
            else
            {
                return false;
            }

        }


        private async void ConnectButton_Click(object sender, RoutedEventArgs e)
        {
            ProgressBar.Visibility = Visibility.Visible;
            if (await SignInCurrentUserAsync())
            { 
                InfoText.Text = "Hi " + _displayName + "," + Environment.NewLine + ResourceLoader.GetForCurrentView().GetString("SendMailPrompt");
                MailButton.IsEnabled = true;
                EmailAddressBox.IsEnabled = true;
                ConnectButton.Visibility = Visibility.Collapsed;
                DisconnectButton.Visibility = Visibility.Visible;
                EmailAddressBox.Text = _mailAddress;
            }
            else
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("AuthenticationErrorMessage");
            }

            ProgressBar.Visibility = Visibility.Collapsed;
        }

        private async void MailButton_Click(object sender, RoutedEventArgs e)
        {
            _mailAddress = EmailAddressBox.Text;
            ProgressBar.Visibility = Visibility.Visible;
            MailStatus.Text = string.Empty;
            try
            {
                await _mailHelper.ComposeAndSendMailAsync(ResourceLoader.GetForCurrentView().GetString("MailSubject"), ComposePersonalizedMail(_displayName), _mailAddress);
                MailStatus.Text = string.Format(ResourceLoader.GetForCurrentView().GetString("SendMailSuccess"), _mailAddress);
            }
            catch (Exception)
            {
                MailStatus.Text = ResourceLoader.GetForCurrentView().GetString("MailErrorMessage");
            }
            finally
            {
                ProgressBar.Visibility = Visibility.Collapsed;
            }
            
        }

        // <summary>
        // Personalizes the email.
        // </summary>
        public static string ComposePersonalizedMail(string userName)
        {
            return String.Format(ResourceLoader.GetForCurrentView().GetString("MailContents"), userName);
        }

        private void Disconnect_Click(object sender, RoutedEventArgs e)
        {
            ProgressBar.Visibility = Visibility.Visible;
            AuthenticationHelper.SignOut();
            ProgressBar.Visibility = Visibility.Collapsed;
            MailButton.IsEnabled = false;
            EmailAddressBox.IsEnabled = false;
            ConnectButton.Visibility = Visibility.Visible;
            InfoText.Text = ResourceLoader.GetForCurrentView().GetString("ConnectPrompt");
            this._displayName = null;
            this._mailAddress = null;
        }
    }
```

***Versão REST***

A versão REST dessa classe se parece muito com a versão da biblioteca de cliente, exceto pelo fato de chamar o método `GetTokenForUserAsync` diretamente quando o usuário autentica. Ela também recupera valores de usuário das configurações de roaming do aplicativo. 

Adicione esse código dentro de seu namespace para concluir a versão REST da classe MainPage em MainPage.xaml.cs:

```c#
    public sealed partial class MainPage : Page
    {
        private string _mailAddress;
        private string _displayName = null;
        private MailHelper _mailHelper = new MailHelper();
        public static ApplicationDataContainer _settings = ApplicationData.Current.RoamingSettings;

        public MainPage()
        {
            this.InitializeComponent();
        }

        protected override void OnNavigatedTo(NavigationEventArgs e)
        {
            // Developer code - if you haven't registered the app yet, we warn you. 
            if (!App.Current.Resources.ContainsKey("ida:ClientID"))
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("NoClientIdMessage");
                ConnectButton.IsEnabled = false;
            }
            else
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("ConnectPrompt");
                ConnectButton.IsEnabled = true;
            }
        }

        /// <summary>
        /// Signs in the current user.
        /// </summary>
        /// <returns></returns>
        public async Task<bool> SignInCurrentUserAsync()
        {
            var token = await AuthenticationHelper.GetTokenForUserAsync();

            if (token != null)
            {
                string userId = (string)_settings.Values["userID"];
                _mailAddress = (string)_settings.Values["userEmail"];
                _displayName = (string)_settings.Values["userName"];
                return true;
            }
            else
            {
                return false;
            }

        }


        private async void ConnectButton_Click(object sender, RoutedEventArgs e)
        {
            ProgressBar.Visibility = Visibility.Visible;
            if (await SignInCurrentUserAsync())
            { 
                InfoText.Text = "Hi " + _displayName + "," + Environment.NewLine + ResourceLoader.GetForCurrentView().GetString("SendMailPrompt");
                MailButton.IsEnabled = true;
                EmailAddressBox.IsEnabled = true;
                ConnectButton.Visibility = Visibility.Collapsed;
                DisconnectButton.Visibility = Visibility.Visible;
                EmailAddressBox.Text = _mailAddress;
            }
            else
            {
                InfoText.Text = ResourceLoader.GetForCurrentView().GetString("AuthenticationErrorMessage");
            }

            ProgressBar.Visibility = Visibility.Collapsed;
        }

        private async void MailButton_Click(object sender, RoutedEventArgs e)
        {
            _mailAddress = EmailAddressBox.Text;
            ProgressBar.Visibility = Visibility.Visible;
            MailStatus.Text = string.Empty;
            try
            {
                await _mailHelper.ComposeAndSendMailAsync(ResourceLoader.GetForCurrentView().GetString("MailSubject"), ComposePersonalizedMail(_displayName), _mailAddress);
                MailStatus.Text = string.Format(ResourceLoader.GetForCurrentView().GetString("SendMailSuccess"), _mailAddress);
            }
            catch (Exception)
            {
                MailStatus.Text = ResourceLoader.GetForCurrentView().GetString("MailErrorMessage");
            }
            finally
            {
                ProgressBar.Visibility = Visibility.Collapsed;
            }
            
        }

        // <summary>
        // Personalizes the email.
        // </summary>
        public static string ComposePersonalizedMail(string userName)
        {
            return String.Format(ResourceLoader.GetForCurrentView().GetString("MailContents"), userName);
        }

        private void Disconnect_Click(object sender, RoutedEventArgs e)
        {
            ProgressBar.Visibility = Visibility.Visible;
            AuthenticationHelper.SignOut();
            ProgressBar.Visibility = Visibility.Collapsed;
            MailButton.IsEnabled = false;
            EmailAddressBox.IsEnabled = false;
            ConnectButton.Visibility = Visibility.Visible;
            InfoText.Text = ResourceLoader.GetForCurrentView().GetString("ConnectPrompt");
            this._displayName = null;
            this._mailAddress = null;
        }
    }
```
 
Agora você realizou as três etapas obrigatórias para interagir com o Microsoft Graph: registro do aplicativo, autenticação do usuário e solicitação. 

## <a name="run-the-app"></a>Executar o aplicativo
1. Pressione F5 para criar e executar o aplicativo. 

2. Entre com sua conta pessoal, comercial ou de estudante, e conceda as permissões solicitadas.

3. Escolha o botão **Enviar email**. Quando o email for enviado, será exibida uma mensagem de sucesso abaixo do botão.

## <a name="next-steps"></a>Próximas etapas
- Experimente a API REST, usando o [Explorador do Graph](https://graph.microsoft.io/graph-explorer).
- Encontre exemplos de operações comuns para operações REST e SDK no [Exemplo de trechos de UWP do Microsoft Graph (SDK)](https://github.com/microsoftgraph/uwp-csharp-snippets-sample) e no [Exemplo de trechos de UWP do Microsoft Graph (REST)](https://github.com/microsoftgraph/uwp-csharp-snippets-rest-sample) ou explore nossos outros [exemplos de UWP](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=uwp) no GitHub.

## <a name="see-also"></a>Ver também
- [Biblioteca de cliente do .NET do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet)
- [Protocolos do Azure AD v2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [Tokens do Azure AD v2.0](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)

