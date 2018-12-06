---
title: Perguntas frequentes do início rápido do Microsoft Graph
description: Estas perguntas frequentes respondem dúvidas relacionadas aos Inícios Rápidos do Microsoft Graph.
ms.openlocfilehash: 90e16a340d4dbb337cbe0af5f799476b28eba200
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091651"
---
# <a name="microsoft-graph-quick-start-faq"></a>Perguntas frequentes do início rápido do Microsoft Graph

Estas perguntas frequentes respondem dúvidas relacionadas aos [Inícios Rápidos do Microsoft Graph](https://developer.microsoft.com/graph/quick-start).

## <a name="what-do-the-quick-starts-do"></a>O que os inícios rápidos fazem?

Os exemplos de início rápido mostram como acessar os recursos do Microsoft Graph. 

Se você usa as APIs REST do Office 365, você deve autenticar para cada serviço que deseja chamar. O Microsoft Graph elimina essa complexidade unificando a autenticação e dando acesso a todas as APIs através de um único ponto de entrada. Você pode autenticar uma vez e acessar informações em vários aplicativos e serviços. 

Os inícios rápidos do Microsoft Graph acessa três serviços com uma autenticação: Conta da Microsoft, OneDrive e Outlook. Cada guia de início rápido acessa informações de perfis de usuários da conta da Microsoft, grava dados no OneDrive (uma foto) e gera um email usando o Outlook (incluindo um link para a foto). 

Os inícios rápidos envolvem quatro etapas:

- Selecione sua plataforma 
- Obter sua ID de aplicativo (ID do cliente)
- Criar o exemplo
- Entrar e enviar uma foto do perfil via email

Quando você completar o início rápido, você possui um aplicativo pronto para ser executado.


## <a name="general-quick-start-sample-questions"></a>Exemplos de perguntas do início rápido gerais
Esta seção responde perguntas sobre a organização e o conteúdo dos exemplos de início rápido.

### <a name="why-does-my-quick-start-contain-a-readme-file"></a>Por que meu início rápido contém um arquivo Leiame?

Cada início rápido registra um novo aplicativo e cria um arquivo zip que contém o conteúdo de um repositório do GitHub. Ele atualiza os arquivos no repositório para que você não precise configurar o aplicativo de exemplo no repositório. Você pode ver esses repositórios na [organização do MicrosoftGraph](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect) no GitHub.

Fique à vontade para examinar o repositório associado a cada início rápido, problemas de arquivo e/ou seguir as instruções no Leiame para registrar seu próprio aplicativo. Vá até o repositório, siga o link **Basta dar-me o código de exemplo** na etapa 2 de cada guia de início rápido.

### <a name="which-microsoft-graph-features-do-the-quick-start-samples-use"></a>Quais recursos do Microsoft Graph os exemplos de início rápido mostram?

Estamos continuamente atualizando as amostras do início rápido. Para obter as atualizações, assista o repositório para a amostra em que você está interessado. À medida que adicionamos recursos, atualizaremos o arquivo Leiame da amostra com as novas informações. A tabela a seguir lista os recursos atuais para cada amostra.
 +<!-- Replace the check mark images with an actual character that can be read by a screen reader. Or you could add alt text to each instance of the image. -->

|Amostra|Autenticar|Obter imagem do perfil|Carregar imagem no OneDrive|Compartilhando link no email|Anexar imagem a um email|Enviar email|
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
Esta seção responde perguntas relacionadas a problemas de autenticação e autorização. 

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>Por que nenhum dos exemplos de início rápido mostra casos de uso de autenticação avançados?

Os exemplos de início rápido oferecem uma introdução à autenticação e às chamadas à API do Microsoft Graph. Ao adicionar autenticação e chamadas à API do Microsoft Graph ao aplicativo de produção, você precisa saber como projetar para cenários avançados de autenticação que envolvem problemas de segurança e acesso condicional.

Você pode encontrar mais informações sobre cenários avançados de autenticação para a biblioteca de autenticação que está usando ao acessar a página do editor da biblioteca de autenticação.

- [OAuth2Client para Android e iOS](https://github.com/nxtbgthng/OAuth2Client)
- [Passport para Node](https://passportjs.org/)
- [Illuminate Auth para PHP](https://github.com/illuminate/auth)
- [Flask para Python 3](https://pypi.python.org/pypi/Flask-OAuth2-Provider/0.2.1)
- [OmniAuth para Ruby](https://github.com/omniauth/omniauth)
- [Biblioteca de Autenticação da Microsoft (MSAL) para .NET](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet)
- [Biblioteca de Autenticação da Microsoft para Android](https://github.com/AzureAD/microsoft-authentication-library-for-android)
- [Biblioteca de Autenticação da Microsoft para JavaScript](https://github.com/AzureAD/microsoft-authentication-library-for-js)

## <a name="microsoft-graph-api"></a>API do Microsoft Graph
Esta seção responde perguntas sobre codificação de aplicativos que usam as APIs do Microsoft Graph.

### <a name="i-didnt-get-an-email-and-i-dont-see-any-errors-or-exceptions-why-didnt-this-work"></a>Eu não recebi um email e não vejo erros ou exceções. Por que isso não funcionou?

Se parecer que o exemplo enviou um email, mas ele não for exibido em sua Caixa de Entrada, verifique a pasta de lixo eletrônico ou spam. Se você estiver enviando a mensagem de um locatário de teste, a mensagem poderá ser sinalizada como spam.

### <a name="why-doesnt-the-email-sent-by-the-sample-have-my-profile-picture"></a>Por que o email enviado pelos exemplo não tem minha imagem do perfil?

Isso geralmente ocorre porque seu perfil não foi configurado com uma imagem de perfil de usuário. Se você entrou com uma conta da Microsoft, mesmo que tenha uma imagem do perfil, ela não será exibida no email. A API do Microsoft Graph não dá suporte no momento a imagens de perfil de usuário de contas da Microsoft. A maioria dos exemplos de inícios rápidos pegam sua imagem do perfil e carregam-a na pasta raiz de sua conta do OneDrive. Se você entrar com uma conta da Microsoft (live.com, hotmail.com), atualmente, o Microsoft Graph não consegue buscar sua imagem do perfil e, portanto, retornaremos à imagem do balão de pensamento.

Os exemplos do Node iOS Objective C não anexam imagens de perfil de usuário à mensagem de email. 

## <a name="aspnet"></a>ASP.NET
Esta seção responde perguntas relacionadas a codificação, compilação ou execução do exemplo de início rápido do ASP.NET.

### <a name="why-wont-my-aspnet-project-build"></a>Por que meu projeto ASP.NET não será desenvolvido?
Se um exemplo que usa bibliotecas .NET falhar ao compilar no Visual Studio, um ou mais dos projetos podem estar sendo executados no limite do comprimento do caminho do Windows que é de 260 caracteres. Tente mover a solução para um local no ou próxima ao diretório raiz. 

## <a name="universal-windows-platform-uwp"></a>UWP (Plataforma Universal do Windows)
Esta seção responde perguntas relacionadas a codificação, compilação ou execução do exemplo de início rápido da UWP.

### <a name="why-wont-my-uwp-project-build"></a>Por que meu projeto UWP não será desenvolvido?
Se um exemplo que usa bibliotecas .NET falhar ao compilar no Visual Studio, um ou mais dos projetos podem estar sendo executados no limite do comprimento do caminho do Windows que é de 260 caracteres. Tente mover a solução para um local no ou próxima ao diretório raiz. 

## <a name="xamarin"></a>Xamarin
Esta seção responde perguntas relacionadas a codificação, compilação ou execução do exemplo de início rápido do Xamarin.

### <a name="why-wont-my-xamarin-project-build"></a>Por que meu projeto Xamarin não será desenvolvido?

Se um exemplo que usa bibliotecas .NET falhar ao compilar no Visual Studio, um ou mais dos projetos podem estar sendo executados no limite do comprimento do caminho do Windows que é de 260 caracteres. Principalmente as soluções Xamarin estão sujeitas a isso, especialmente projetos do Android em soluções Xamarin. Tente mover a solução para um local no ou próxima ao diretório raiz. 

## <a name="web-stack-samples"></a>Exemplos de pilha da Web
Esta seção responde perguntas relacionadas a exemplos de início rápido de codificação, compilação ou execução criados com tecnologia da Web.

### <a name="how-do-i-know-if-my-local-computer-supports-a-local-web-server"></a>Como saber se meu computador local dá suporte a um servidor Web local?
Os exemplos de início rápido com base em tecnologia da Web fornecem a lógica necessária para iniciar e hospedar um servidor Web local. O exemplo de PHP com base em tempo de execução do PHP 5.4.0+ inclui um [servidor Web interno](https://php.net/manual/en/features.commandline.webserver.php) que você usará para desenvolvimento. Não se destina a ser usado em um ambiente de produção. 

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

Se essas Perguntas Frequentes não esclareceram a dúvida ou problema encontrado em um ou mais inícios rápidos, informe seu problema ou pergunta no [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). Marque sua pergunta com o microsoft-graph.

Se seu problema tiver relação com o exemplo de código fornecido pelo início rápido, você também poderá apresentar o problema no repositório de exemplos do GitHub. Localize o repositório seguindo o link **Basta dar-me o código de exemplo** na etapa 2 de cada guia de início rápido.
