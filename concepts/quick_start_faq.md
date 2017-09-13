# <a name="microsoft-graph-quick-start-faq"></a>Perguntas frequentes do Início Rápido do Microsoft Graph

Essas Perguntas Frequentes abordam dúvidas e problemas que podem ocorrer ao percorrer um dos [Inícios Rápidos do Microsoft Graph](https://developer.microsoft.com/en-us/graph/quick-start).

## <a name="what-do-the-quick-starts-do"></a>O que os inícios rápidos fazem?

Independentemente da plataforma que você escolher, os inícios rápidos fazem o seguinte:

- Registram um novo aplicativo para você no [Portal de Registro do Aplicativo](https://apps.dev.microsoft.com). Isso ocorre porque pedimos que você entre com uma conta da Microsoft ao **Obter uma ID de aplicativo**. Se seu aplicativo exigir um segredo do aplicativo, o início rápido criará um para você. 
- Baixa uma cópia do código de exemplo armazenado em um repositório do GitHub. Você pode ver esses repositórios na [organização MicrosoftGraph](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect) no GitHub.
- Insere a nova ID de aplicativo, e, onde necessário, o segredo do aplicativo, em um arquivo de configuração dentro do código de exemplo armazenado no repositório do GitHub. Não desejamos enviar informações confidenciais em uma solicitação HTTP, portanto, pedimos que você copie o segredo do aplicativo após criar o novo aplicativo e, em seguida, copie-o para um formulário no início rápido antes de baixar uma cópia do exemplo.
- Solicita que você baixe o exemplo totalmente configurado. Depois de baixar e descompactar o código de exemplo, você terá um aplicativo Web ou de cliente que deverá ser executado, supondo que você tenha instalado os pré-requisitos especificados (IDEs, estruturas da Web e assim por diante) em seu ambiente de desenvolvimento.


## <a name="why-wont-my--aspnet-uwp-or-xamarin-project-build"></a>Por que meu projeto ASP.NET, UWP ou Xamarin não é compilado?

Se um exemplo que usa bibliotecas .NET falhar ao compilar no Visual Studio, um ou mais dos projetos podem estar sendo executados no limite do comprimento do caminho do Windows que é de 260 caracteres. Principalmente as soluções Xamarin estão sujeitas a isso, especialmente projetos do Android em soluções Xamarin. Tente mover a solução para um local no ou próxima ao diretório raiz. 

## <a name="if-a-web-platform-quick-start-provides-rest-and-sdk-samples-can-i-run-them-both-at-the-same-time"></a>Se o início rápido de uma plataforma Web fornecer exemplos de REST e SDK, posso executá-los ao mesmo tempo?

Sim, você pode executar os dois exemplos ao mesmo tempo. Basta verificar se um deles não está sendo executado na porta padrão. Isso significa que, quando você inicia o servidor Web de teste, será necessário especificar um número de porta para, pelo menos, uma versão do exemplo.

## <a name="i-didnt-get-an-email-and-i-see-no-errors-or-exceptions-why-didnt-this-work"></a>Eu não recebi um email e não vejo erros ou exceções. Por que isso não funcionou?

Se parecer que o exemplo enviou um email, mas ele não for exibido em sua Caixa de Entrada, verifique a pasta de lixo eletrônico ou spam. Se você estiver enviando a mensagem de um locatário de teste, a mensagem poderá ser sinalizada como spam.

## <a name="i-get-an-error-when-i-try-to-sign-in-and-authorize-the-sample-app-what-steps-can-i-take-to-fix-this"></a>Recebo um erro quando tento entrar e autorizar o aplicativo de teste. Quais etapas posso seguir para corrigir isso? 

Primeiro, tente executar o aplicativo de exemplo em uma janela InPrivate ou Incognito. Às vezes, as configurações de cache do navegador da Web podem fazer com que a etapa de autorização falhe, especialmente se você entrar com várias contas da Microsoft. Se isso não funcionar, entre em contato conosco em [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). Lembre-se de marcar sua pergunta com microsoft-graph e copie as informações de erro para a pergunta.

## <a name="why-do-some-quick-starts-include-an-app-secret-and-others-dont"></a>Por que alguns inícios rápidos incluem um segredo do aplicativo e outros não?

Os aplicativos Web do servidor que precisam fazer chamadas seguras para a API do Microsoft Graph exigem segredos do aplicativo. Isso ocorre porque os inícios rápidos do ASP.NET MVC, Node.js, PHP e Ruby fornecem um segredo do aplicativo.

## <a name="why-doesnt-the-angular-quick-start-give-me-an-app-secret-when-all-the-other-web-platform-quick-starts-do"></a>Por que o início rápido do Angular não me oferece um segredo do aplicativo quando todos os demais inícios rápidos da plataforma Web oferecem?

O segredo do aplicativo só é necessário para aplicativos Web do servidor.

## <a name="why-does-my-quick-start-contain-a-readme-file"></a>Por que meu início rápido contém um arquivo Leiame?

Cada início rápido registra um novo aplicativo e cria um arquivo zip que contém o conteúdo de um repositório do GitHub. Ele atualiza os arquivos no repositório para que você não precise configurar o aplicativo de exemplo no repositório. Você pode ver esses repositórios na [organização do MicrosoftGraph](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect) no GitHub.

Fique à vontade para examinar o repositório associado a cada início rápido, problemas de arquivo e/ou seguir as instruções no Leiame para registrar seu próprio aplicativo. Siga o link **Basta dar-me o código de exemplo** na etapa 2 de cada guia de início rápido para ir para o repositório associado.

## <a name="why-did-the-sample-give-me-an-image-containing-a-thought-bubble"></a>Por que o exemplo disponibilizou uma imagem que contém um balão de pensamento?

A maioria dos exemplos fornecidos pelo inícios rápidos pegam sua imagem do perfil e carregam-a na pasta raiz de sua conta do OneDrive. Se você entrar com uma conta da Microsoft (live.com, hotmail.com), atualmente, o Microsoft Graph não consegue buscar sua imagem do perfil e, portanto, retornamos à imagem do balão de pensamento. O exemplo também usará essa imagem se sua conta não tiver uma imagem de perfil.

## <a name="why-do-you-provide-a-manage-your-apphttpsappsdevmicrosoftcom-link-after-i-get-an-app-id"></a>Por que você disponibiliza um link **[Gerenciar seu aplicativo](https://apps.dev.microsoft.com)** após obter uma ID de aplicativo?

Oferecemos esse link porque a etapa da ID de aplicativo registra um novo aplicativo para você no [Portal de Registro do Aplicativo](https://apps.dev.microsoft.com). Fornecemos o link para que você possa exibir as configurações deste aplicativo, excluir o aplicativo ou até atualizar as configurações do aplicativo depois de executar o exemplo. 

## <a name="didnt-find-what-you-need"></a>Não consegue encontrar o que precisa?

Se essas Perguntas Frequentes não esclareceram sua dúvida ou trataram de um problema encontrado em um ou mais inícios rápidos, informe seu problema ou pergunta no [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). 

Se seu problema tiver relação com o exemplo de código fornecido pelo início rápido, você também poderá apresentar o problema no repositório de exemplos do GitHub. Localize o repositório seguindo o link **Basta dar-me o código de exemplo** na etapa 2 de cada guia de início rápido.
