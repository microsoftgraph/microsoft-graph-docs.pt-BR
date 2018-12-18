---
title: Perguntas frequentes do início rápido do Microsoft Graph
description: Estas perguntas frequentes respondem dúvidas relacionadas aos Inícios Rápidos do Microsoft Graph.
author: jasonjoh
ms.author: jasonjoh
ms.date: 12/13/2018
ms.openlocfilehash: 55630e8fbdbccd8355d2b23e4c839d2ccec2b7d3
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283637"
---
# <a name="microsoft-graph-quick-start-faq"></a><span data-ttu-id="9f653-103">Perguntas frequentes do início rápido do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9f653-103">Microsoft Graph quick start FAQ</span></span>

<span data-ttu-id="9f653-104">Estas perguntas frequentes respondem dúvidas relacionadas aos [Inícios Rápidos do Microsoft Graph](https://developer.microsoft.com/graph/quick-start).</span><span class="sxs-lookup"><span data-stu-id="9f653-104">This FAQ answers questions related to the [Microsoft Graph Quick Starts](https://developer.microsoft.com/graph/quick-start).</span></span>

## <a name="general-design"></a><span data-ttu-id="9f653-105">Design geral</span><span class="sxs-lookup"><span data-stu-id="9f653-105">General design</span></span>

<span data-ttu-id="9f653-106">Os exemplos de início rápido mostram como acessar os recursos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9f653-106">The quick start samples show you how to access the power of Microsoft Graph.</span></span> <span data-ttu-id="9f653-107">Esses exemplos acessam dois serviços com uma autenticação: conta da Microsoft e o Outlook.</span><span class="sxs-lookup"><span data-stu-id="9f653-107">These samples access two services with one authentication: Microsoft account and Outlook.</span></span> <span data-ttu-id="9f653-108">Cada início rápido acessa informações de perfis de usuários com uma conta Microsoft e exibe eventos no calendário.</span><span class="sxs-lookup"><span data-stu-id="9f653-108">Each quick start accesses information from Microsoft account users' profiles and displays events from their calendar.</span></span>

<span data-ttu-id="9f653-109">Os inícios rápidos envolvem quatro etapas:</span><span class="sxs-lookup"><span data-stu-id="9f653-109">The quick starts involve four steps:</span></span>

- <span data-ttu-id="9f653-110">Selecione sua plataforma</span><span class="sxs-lookup"><span data-stu-id="9f653-110">Select your platform</span></span>
- <span data-ttu-id="9f653-111">Obter sua ID de aplicativo (ID do cliente)</span><span class="sxs-lookup"><span data-stu-id="9f653-111">Get your app ID (client ID)</span></span>
- <span data-ttu-id="9f653-112">Criar o exemplo</span><span class="sxs-lookup"><span data-stu-id="9f653-112">Build the sample</span></span>
- <span data-ttu-id="9f653-113">Entrar e exibir eventos no calendário</span><span class="sxs-lookup"><span data-stu-id="9f653-113">Sign in, and view events on your calendar</span></span>

<span data-ttu-id="9f653-114">Quando você completar o início rápido, você possui um aplicativo pronto para ser executado.</span><span class="sxs-lookup"><span data-stu-id="9f653-114">When you complete the quick start, you have an app that's ready to run.</span></span>

## <a name="general-quick-start-sample-questions"></a><span data-ttu-id="9f653-115">Exemplos de perguntas do início rápido gerais</span><span class="sxs-lookup"><span data-stu-id="9f653-115">General quick start sample questions</span></span>

<!-- markdownlint-disable MD026 -->

<span data-ttu-id="9f653-116">Esta seção responde perguntas sobre o conteúdo dos exemplos de início rápido.</span><span class="sxs-lookup"><span data-stu-id="9f653-116">This section answers questions about the organization and contents of the quick start samples.</span></span>

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a><span data-ttu-id="9f653-117">Posso obter o código de início rápido sem fazer o download através da página de início rápido?</span><span class="sxs-lookup"><span data-stu-id="9f653-117">Can I get the quick start code without downloading through the quick start page?</span></span>

<span data-ttu-id="9f653-118">Com certeza!</span><span class="sxs-lookup"><span data-stu-id="9f653-118">Absolutely.</span></span> <span data-ttu-id="9f653-119">Todo download de início rápido é baseado em um [tutorial do Microsoft Graph](tutorials.md), portanto, você terá duas outras opções para obter o mesmo código-fonte:</span><span class="sxs-lookup"><span data-stu-id="9f653-119">Each quick start download is based on a [Microsoft Graph tutorial](tutorials.md), so you have two other options to get the same source code:</span></span>

- <span data-ttu-id="9f653-120">Crie o código por conta própria seguindo tutorial passo a passo.</span><span class="sxs-lookup"><span data-stu-id="9f653-120">Build the code yourself by following the step-by-step tutorial.</span></span>
- <span data-ttu-id="9f653-121">Faça o download do projeto concluído a partir do repositório GitHub correspondente e siga as instruções no README para configurar e executar a amostra.</span><span class="sxs-lookup"><span data-stu-id="9f653-121">Download the completed project from the corresponding GitHub repository and follow the instructions in the README to configure and run the sample.</span></span>

> <span data-ttu-id="9f653-122">**Observação:** Estamos no processo de gerar tutoriais para cada uma das plataformas que atualmente têm um início rápido.</span><span class="sxs-lookup"><span data-stu-id="9f653-122">**Note:** We are in the process of generating tutorials for each of the platforms that currently have a quick start.</span></span> <span data-ttu-id="9f653-123">Algumas com início rápido não têm o tutoriais correspondentes.</span><span class="sxs-lookup"><span data-stu-id="9f653-123">Some of the quick starts do not have corresponding tutorials yet.</span></span>

#### <a name="tutorials-and-github-repositories"></a><span data-ttu-id="9f653-124">Tutoriais e repositórios do GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-124">Tutorials and GitHub repositories</span></span>

<span data-ttu-id="9f653-125">A tabela a seguir lista o tutorial correspondente e o repositório do GitHub para cada amostra de início rápido.</span><span class="sxs-lookup"><span data-stu-id="9f653-125">The following table lists the corresponding tutorial and GitHub repository for each quick start sample.</span></span>

| <span data-ttu-id="9f653-126">Início Rápido</span><span class="sxs-lookup"><span data-stu-id="9f653-126">Quick start</span></span> | <span data-ttu-id="9f653-127">Tutorial</span><span class="sxs-lookup"><span data-stu-id="9f653-127">Tutorial</span></span> | <span data-ttu-id="9f653-128">Repositório do GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-128">PnP-Transformation GitHub repository</span></span> |
|-------------|----------|-------------------|
| <span data-ttu-id="9f653-129">Android</span><span class="sxs-lookup"><span data-stu-id="9f653-129">Android</span></span> | <span data-ttu-id="9f653-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f653-130">None</span></span> | [<span data-ttu-id="9f653-131">GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-131">GitHub Help</span></span>](https://github.com/microsoftgraph/android-java-connect-sample) |
| <span data-ttu-id="9f653-132">Angular</span><span class="sxs-lookup"><span data-stu-id="9f653-132">Angular</span></span> | [<span data-ttu-id="9f653-133">Tutorial</span><span class="sxs-lookup"><span data-stu-id="9f653-133">Tutorial</span></span>](/graph/tutorials/angular) | [<span data-ttu-id="9f653-134">GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-134">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| <span data-ttu-id="9f653-135">ASP.NET MVC</span><span class="sxs-lookup"><span data-stu-id="9f653-135">ASP.NET MVC</span></span> | [<span data-ttu-id="9f653-136">Tutorial</span><span class="sxs-lookup"><span data-stu-id="9f653-136">Tutorial</span></span>](/graph/tutorials/aspnet) | [<span data-ttu-id="9f653-137">GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-137">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| <span data-ttu-id="9f653-138">iOS (Swift)</span><span class="sxs-lookup"><span data-stu-id="9f653-138">iOS (Swift)</span></span> | <span data-ttu-id="9f653-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f653-139">None</span></span> | [<span data-ttu-id="9f653-140">GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-140">GitHub Help</span></span>](https://github.com/microsoftgraph/ios-swift-connect-sample) |
| <span data-ttu-id="9f653-141">iOS (Objective-C)</span><span class="sxs-lookup"><span data-stu-id="9f653-141">iOS Objective-C</span></span> | <span data-ttu-id="9f653-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f653-142">None</span></span> | [<span data-ttu-id="9f653-143">GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-143">GitHub Help</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample) |
| <span data-ttu-id="9f653-144">Node.js</span><span class="sxs-lookup"><span data-stu-id="9f653-144">Node.js</span></span> | [<span data-ttu-id="9f653-145">Tutorial</span><span class="sxs-lookup"><span data-stu-id="9f653-145">Tutorial</span></span>](/graph/tutorials/node) | [<span data-ttu-id="9f653-146">GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-146">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| <span data-ttu-id="9f653-147">PHP</span><span class="sxs-lookup"><span data-stu-id="9f653-147">PHP</span></span> | [<span data-ttu-id="9f653-148">Tutorial</span><span class="sxs-lookup"><span data-stu-id="9f653-148">Tutorial</span></span>](/graph/tutorials/php) | [<span data-ttu-id="9f653-149">GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-149">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| <span data-ttu-id="9f653-150">Python</span><span class="sxs-lookup"><span data-stu-id="9f653-150">Python</span></span> | [<span data-ttu-id="9f653-151">Tutorial</span><span class="sxs-lookup"><span data-stu-id="9f653-151">Tutorial</span></span>](/graph/tutorials/python) | [<span data-ttu-id="9f653-152">GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-152">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| <span data-ttu-id="9f653-153">Ruby</span><span class="sxs-lookup"><span data-stu-id="9f653-153">Ruby</span></span> | [<span data-ttu-id="9f653-154">Tutorial</span><span class="sxs-lookup"><span data-stu-id="9f653-154">Tutorial</span></span>](/graph/tutorials/ruby) | [<span data-ttu-id="9f653-155">GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-155">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| <span data-ttu-id="9f653-156">UWP</span><span class="sxs-lookup"><span data-stu-id="9f653-156">UWP</span></span> | [<span data-ttu-id="9f653-157">Tutorial</span><span class="sxs-lookup"><span data-stu-id="9f653-157">Tutorial</span></span>](/graph/tutorials/uwp) | [<span data-ttu-id="9f653-158">GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-158">GitHub Help</span></span>](https://github.com/microsoftgraph/msgraph-training-uwp) |
| <span data-ttu-id="9f653-159">Xamarin</span><span class="sxs-lookup"><span data-stu-id="9f653-159">Xamarin</span></span> | <span data-ttu-id="9f653-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f653-160">None</span></span> | [<span data-ttu-id="9f653-161">GitHub</span><span class="sxs-lookup"><span data-stu-id="9f653-161">GitHub Help</span></span>](https://github.com/microsoftgraph/uwp-csharp-connect-sample) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a><span data-ttu-id="9f653-162">Por que nenhum dos exemplos de início rápido mostra casos de uso de autenticação avançados?</span><span class="sxs-lookup"><span data-stu-id="9f653-162">Why don't any of the quick start samples show advanced authentication use cases?</span></span>

<span data-ttu-id="9f653-163">Os exemplos de início rápido oferecem uma introdução à autenticação e às chamadas à API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9f653-163">The quick start samples give you an introduction to authentication and Microsoft Graph API calls.</span></span> <span data-ttu-id="9f653-164">Saiba mais sobre outros fluxos de autenticação na documentação [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios).</span><span class="sxs-lookup"><span data-stu-id="9f653-164">You can learn more about other authentication flows in the [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios) documentation.</span></span>

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a><span data-ttu-id="9f653-165">E se eu tiver um erro inesperado ou um problema com um início rápido?</span><span class="sxs-lookup"><span data-stu-id="9f653-165">What if I run into an unexpected error or problem with a quick start?</span></span>

<span data-ttu-id="9f653-166">Se você tiver problemas para o início rápido funcionar corretamente, abra um problema no repositório do GitHub correspondente.</span><span class="sxs-lookup"><span data-stu-id="9f653-166">If you have trouble getting the quick start to work properly, please open an issue on the corresponding GitHub repository.</span></span>

## <a name="didnt-find-what-you-need"></a><span data-ttu-id="9f653-167">Não consegue encontrar o que precisa?</span><span class="sxs-lookup"><span data-stu-id="9f653-167">Didn't find what you need?</span></span>

<span data-ttu-id="9f653-168">Se essas Perguntas Frequentes não esclareceram a dúvida ou problema encontrado em um ou mais inícios rápidos, por favor nos avise usando a seção **Feedback** abaixo.</span><span class="sxs-lookup"><span data-stu-id="9f653-168">If this FAQ didn't address a question or problem you encountered with one or more of the quick starts, please let us know using the **Feedback** section below.</span></span>
