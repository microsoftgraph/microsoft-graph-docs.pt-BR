---
title: Usar o Explorador do Graph para experimentar as APIs do Microsoft Graph
description: Use o Explorador do Graph para experimentar as APIs do Microsoft Graph no locatário de exemplo padrão para explorar os recursos ou entre em seu próprio locatário e use-o como uma ferramenta de criação de protótipo para atender aos cenários do aplicativo.
localization_priority: Normal
author: bettirosengugi
ms.openlocfilehash: 3f957d940d4dde483324492f1778ede970a5aefc
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013716"
---
# <a name="use-graph-explorer-to-try-microsoft-graph-apis"></a><span data-ttu-id="42b95-103">Usar o Explorador do Graph para experimentar as APIs do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="42b95-103">Use Graph Explorer to try Microsoft Graph APIs</span></span>

<span data-ttu-id="42b95-104">[O Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/) é uma ferramenta de desenvolvedor que permite que você faça convenientemente solicitações da API REST do Microsoft Graph e veja as respostas correspondentes.</span><span class="sxs-lookup"><span data-stu-id="42b95-104">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) is a developer tool that lets you conveniently make Microsoft Graph REST API requests and view corresponding responses.</span></span> <span data-ttu-id="42b95-105">Use o Explorador do Graph para experimentar APIs no exemplo de locatário padrão para explorar as funcionalidades ou entre em seu próprio locatário e use-o como uma ferramenta de criação de protótipo para atender aos cenários do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42b95-105">Use Graph Explorer to try APIs on the default sample tenant to explore capabilities, or sign in to your own tenant and use it as a prototyping tool to fulfill your app scenarios.</span></span> <span data-ttu-id="42b95-106">Essa ferramenta inclui recursos úteis, como trechos de código em C#, Java, JavaScript e Objective C; Integração de cartões adaptáveis e kits de ferramentas do Microsoft Graph; e muito mais.</span><span class="sxs-lookup"><span data-stu-id="42b95-106">This tool includes helpful features such as code snippets in C#, Java, JavaScript, and Objective C; Microsoft Graph Toolkit and adaptive cards integration; and more.</span></span>

<span data-ttu-id="42b95-107">Use o Explorador do Graph para:</span><span class="sxs-lookup"><span data-stu-id="42b95-107">Use Graph Explorer to:</span></span>

- <span data-ttu-id="42b95-108">Faça solicitações da API do Microsoft Graph (GET, POST, PUT, PATCH e DELETE) e veja respostas, incluindo o código de resposta e quaisquer headers e corpos.</span><span class="sxs-lookup"><span data-stu-id="42b95-108">Make Microsoft Graph API requests (GET, POST, PUT, PATCH and DELETE) and see responses including response code and any headers and bodies.</span></span>
- <span data-ttu-id="42b95-109">Consentimento para permissões.</span><span class="sxs-lookup"><span data-stu-id="42b95-109">Consent to permissions.</span></span>
- <span data-ttu-id="42b95-110">Adicione um corpo de solicitação e um header de solicitação à sua consulta.</span><span class="sxs-lookup"><span data-stu-id="42b95-110">Add a request body and request header to your query.</span></span>
- <span data-ttu-id="42b95-111">Exibir e copiar o token de acesso.</span><span class="sxs-lookup"><span data-stu-id="42b95-111">View and copy the access token.</span></span>
- <span data-ttu-id="42b95-112">Veja exemplos de consultas para diferentes serviços no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="42b95-112">View sample queries for different services in Microsoft Graph.</span></span>
- <span data-ttu-id="42b95-113">Exibir, baixar ou excluir as consultas que você fez nos últimos 30 dias.</span><span class="sxs-lookup"><span data-stu-id="42b95-113">View, download, or delete the queries you ran in the last 30 days.</span></span>
- <span data-ttu-id="42b95-114">Exibir e copiar trechos de código de cada consulta que você executar em C#, Java, JavaScript e Objective C.</span><span class="sxs-lookup"><span data-stu-id="42b95-114">View and copy code snippets of each query you run in C#, Java, JavaScript, and Objective C.</span></span>
- <span data-ttu-id="42b95-115">Acesse os componentes e cartões adaptáveis do Microsoft Graph Toolkit para algumas consultas de exemplo.</span><span class="sxs-lookup"><span data-stu-id="42b95-115">Access Microsoft Graph Toolkit components and adaptive cards for some sample queries.</span></span>
- <span data-ttu-id="42b95-116">Compartilhe consultas, incluindo o corpo da solicitação e os headers de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42b95-116">Share queries, including the request body and request headers.</span></span>

<span data-ttu-id="42b95-117">O Explorador do Graph lida com o processo de autenticação para você.</span><span class="sxs-lookup"><span data-stu-id="42b95-117">Graph Explorer handles the authentication process for you.</span></span> <span data-ttu-id="42b95-118">Personalize a experiência repondo a barra lateral e alterando o tema.</span><span class="sxs-lookup"><span data-stu-id="42b95-118">Customize the experience by collapsing the sidebar and changing the theme.</span></span>

## <a name="get-started"></a><span data-ttu-id="42b95-119">Introdução</span><span class="sxs-lookup"><span data-stu-id="42b95-119">Get started</span></span>

<span data-ttu-id="42b95-120">O Graph Explorer é um aplicativo Web hospedado na central de desenvolvedores [do Microsoft Graph.](https://developer.microsoft.com/en-us/graph/graph-explorer)</span><span class="sxs-lookup"><span data-stu-id="42b95-120">Graph Explorer is a web application hosted on the [Microsoft Graph developer center](https://developer.microsoft.com/en-us/graph/graph-explorer).</span></span> <span data-ttu-id="42b95-121">É um projeto de código aberto e damos as boas-vindas às suas contribuições e comentários no [repositório do GitHub.](https://github.com/microsoftgraph/microsoft-graph-explorer-v4)</span><span class="sxs-lookup"><span data-stu-id="42b95-121">It's an open source project,  and we welcome your contributions and feedback in the [GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4).</span></span>

<span data-ttu-id="42b95-122">O Graph Explorer inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="42b95-122">Graph Explorer includes the following elements:</span></span>

1. <span data-ttu-id="42b95-123">Lista drop-down de verbo HTTP</span><span class="sxs-lookup"><span data-stu-id="42b95-123">HTTP verb drop-down list</span></span>
2. <span data-ttu-id="42b95-124">Lista drop-down de versão da API</span><span class="sxs-lookup"><span data-stu-id="42b95-124">API version drop-down list</span></span>
3. <span data-ttu-id="42b95-125">Barra de endereços de consulta de solicitação</span><span class="sxs-lookup"><span data-stu-id="42b95-125">Request query address bar</span></span>
4. <span data-ttu-id="42b95-126">Consulta de exemplo</span><span class="sxs-lookup"><span data-stu-id="42b95-126">Sample query</span></span>
5. <span data-ttu-id="42b95-127">Link de documentação para a consulta de exemplo</span><span class="sxs-lookup"><span data-stu-id="42b95-127">Documentation link for the sample query</span></span>

![Captura de tela da interface do usuário do Graph Explorer](./images/getting-started.png)

### <a name="make-a-get-request-in-graph-explorer"></a><span data-ttu-id="42b95-129">Fazer uma solicitação GET no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="42b95-129">Make a GET request in Graph Explorer</span></span>

<span data-ttu-id="42b95-130">Para executar uma solicitação GET no Explorador do Graph, você não precisa entrar.</span><span class="sxs-lookup"><span data-stu-id="42b95-130">To run a GET request in Graph Explorer, you don’t have to be signed in.</span></span> <span data-ttu-id="42b95-131">Basta clicar em um exemplo de consulta e mostrar dados de exemplo na visualização da resposta.</span><span class="sxs-lookup"><span data-stu-id="42b95-131">Just click a sample query and sample data will show in the response preview.</span></span> 

![Captura de tela de uma solicitação de exemplo no Explorador do Graph](./images/making-a-get-request.png)

<span data-ttu-id="42b95-133">Para fazer uma solicitação:</span><span class="sxs-lookup"><span data-stu-id="42b95-133">To make a request:</span></span>

1. <span data-ttu-id="42b95-134">Selecione uma consulta de exemplo e execute-a.</span><span class="sxs-lookup"><span data-stu-id="42b95-134">Select a sample query and run it.</span></span>
2. <span data-ttu-id="42b95-135">Obter o código de resposta HTTP.</span><span class="sxs-lookup"><span data-stu-id="42b95-135">Get the HTTP response code.</span></span>
3. <span data-ttu-id="42b95-136">Veja a resposta da API do Microsoft Graph com dados de exemplo.</span><span class="sxs-lookup"><span data-stu-id="42b95-136">See the response from the Microsoft Graph API with sample data.</span></span>

<span data-ttu-id="42b95-137">Quando você entrar no Explorador do Graph e clicar na mesma consulta, a resposta será retornada com dados reais do locatário em que você se inscreveu.</span><span class="sxs-lookup"><span data-stu-id="42b95-137">When you sign in to Graph Explorer and click the same query, the response will be returned with real data from the tenant you signed in to.</span></span>

### <a name="running-non-get-requests-in-graph-explorer"></a><span data-ttu-id="42b95-138">Executando solicitações não GET no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="42b95-138">Running non-GET requests in Graph Explorer</span></span>

<span data-ttu-id="42b95-139">Para experimentar solicitações POST, PUT, PATCH e DELETE, entre no Explorador do Graph usando uma conta do Microsoft 365. Pode ser uma conta organizacional para fins de teste ou demonstração.</span><span class="sxs-lookup"><span data-stu-id="42b95-139">To try POST, PUT, PATCH and DELETE requests, sign in to Graph Explorer using a Microsoft 365 account.This can be an organizational account for testing or demonstration purpose.</span></span> <span data-ttu-id="42b95-140">Para obter um exemplo gratuito de assinatura de desenvolvedor do Microsoft 365 E5, juntamente com ferramentas e outros recursos para ajudá-lo a criar soluções para a plataforma Microsoft 365, participe do Programa para Desenvolvedores [do Microsoft 365.](https://developer.microsoft.com/microsoft-365/dev-program)</span><span class="sxs-lookup"><span data-stu-id="42b95-140">To get a free sample Microsoft 365 E5 developer subscription, along with tools and other resources to help you build solutions for the Microsoft 365 platform, join the [Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> 

>[!IMPORTANT]
><span data-ttu-id="42b95-141">Se você optar por entrar usando sua conta organizacional, executar uma solicitação não GET pode afetar os dados no locatário.</span><span class="sxs-lookup"><span data-stu-id="42b95-141">If you choose to sign in using your organizational account, running a non-GET request can affect the data in the tenant.</span></span>

<span data-ttu-id="42b95-142">Por exemplo, para executar uma solicitação POST, selecione POST na lista drop-down para o verbo HTTP e adicione um corpo de solicitação e cabeçalhos de solicitação conforme apropriado.</span><span class="sxs-lookup"><span data-stu-id="42b95-142">For example, to run a POST request, select POST in the drop-down list for the HTTP verb, and add a request body and request headers as appropriate.</span></span>

![Captura de tela de uma solicitação POST no Explorador do Graph](./images/making-a-post-request.png)

1. <span data-ttu-id="42b95-144">Selecione uma consulta de exemplo POST.</span><span class="sxs-lookup"><span data-stu-id="42b95-144">Select a POST sample query.</span></span>
2. <span data-ttu-id="42b95-145">Atualizar **corpo da solicitação;** por exemplo, dê um nome ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42b95-145">Update **Request body**; for example, give the application a name.</span></span>
3. <span data-ttu-id="42b95-146">Clique **em Executar consulta**.</span><span class="sxs-lookup"><span data-stu-id="42b95-146">Click **Run query**.</span></span>
4. <span data-ttu-id="42b95-147">Veja a resposta da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="42b95-147">See the response from the Microsoft Graph API.</span></span>

<span data-ttu-id="42b95-148">Para exibir a resposta em um formato diferente do JSON padrão, escolha a guia Solicitação de **headers** no painel de solicitação, defina o par chave/valor e clique em **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="42b95-148">To view the response in a format other than the default JSON, choose the **Request headers** tab in the request pane, define the key/value pair, and click **Add**.</span></span>

![Screenshot that shows the Request headers tab in Graph Explorer](./images/adding-key-value-pairs.png)

## <a name="next-steps"></a><span data-ttu-id="42b95-150">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="42b95-150">Next steps</span></span>

- <span data-ttu-id="42b95-151">Visite [o Explorador do Graph.](https://developer.microsoft.com/graph/graph-explorer/)</span><span class="sxs-lookup"><span data-stu-id="42b95-151">Visit [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/).</span></span>
- <span data-ttu-id="42b95-152">Saiba mais sobre os [recursos do Graph Explorer.](./graph-explorer-features.md)</span><span class="sxs-lookup"><span data-stu-id="42b95-152">Learn more about [Graph Explorer features](./graph-explorer-features.md).</span></span>
- <span data-ttu-id="42b95-153">Contribuir ou fornecer comentários no [repositório do GitHub.](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose)</span><span class="sxs-lookup"><span data-stu-id="42b95-153">Contribute or provide feedback in the [GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).</span></span>
