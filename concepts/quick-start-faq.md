---
title: Perguntas frequentes do início rápido do Microsoft Graph
description: Estas perguntas frequentes respondem dúvidas relacionadas aos Inícios Rápidos do Microsoft Graph.
author: jasonjoh
ms.author: jasonjoh
localization_priority: Normal
ms.openlocfilehash: 9b260a29512595fe39d556a57d8e30d86ae06ca6
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916911"
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

## <a name="general-quick-start-sample-questions"></a>Exemplos de perguntas do início rápido gerais

<!-- markdownlint-disable MD026 -->

Esta seção responde perguntas sobre o conteúdo dos exemplos de início rápido.

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a>Posso obter o código de início rápido sem fazer o download através da página de início rápido?

Com certeza! Todo download de início rápido é baseado em um [tutorial do Microsoft Graph](tutorials.yml), portanto, você terá duas outras opções para obter o mesmo código-fonte:

- Crie o código por conta própria seguindo tutorial passo a passo.
- Faça o download do projeto concluído a partir do repositório GitHub correspondente e siga as instruções no README para configurar e executar a amostra.

> [!NOTE]
> Estamos no processo de criação de tutoriais para cada uma das plataformas que atualmente têm um início rápido. Algumas com início rápido não têm o tutoriais correspondentes.

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

## <a name="didnt-find-what-you-need"></a>Não consegue encontrar o que precisa?

Se essas Perguntas Frequentes não esclareceram a dúvida ou problema encontrado em um ou mais inícios rápidos, por favor nos avise usando a seção **Feedback** abaixo.
