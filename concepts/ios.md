# <a name="ios-samples-for-the-microsoft-graph-api"></a>Exemplos de iOS para a API do Microsoft Graph
Este artigo apresenta dois exemplos do iOS que autenticam um usuário em relação ao Office 365 ou a MSA (Contas de Serviço Gerenciadas), como os usuários do Outlook de consumidor. Ambos os exemplos enviam um email por meio do serviço do Outlook, mas um dos exemplos estende o recurso obtendo a foto do perfil do usuário e enviando-a no corpo do email

## <a name="ios-objective-c-connect-rest-sample"></a>Exemplo de iOS Objective C Connect REST
Este exemplo usa uma biblioteca HTTPS iOS padrão para fazer chamadas REST ao Microsoft Graph. Usa a MSAL (Biblioteca de Autenticação da Microsoft) para autenticar um usuário. A biblioteca MSAL permite que o aplicativo autentique um usuário do Office 365 ou de uma conta MSA. Porém, você não poderá autenticar um usuário de uma instância do Azure Active Directory localmente.

Você pode enviar um email com este exemplo, mas ele não recupera a foto do usuário autenticado nem a insere no email.

- [Introdução ao Microsoft Graph em um aplicativo Objectve C iOS](ios_objectivec.md)

## <a name="ios-swift-sonnect-sample"></a>Exemplo de iOS Swift Sonnect
Este exemplo utiliza a biblioteca de cliente do Microsoft Graph para Objective C para acessar o ponto de extremidade do Microsoft Graph. A autenticação do usuário é tratada pela biblioteca de terceiros [NXOAuth2Client](https://github.com/nxtbgthng/OAuth2Client). Esta biblioteca permite que o aplicativo autentique um usuário de uma instância do Azure Active Directory local, mas não permite autenticar usuários MSA.

O exemplo mostra como acessar o perfil do Azure do usuário por meio do Graph. Você também aprenderá a obter foto do perfil do usuário, carregar a foto para o armazenamento do OneDrive do usuário e inserir a foto no corpo de uma mensagem de email do Outlook.

- [Introdução ao Microsoft Graph em um aplicativo iOS](ios_swift.md)