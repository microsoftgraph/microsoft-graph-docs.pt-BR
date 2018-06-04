# <a name="ios-samples-for-the-microsoft-graph-api"></a>Exemplos de iOS para a API do Microsoft Graph
Este artigo apresenta dois exemplos do iOS que autenticam um usuário em relação ao Office 365 ou a MSA (Contas de Serviço Gerenciadas), como os usuários do Outlook de consumidor. Ambos os exemplos enviam um email por meio do serviço do Outlook, mas um dos exemplos estende o recurso obtendo a foto do perfil do usuário e enviando-a no corpo do email

## <a name="ios-objective-c-connect-rest-sample"></a>Exemplo de iOS Objective-C Connect REST
Este exemplo usa uma biblioteca HTTPS iOS padrão para fazer chamadas REST ao Microsoft Graph. Ele usa a [MSAL (Biblioteca de Autenticação da Microsoft)](https://github.com/AzureAD/microsoft-authentication-library-for-objc/blob/dev/README.md) para autenticar um usuário. A biblioteca MSAL permite que o aplicativo autentique um usuário do Office 365 ou de uma conta MSA. Porém, você não poderá autenticar um usuário de uma instância do Azure Active Directory localmente.

Você pode enviar um email com este exemplo, mas ele não recupera a foto do usuário autenticado nem a insere no email.

- [Introdução ao Microsoft Graph em um aplicativo Objective-C iOS](ios_objectivec.md)

## <a name="ios-swift-connect-rest-sample"></a>Exemplo de iOS Swift Connect REST
Este exemplo usa a biblioteca Foundation HTTP e o [PromiseKit](https://github.com/mxcl/PromiseKit/blob/master/README.md) para acessar o ponto de extremidade do Microsoft Graph usando operações REST com o padrão assíncrono **Promessas**. Ele usa a [MSAL (Biblioteca de Autenticação da Microsoft)](https://github.com/AzureAD/microsoft-authentication-library-for-objc/blob/dev/README.md) para autenticar um usuário. A biblioteca permite que o aplicativo autentique um usuário do Office 365 ou da MSA.

O exemplo mostra como acessar o perfil do Azure do usuário por meio do Graph. Você também aprenderá a obter foto do perfil do usuário, carregar a foto para o armazenamento do OneDrive do usuário e inserir a foto no corpo de uma mensagem de email do Outlook.

- [Introdução ao Microsoft Graph em um aplicativo iOS](ios_swift.md)
