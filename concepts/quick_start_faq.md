# <a name="microsoft-graph-quick-start-faq"></a>Perguntas frequentes do Início Rápido do Microsoft Graph

Essas Perguntas Frequentes abordam dúvidas e problemas que podem ocorrer ao percorrer um dos [Inícios Rápidos do Microsoft Graph](https://developer.microsoft.com/en-us/graph/quick-start).

## <a name="what-do-the-quick-starts-do"></a>O que os inícios rápidos fazem?

Os exemplos de início rápido mostram como acessar os recursos do Microsoft Graph. 

Com as APIs REST anteriores da Microsoft, você precisava se autenticar em cada serviço que queria chamar. O Microsoft Graph elimina essa complexidade para os desenvolvedores unificando a autenticação e combinando todos os pontos de entrada da API em um ponto de entrada da API do Graph. Agora você faz a autenticação uma vez e obtém a capacidade de acessar informações em vários aplicativos e serviços. 

Para fins ilustrativos, o exemplo de início rápido do Microsoft Graph acessará três serviços diferentes com uma autenticação: Conta da Microsoft, OneDrive e Outlook. Cada guia de início rápido obterá informações de perfis de usuários da Conta da Microsoft, combinando-as à gravação de dados no OneDrive (uma foto), gerando em seguida um email usando o Outlook (incluindo um link para a foto). 

Há quatro etapas para cada guia de início rápido para obter um aplicativo de exemplo que está pronto para ser executado:
- Selecione sua plataforma 
- Obter sua ID de aplicativo (também conhecida como ID de cliente)
- Criar o exemplo,
- Entrar e enviar uma foto do perfil via email

>Observação: isso não foi projetado para ser um código pronto para a produção. Trata-se apenas de ilustrações fáceis de como você pode utilizar o mesmo cenário em muitas plataformas e linguagens de programação diferentes. Após fazer um início rápido, recomendamos que você [entenda totalmente a autenticação](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-authentication-scenarios) para criar aplicativos prontos para produção.


## <a name="general-quick-start-sample-questions"></a>Exemplos de perguntas do início rápido gerais
Perguntas sobre a organização e o conteúdo do pacote de exemplos de início rápido.

### <a name="why-does-my-quick-start-contain-a-readme-file"></a>Por que meu início rápido contém um arquivo Leiame?

Cada início rápido registra um novo aplicativo e cria um arquivo zip que contém o conteúdo de um repositório do GitHub. Ele atualiza os arquivos no repositório para que você não precise configurar o aplicativo de exemplo no repositório. Você pode ver esses repositórios na [organização do MicrosoftGraph](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect) no GitHub.

Fique à vontade para examinar o repositório associado a cada início rápido, problemas de arquivo e/ou seguir as instruções no Leiame para registrar seu próprio aplicativo. Siga o link **Basta dar-me o código de exemplo** na etapa 2 de cada guia de início rápido para ir para o repositório associado.

### <a name="which-microsoft-api-features-do-the-quick-start-samples-show"></a>Quais recursos da API Microsoft os exemplos de início rápido mostram?

O pacote de exemplos está sendo continuamente melhorado. Assista ao repositório de exemplo em que você está interessado. Ao adicionarmos recursos a seu exemplo favorito, anunciamos a adição através do Leiame de exemplo. A tabela a seguir mostra os recursos atuais de cada exemplo

|Exemplo|Autenticar|Obter imagem do perfil|Carregar imagem no OneDrive|Compartilhando link no email|Anexar imagem a um email|Enviar email|
|-----:|-----:|-----:|------:|------:|------:|-----:|
|[Android Connect](https://github.com/microsoftgraph/android-java-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[Angular 2 Connect](https://github.com/microsoftgraph/angular-connect-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[Angular 2 Connect REST](https://github.com/microsoftgraph/angular2-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[ASP.NET Connect](https://github.com/microsoftgraph/aspnet-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[iOS Connect - Swift](https://github.com/microsoftgraph/ios-swift-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[iOS Connect REST - Objective C](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|[](./images/Check.PNG)|
|[Node.js Connect REST](https://github.com/microsoftgraph/nodejs-connect-rest-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)| |![](./images/Check.PNG)|
|[php Connect REST](https://github.com/microsoftgraph/php-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[php Connect](https://github.com/microsoftgraph/php-connect-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[Ruby Connect REST](https://github.com/microsoftgraph/ruby-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[UWP Connect](https://github.com/microsoftgraph/uwp-csharp-connect-sample) |![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[Xamarin Connect](https://github.com/microsoftgraph/uwp-csharp-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|

## <a name="authentication-and-authorization"></a>Autenticação e autorização
Perguntas relacionadas a problemas de autenticação e autorização. 

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>Por que nenhum dos exemplos de início rápido mostra casos de uso de autenticação avançados?

Os exemplos de início rápido oferecem uma introdução à autenticação e às chamadas à API do Microsoft Graph. Ao adicionar autenticação e chamadas à API do Graph ao aplicativo de produção, você precisa saber como projetar para cenários avançados de autenticação que envolvem problemas de segurança e acesso condicional.

Para encontrar mais informações sobre cenários avançados de autenticação para a biblioteca de autenticação que está usando, acesse as páginas do editor da biblioteca de autenticação.

- [OAuth2Client para Android e iOS](https://github.com/nxtbgthng/OAuth2Client)
- [Passport para Node](http://passportjs.org/)
- [Illuminate Auth para PHP](https://github.com/illuminate/auth)
- [Flask para Python 3](https://pypi.python.org/pypi/Flask-OAuth2-Provider/0.2.1)
- [OmniAuth para Ruby](https://github.com/omniauth/omniauth)
- [Biblioteca de Autenticação da Microsoft (MSAL) para .NET](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet)
- [Biblioteca de Autenticação da Microsoft para Android](https://github.com/AzureAD/microsoft-authentication-library-for-android)
- [Biblioteca de Autenticação da Microsoft para JavaScript](https://github.com/AzureAD/microsoft-authentication-library-for-js)

## <a name="microsoft-graph-api"></a>API do Microsoft Graph
Perguntas sobre codificação para a API do Microsoft Graph

### <a name="i-didnt-get-an-email-and-i-see-no-errors-or-exceptions-why-didnt-this-work"></a>Eu não recebi um email e não vejo erros ou exceções. Por que isso não funcionou?

Se parecer que o exemplo enviou um email, mas ele não for exibido em sua Caixa de Entrada, verifique a pasta de lixo eletrônico ou spam. Se você estiver enviando a mensagem de um locatário de teste, a mensagem poderá ser sinalizada como spam.

### <a name="why-doesnt-the-email-sent-by-the-sample-have-my-profile-picture"></a>Por que o email enviado pelos exemplo não tem minha imagem do perfil?

- Isso geralmente ocorre porque seu perfil não foi configurado com uma imagem de perfil de usuário. Se você entrou com uma MSA (Conta de Serviço da Microsoft), mesmo que tenha uma imagem do perfil, ela não será exibida no email. A API do Microsoft Graph não dá suporte no momento a imagens de perfil de usuário de contas MSA. <br/>A maioria dos exemplos fornecidos pelo inícios rápidos pegam sua imagem do perfil e carregam-a na pasta raiz de sua conta do OneDrive. Se você entrar com uma conta da Microsoft (live.com, hotmail.com), atualmente, o Microsoft Graph não consegue buscar sua imagem do perfil e, portanto, retornamos à imagem do balão de pensamento.

- O exemplo do Node e os exemplos do iOS Objective C não anexam imagens de perfil de usuário à mensagem de email. 

## <a name="asp-net"></a>ASP .NET
Perguntas relacionadas a codificação, compilação ou execução do exemplo de início rápido do ASP.NET.

## <a name="universal-windows-platform-uwp"></a>UWP (Plataforma Universal do Windows)
Perguntas relacionadas a codificação, compilação ou execução do exemplo de início rápido da UWP.

## <a name="xamarin"></a>Xamarin
Perguntas relacionadas a codificação, compilação ou execução do exemplo de início rápido do Xamarin.

### <a name="why-wont-my--aspnet-uwp-or-xamarin-project-build"></a>Por que meu projeto ASP.NET, UWP ou Xamarin não é compilado?

Se um exemplo que usa bibliotecas .NET falhar ao compilar no Visual Studio, um ou mais dos projetos podem estar sendo executados no limite do comprimento do caminho do Windows que é de 260 caracteres. Principalmente as soluções Xamarin estão sujeitas a isso, especialmente projetos do Android em soluções Xamarin. Tente mover a solução para um local no ou próxima ao diretório raiz. 

## <a name="web-stack-samples"></a>Exemplos de pilha da Web
Perguntas relacionadas a exemplos de início rápido de codificação, compilação ou execução criados com tecnologia da Web.

### <a name="how-do-i-know-if-my-local-computer-supports-a-local-web-server"></a>Como saber se meu computador local dá suporte a um servidor Web local?
Os exemplos de início rápido com base em tecnologia da Web fornecem a lógica necessária para iniciar e hospedar um servidor Web local. O exemplo de php com base em tempo de execução do php 5.4.0+ inclui um [servidor Web interno](http://php.net/manual/en/features.commandline.webserver.php) que você usará para desenvolvimento. Não se destina a ser usado em um ambiente de produção. 

Se você tiver baixado o exemplo do Node.js, leia este [Guia de Introdução do Node.js](https://nodejs.org/en/docs/guides/getting-started-guide/) para saber como iniciar o servidor Web do Node. 

Para o exemplo do ASP.NET, do Visual Studio 2015 e de versões mais recentes, inclua um servidor Web de desenvolvimento que é iniciado automaticamente quando você executa o exemplo. Não é necessário configurar o projeto de exemplo para usar o servidor Web. 

O [leiame](https://github.com/microsoftgraph/ruby-connect-rest-sample/blob/master/README.md) de exemplo de conexão ao Ruby fornece as instruções necessárias para iniciar um servidor Web Ruby local. 

### <a name="if-a-web-platform-quick-start-provides-rest-and-sdk-samples-can-i-run-them-both-at-the-same-time"></a>Se o início rápido de uma plataforma Web fornecer exemplos de REST e SDK, posso executá-los ao mesmo tempo?

Sim, você pode executar os dois exemplos ao mesmo tempo. Basta verificar se um deles não está sendo executado na porta padrão. Isso significa que, quando você inicia o servidor Web de teste, será necessário especificar um número de porta para, pelo menos, uma versão do exemplo.

### <a name="why-do-some-quick-starts-include-an-app-secret-and-others-dont"></a>Por que alguns inícios rápidos incluem um segredo do aplicativo e outros não?

Os aplicativos Web do servidor que precisam fazer chamadas seguras para a API do Microsoft Graph exigem segredos do aplicativo. Isso ocorre porque os inícios rápidos do ASP.NET MVC, Node.js, PHP e Ruby fornecem um segredo do aplicativo.

### <a name="why-doesnt-the-angular-quick-start-give-me-an-app-secret-when-all-the-other-web-platform-quick-starts-do"></a>Por que o início rápido do Angular não me oferece um segredo do aplicativo quando todos os demais inícios rápidos da plataforma Web oferecem?

O segredo do aplicativo só é necessário para aplicativos Web do servidor.

### <a name="i-get-an-error-when-i-try-to-sign-in-and-authorize-the-sample-app-what-steps-can-i-take-to-fix-this"></a>Recebo um erro quando tento entrar e autorizar o aplicativo de teste. Quais etapas posso seguir para corrigir isso? 

Primeiro, tente executar o aplicativo de exemplo em uma janela InPrivate ou Incognito. Às vezes, as configurações de cache do navegador da Web podem fazer com que a etapa de autorização falhe, especialmente se você entrar com várias contas da Microsoft. Se isso não funcionar, entre em contato conosco em [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). Lembre-se de marcar sua pergunta com microsoft-graph e copie as informações de erro para a pergunta.

## <a name="didnt-find-what-you-need"></a>Não consegue encontrar o que precisa?

Se essas Perguntas Frequentes não esclareceram sua dúvida ou trataram de um problema encontrado em um ou mais inícios rápidos, informe seu problema ou pergunta no [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). 

Se seu problema tiver relação com o exemplo de código fornecido pelo início rápido, você também poderá apresentar o problema no repositório de exemplos do GitHub. Localize o repositório seguindo o link **Basta dar-me o código de exemplo** na etapa 2 de cada guia de início rápido.
