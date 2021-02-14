---
title: Perguntas frequentes do início rápido do Microsoft Graph
description: Estas perguntas frequentes respondem dúvidas relacionadas aos Inícios Rápidos do Microsoft Graph.
author: jasonjoh
localization_priority: Normal
ms.openlocfilehash: 71cd53990d76456d20bdcf21fcf7a92cbde16ff2
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239601"
---
# <a name="microsoft-graph-quick-start-faq"></a>Perguntas frequentes do início rápido do Microsoft Graph

Estas perguntas frequentes respondem dúvidas relacionadas aos [Inícios Rápidos do Microsoft Graph](https://developer.microsoft.com/graph/quick-start).

## <a name="general-design"></a>Design geral

Os exemplos de início rápido mostram como acessar os recursos do Microsoft Graph. Esses exemplos acessam dois serviços com uma autenticação: conta da Microsoft e o Outlook. Cada início rápido acessa informações de perfis de usuários com uma conta Microsoft e exibe eventos no calendário.

Os inícios rápidos envolvem quatro etapas:

- Selecione sua plataforma
- Obter sua ID de aplicativo (ID do cliente)
- Criar o exemplo
- Entrar e exibir eventos no calendário

Quando você completar o início rápido, você possui um aplicativo pronto para ser executado.

## <a name="prerequisites"></a>Pré-requisitos

Todos os exemplos de início rápido exigem acesso a uma conta pessoal da Microsoft com uma caixa de correio no Outlook.com ou a uma conta de trabalho ou de estudante da Microsoft com uma caixa de correio do Exchange Online. Se você não tiver uma conta da Microsoft, há algumas opções para obter uma conta gratuita:

- Você pode [se inscrever para uma nova conta pessoal da Microsoft.](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1)
- Você pode [se inscrever no Programa para Desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program) para obter uma assinatura gratuita do Microsoft 365.

## <a name="general-quick-start-sample-questions"></a>Exemplos de perguntas do início rápido gerais

<!-- markdownlint-disable MD026 -->

Esta seção responde perguntas sobre o conteúdo dos exemplos de início rápido.

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a>Posso obter o código de início rápido sem fazer o download através da página de início rápido?

Com certeza! Todo download de início rápido é baseado em um [tutorial do Microsoft Graph](tutorials.yml), portanto, você terá duas outras opções para obter o mesmo código-fonte:

- Crie o código por conta própria seguindo tutorial passo a passo.
- Faça o download do projeto concluído a partir do repositório GitHub correspondente e siga as instruções no README para configurar e executar a amostra.

#### <a name="tutorials-and-github-repositories"></a>Tutoriais e repositórios do GitHub

A tabela a seguir lista o tutorial correspondente e o repositório do GitHub para cada amostra de início rápido.

| Início Rápido | Tutorial | Repositório do GitHub |
|-------------|----------|-------------------|
| Android | [Tutorial](/graph/tutorials/android) | [GitHub](https://github.com/microsoftgraph/msgraph-training-android) |
| Angular | [Tutorial](/graph/tutorials/angular) | [GitHub](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| ASP.NET MVC | [Tutorial](/learn/modules/msgraph-build-aspnetmvc-apps) | [GitHub](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| iOS (Swift) | [Tutorial](/graph/tutorials/ios-swift) | [GitHub](https://github.com/microsoftgraph/msgraph-training-ios-swift) |
| iOS (Objective-C) | [Tutorial](/graph/tutorials/ios-objectivec) | [GitHub](https://github.com/microsoftgraph/msgraph-training-ios-objectivec) |
| Node.js | [Tutorial](/graph/tutorials/node) | [GitHub](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| PHP | [Tutorial](/graph/tutorials/php) | [GitHub](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| Python | [Tutorial](/graph/tutorials/python) | [GitHub](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| React | [Tutorial](/graph/tutorials/react) | [GitHub](https://github.com/microsoftgraph/msgraph-training-reactspa) |
| Ruby | [Tutorial](/graph/tutorials/ruby) | [GitHub](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| UWP | [Tutorial](/graph/tutorials/uwp) | [GitHub](https://github.com/microsoftgraph/msgraph-training-uwp) |
| Xamarin | [Tutorial](/graph/tutorials/xamarin) | [GitHub](https://github.com/microsoftgraph/msgraph-training-xamarin) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>Por que nenhum dos exemplos de início rápido mostra casos de uso de autenticação avançados?

Os exemplos de início rápido oferecem uma introdução à autenticação e às chamadas à API do Microsoft Graph. Saiba mais sobre outros fluxos de autenticação na documentação [Azure Active Directory](/azure/active-directory/develop/authentication-scenarios).

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a>E se eu tiver um erro inesperado ou um problema com um início rápido?

Se você tiver problemas para o início rápido funcionar corretamente, abra um problema no repositório do GitHub correspondente.

## <a name="known-issues"></a>Problemas conhecidos

### <a name="aspnet-quick-start-displays-an-error-when-running-it-cannot-find-a-part-of-the-path-graph-tutorialgraph-tutorialbinroslyncscexe"></a>O início rápido do ASP.NET exibe um erro ao executá-lo: Não é possível localizar uma parte do caminho '[...]\Graph Tutorial\graph-tutorial\bin\roslyn\csc.exe'.

Isso é causado por um [problema com o Visual Studio e o compilador Roslyn](https://github.com/dotnet/roslyn/issues/15556). Uma das opções a seguir deve resolver o erro.

- Descarregar/recarregar o projeto no Gerenciador de Soluções
- Limpar/Reconstruir a solução
- Atualizar pacotes do NuGet

### <a name="im-getting-aadsts50011-the-reply-url-specified-in-the-request-does-not-match-the-reply-urls-configured-for-the-application-when-running-a-quick-start"></a>Estou recebendo "AADSTS50011: O URL de resposta especificado na solicitação não corresponde aos URLs de resposta configurados para o aplicativo" ao executar um início rápido.

Isso indica um problema com o registro do aplicativo para o início rápido. Quando você faz o download de um início rápido da página [Início Rápido do Microsoft Graph](https://developer.microsoft.com/graph/quick-start), nós criamos o registro do aplicativo para você e configuramos um URL de resposta (também conhecido como URL de redirecionamento) que corresponde ao URL padrão usado pelo projeto de amostra. Se você alterar o URL, o registro do aplicativo não mais corresponderá e poderá causar esse erro. Para resolver esse erro, consulte o arquivo README.md incluído no projeto de início rápido para obter instruções sobre como criar um registro de aplicativo e configurá-lo no código de amostra.

### <a name="after-signing-in-im-told-i-need-admin-approval"></a>Depois de entrar, estou informado de que preciso da aprovação do administrador.

Depois de entrar em um dos exemplos de início rápido, você poderá ver uma mensagem informando que precisa de aprovação do administrador **"Xxx** Tutorial precisa de permissão para acessar recursos em sua organização que somente um administrador pode conceder. Peça ao administrador para conceder permissão a este aplicativo antes de usá-lo." Isso não é um bug com o exemplo! Nenhum dos inícios rápidos solicita escopos de permissão do Graph *que, por padrão,* exigem consentimento do administrador. Os administradores de locatários podem desabilitar sua capacidade de consentir com escopos de permissões do Graph para todos os aplicativos que eles não aprovaram. Nesse caso, você verá esse erro.

Você precisará trabalhar com seus administradores para obter aprovação, usar uma conta pessoal da Microsoft (Outlook.com) ou usar um locatário do Microsoft 365 de teste com o Exchange Online.

## <a name="didnt-find-what-you-need"></a>Não consegue encontrar o que precisa?

Se essas Perguntas Frequentes não esclareceram a dúvida ou problema encontrado em um ou mais inícios rápidos, por favor nos avise usando a seção **Feedback** abaixo.
