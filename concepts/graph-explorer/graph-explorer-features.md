---
title: Trabalhar com o Explorador do Graph
description: Saiba como usar alguns dos recursos importantes no Explorador do Graph.
localization_priority: Normal
author: bettirosengugi
ms.openlocfilehash: b4c669ae6983efe2082b623c3de5b019a049311d
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072384"
---
# <a name="working-with-graph-explorer"></a><span data-ttu-id="69ffc-103">Trabalhar com o Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="69ffc-103">Working with Graph Explorer</span></span>

<span data-ttu-id="69ffc-104">[O Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/) é uma ferramenta de desenvolvedor que permite que você faça convenientemente solicitações da API REST do Microsoft Graph e veja as respostas correspondentes.</span><span class="sxs-lookup"><span data-stu-id="69ffc-104">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) is a developer tool that lets you conveniently make Microsoft Graph REST API requests and view corresponding responses.</span></span> <span data-ttu-id="69ffc-105">Este artigo descreve como usar alguns dos recursos importantes no Explorador do Graph.</span><span class="sxs-lookup"><span data-stu-id="69ffc-105">This article describes how to use some of the important features in Graph Explorer.</span></span>

## <a name="consent-to-permissions"></a><span data-ttu-id="69ffc-106">Consentimento para permissões</span><span class="sxs-lookup"><span data-stu-id="69ffc-106">Consent to permissions</span></span>

<span data-ttu-id="69ffc-107">O usuário ou administrador deve conceder ao Explorador do Graph as permissões corretas por meio de um processo de consentimento para acessar dados no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="69ffc-107">The user or administrator must grant Graph Explorer the correct permissions via a consent process to access data in Microsoft Graph.</span></span> <span data-ttu-id="69ffc-108">Consentir com permissões no Explorador  do Graph por  meio da guia Modificar permissões ou da opção Selecionar permissões na engrenagem de configurações ao lado do seu perfil quando você estiver entrar.</span><span class="sxs-lookup"><span data-stu-id="69ffc-108">Consent to permissions in Graph Explorer either via the **Modify permissions** tab or the **Select permissions** option in the settings gear next to your profile when you’re signed in.</span></span> <span data-ttu-id="69ffc-109">A **guia Modificar permissões** lista todas as permissões de que você precisa para executar a consulta na barra de endereços.</span><span class="sxs-lookup"><span data-stu-id="69ffc-109">The **Modify permissions** tab lists all permissions you need to run the query in the address bar.</span></span> 

<span data-ttu-id="69ffc-110">Para consentir com permissões:</span><span class="sxs-lookup"><span data-stu-id="69ffc-110">To consent to permissions:</span></span>

1.  <span data-ttu-id="69ffc-111">Selecione uma consulta de exemplo e execute-a.</span><span class="sxs-lookup"><span data-stu-id="69ffc-111">Select a sample query and run it.</span></span>
2.  <span data-ttu-id="69ffc-112">Selecione a **guia Modificar permissões.**</span><span class="sxs-lookup"><span data-stu-id="69ffc-112">Select the **Modify permissions** tab.</span></span>
3.  <span data-ttu-id="69ffc-113">Consulte a lista de permissões necessárias para executar a consulta.</span><span class="sxs-lookup"><span data-stu-id="69ffc-113">See the list of permissions required to run the query.</span></span>
4.  <span data-ttu-id="69ffc-114">Selecione o botão de consentimento ao lado da permissão que você deseja consentir.</span><span class="sxs-lookup"><span data-stu-id="69ffc-114">Select the consent button next to the permission you want to consent to.</span></span> 

![Captura de tela do Explorador do Graph com as etapas de consentimento para permissões realçadas](./images/modify-permissions.png)

<span data-ttu-id="69ffc-116">O **recurso Modificar permissões** está atualmente em visualização, e algumas consultas podem estar sem permissões.</span><span class="sxs-lookup"><span data-stu-id="69ffc-116">The **Modify  permissions** feature is currently in preview, and some queries might be missing permissions.</span></span> <span data-ttu-id="69ffc-117">Se as permissões não estão disponíveis  para uma consulta, a opção Selecionar permissões na engrenagem de configurações ao lado do seu perfil contém a lista de todas as permissões disponíveis:</span><span class="sxs-lookup"><span data-stu-id="69ffc-117">If permissions are missing for a query, the **Select permissions** option in the settings gear next to your profile contains the list of all available permissions:</span></span>

1.  <span data-ttu-id="69ffc-118">Vá para a engrenagem de configurações e clique **na opção Selecionar** permissões.</span><span class="sxs-lookup"><span data-stu-id="69ffc-118">Go the settings gear and click the **Select permissions** option.</span></span> <span data-ttu-id="69ffc-119">Essa opção contém a lista de todas as permissões disponíveis.</span><span class="sxs-lookup"><span data-stu-id="69ffc-119">This option contains the list of all available permissions.</span></span>
2.  <span data-ttu-id="69ffc-120">Na lista de todas as permissões, consenta com as que você deseja.</span><span class="sxs-lookup"><span data-stu-id="69ffc-120">From the list of all the permissions, consent to the ones you want.</span></span>

![Captura de tela do Explorador do Graph com a opção Selecionar permissões realçada](./images/select-permissions.png)

## <a name="get-an-access-or-authentication-token"></a><span data-ttu-id="69ffc-122">Obter um token de acesso ou autenticação</span><span class="sxs-lookup"><span data-stu-id="69ffc-122">Get an access or authentication token</span></span>

<span data-ttu-id="69ffc-123">O Explorador do Graph inclui uma **guia de token** do Access que mostra seu token de acesso quando você está entrar.</span><span class="sxs-lookup"><span data-stu-id="69ffc-123">Graph Explorer includes an **Access token** tab that shows your access token when you are signed in.</span></span> <span data-ttu-id="69ffc-124">Na guia **token do Access,** você pode copiar o token se precisar usá-lo em seu aplicativo cliente REST favorito.</span><span class="sxs-lookup"><span data-stu-id="69ffc-124">On the **Access token** tab, you can copy the token if you need to use it in your favorite REST client application.</span></span>

![Captura de tela da guia Token de Acesso no Explorador do Graph com o botão Copiar realçada](./images/access-token.png)

## <a name="copy-code-snippets"></a><span data-ttu-id="69ffc-126">Copiar trechos de código</span><span class="sxs-lookup"><span data-stu-id="69ffc-126">Copy code snippets</span></span>

<span data-ttu-id="69ffc-127">Para cada consulta da API REST que você selecionar ou inserir no Explorador do Graph, você pode descobrir como chamar essa API em cada um dos quatro idiomas mostrados na guia **Trechos** de Código - C#, Java, JavaScript e Objective-C.</span><span class="sxs-lookup"><span data-stu-id="69ffc-127">For each REST API query you select or enter in Graph Explorer, you can find how to call that API in each of the four languages showcased under the **Code snippets** tab - C#, Java, JavaScript, and Objective-C.</span></span> 

![Captura de tela do Explorador do Graph com a guia trechos de código realçada](./images/code-snippets.png)

## <a name="ui-component-integration"></a><span data-ttu-id="69ffc-129">Integração de componentes da interface do usuário</span><span class="sxs-lookup"><span data-stu-id="69ffc-129">UI component integration</span></span>

<span data-ttu-id="69ffc-130">O Graph Explorer inclui vários recursos para facilitar a implementação da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="69ffc-130">Graph Explorer includes several features to make implementing UI easier.</span></span> <span data-ttu-id="69ffc-131">Reutilizar esses componentes em seus aplicativos também.</span><span class="sxs-lookup"><span data-stu-id="69ffc-131">Reuse these components in your apps too.</span></span>

### <a name="microsoft-graph-toolkit-integration"></a><span data-ttu-id="69ffc-132">Integração com o Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="69ffc-132">Microsoft Graph Toolkit integration</span></span>

<span data-ttu-id="69ffc-133">O [Microsoft Graph Toolkit](/graph/toolkit/overview) é uma coleção de componentes da Web reutilizáveis e sem estrutura e auxiliares para acessar e trabalhar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="69ffc-133">The [Microsoft Graph Toolkit](/graph/toolkit/overview) is a collection of reusable, framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="69ffc-134">Os componentes são totalmente funcionais, com provedores internos que autenticam e buscam dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="69ffc-134">The components are fully functional, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="69ffc-135">O Graph Explorer fornece exemplos de consultas à API REST que correspondem aos componentes do Kit de Ferramentas do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="69ffc-135">Graph Explorer provides sample REST API queries that correspond to Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="69ffc-136">Um ponto azul na guia do componente **Toolkit** indica que o Kit de Ferramentas fornece um componente para a consulta à API REST especificada no momento no Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="69ffc-136">A blue dot on the **Toolkit component** tab indicates that the Toolkit provides a component for the currently specified REST API query in Graph Explorer.</span></span> <span data-ttu-id="69ffc-137">Você pode copiar convenientemente o código do componente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69ffc-137">You can conveniently copy the code for the component to your app.</span></span>

<span data-ttu-id="69ffc-138">A tabela a seguir lista as consultas de exemplo que atualmente incluem um componente do Kit de Ferramentas.</span><span class="sxs-lookup"><span data-stu-id="69ffc-138">The following table lists the sample queries that currently include a Toolkit component.</span></span>

| <span data-ttu-id="69ffc-139">**Consulta de exemplo do Graph Explorer**</span><span class="sxs-lookup"><span data-stu-id="69ffc-139">**Graph Explorer sample query**</span></span> | <span data-ttu-id="69ffc-140">**URL do iFrame de exemplo do Kit de Ferramentas**</span><span class="sxs-lookup"><span data-stu-id="69ffc-140">**Toolkit sample iFrame URL**</span></span> |
| --- | --- |
| <span data-ttu-id="69ffc-141">GET meu perfil</span><span class="sxs-lookup"><span data-stu-id="69ffc-141">GET my profile</span></span> | [<span data-ttu-id="69ffc-142"> https://mgt.dev/iframe.html?id=components-mgt-person-card—person-card-hover</span><span class="sxs-lookup"><span data-stu-id="69ffc-142">https://mgt.dev/iframe.html?id=components-mgt-person-card—person-card-hover</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person-card--person-card-hover&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083362882%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=9FvGlMZNc78EE66JiY7hrusYVuGUm2NeflYlVgwTVwo%3D&amp;reserved=0) |
| <span data-ttu-id="69ffc-143">GET pessoas com quem trabalho</span><span class="sxs-lookup"><span data-stu-id="69ffc-143">GET people I work with</span></span> | [<span data-ttu-id="69ffc-144"> https://mgt.dev/iframe.html?id=components-mgt-people—people</span><span class="sxs-lookup"><span data-stu-id="69ffc-144">https://mgt.dev/iframe.html?id=components-mgt-people—people</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-people--people&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083372878%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=yMF3X0M%2FmvWTUfhMdNYkG5I7fDMXpPHS6Fwea%2B3ycPs%3D&amp;reserved=0) |
| <span data-ttu-id="69ffc-145">OBTER todas as minhas tarefas de planejador</span><span class="sxs-lookup"><span data-stu-id="69ffc-145">GET all my planner tasks</span></span> | [<span data-ttu-id="69ffc-146"> https://mgt.dev/iframe.html?id=components-mgt-tasks—tasks</span><span class="sxs-lookup"><span data-stu-id="69ffc-146">https://mgt.dev/iframe.html?id=components-mgt-tasks—tasks</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-tasks--tasks&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=Vk5IhPb%2FNbni7c6bteEveIdQNn%2BPm6AchwewCJ%2Fkmzk%3D&amp;reserved=0) |
| <span data-ttu-id="69ffc-147">GET meus eventos para a próxima semana</span><span class="sxs-lookup"><span data-stu-id="69ffc-147">GET my events for the next week</span></span> | [<span data-ttu-id="69ffc-148"> https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week</span><span class="sxs-lookup"><span data-stu-id="69ffc-148">https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-agenda--get-events-for-next-week&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=VVFcx3gXMmg%2B%2BdQCZXjAmkCk5zKcrntK6fI35jbdN94%3D&amp;reserved=0) |
| <span data-ttu-id="69ffc-149">GET minha foto</span><span class="sxs-lookup"><span data-stu-id="69ffc-149">GET my photo</span></span> | [<span data-ttu-id="69ffc-150"> https://mgt.dev/iframe.html?id=components-mgt-person—person-photo-only</span><span class="sxs-lookup"><span data-stu-id="69ffc-150">https://mgt.dev/iframe.html?id=components-mgt-person—person-photo-only</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person--person-photo-only&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083392872%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=aI%2BUqciLPOxEqlIpbjT8wtWBgcaJWM6sqooRlLVspZ0%3D&amp;reserved=0) |

![Captura de tela mostrando a guia Componentes do Kit de Ferramentas com o código para gerar o componente realçado](./images/get-graph-toolkit-card.png)

### <a name="adaptive-cards-integration"></a><span data-ttu-id="69ffc-152">Integração de cartões adaptáveis</span><span class="sxs-lookup"><span data-stu-id="69ffc-152">Adaptive cards integration</span></span>

<span data-ttu-id="69ffc-153">[Cartões adaptáveis](https://adaptivecards.io/) são trechos de interface do usuário que não são de plataforma, de autoria em JSON, que aplicativos e serviços podem trocar de forma aberta.</span><span class="sxs-lookup"><span data-stu-id="69ffc-153">[Adaptive cards](https://adaptivecards.io/) are platform-agnostic snippets of UI, authored in JSON, that apps and services can openly exchange.</span></span> <span data-ttu-id="69ffc-154">Quando você executar uma consulta e um cartão adaptável estiver disponível, um ponto azul aparecerá na **guia Cartões adaptáveis.**</span><span class="sxs-lookup"><span data-stu-id="69ffc-154">When you run a query and an adaptive card is available, a blue dot appears on the **Adaptive cards** tab.</span></span>

![Captura de tela da guia cartões adaptáveis no Explorador do Graph com os detalhes da resposta realçadas](./images/adaptive-cards.png)

## <a name="customize-the-theme-in-graph-explorer"></a><span data-ttu-id="69ffc-156">Personalizar o tema no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="69ffc-156">Customize the theme in Graph Explorer</span></span>

<span data-ttu-id="69ffc-157">Escolha o tema do Explorador do Graph selecionando a **opção Alterar tema** na engrenagem de configurações.</span><span class="sxs-lookup"><span data-stu-id="69ffc-157">Choose the theme for Graph Explorer by selecting the **Change theme** option under the settings gear.</span></span> <span data-ttu-id="69ffc-158">As opções de tema são Claro, Escuro e Alto contraste.</span><span class="sxs-lookup"><span data-stu-id="69ffc-158">Theme options are Light, Dark, and High contrast.</span></span>

![Captura de tela da opção Alterar tema no Explorador do Graph com as opções de tema realçadas](./images/change-theme.png)

## <a name="storing-and-sharing-queries"></a><span data-ttu-id="69ffc-160">Armazenar e compartilhar consultas</span><span class="sxs-lookup"><span data-stu-id="69ffc-160">Storing and sharing queries</span></span>

<span data-ttu-id="69ffc-161">As consultas que são executados no Explorador do Graph são salvas por 30 dias na **guia** Histórico. Na guia Histórico, você pode:</span><span class="sxs-lookup"><span data-stu-id="69ffc-161">Queries run in Graph Explorer are saved for 30 days in the **History** tab. On the History tab, you can:</span></span>

1.  <span data-ttu-id="69ffc-162">Exportar todos os itens de histórico no formato .har.</span><span class="sxs-lookup"><span data-stu-id="69ffc-162">Export all history items in .har format.</span></span>
2.  <span data-ttu-id="69ffc-163">Exclua todos os itens do histórico.</span><span class="sxs-lookup"><span data-stu-id="69ffc-163">Delete all history items.</span></span>
3.  <span data-ttu-id="69ffc-164">Exibir este item de histórico.</span><span class="sxs-lookup"><span data-stu-id="69ffc-164">View this history item.</span></span>
4.  <span data-ttu-id="69ffc-165">Execute esta consulta.</span><span class="sxs-lookup"><span data-stu-id="69ffc-165">Run this query.</span></span>
5.  <span data-ttu-id="69ffc-166">Exporte esse item de histórico no formato .har.</span><span class="sxs-lookup"><span data-stu-id="69ffc-166">Export this history item in .har format.</span></span>
6.  <span data-ttu-id="69ffc-167">Exclua este item de histórico.</span><span class="sxs-lookup"><span data-stu-id="69ffc-167">Delete this history item.</span></span>

![Captura de tela da guia Histórico com opções realçadas](./images/storing-and-sharing-queries.png)

<span data-ttu-id="69ffc-169">Para compartilhar consultas que você executar, clique no botão compartilhar consulta no painel de resposta e clique em **copiar.**</span><span class="sxs-lookup"><span data-stu-id="69ffc-169">To share queries that you run, click the share query button in the response pane and click **copy**.</span></span> <span data-ttu-id="69ffc-170">Isso copia um link para compartilhar e permite que outras pessoas vejam sua consulta e os resultados.</span><span class="sxs-lookup"><span data-stu-id="69ffc-170">This copies a link to share and allow others to see your query and the results.</span></span>

![Captura de tela do Explorador do Graph com as opções de Compartilhamento e Cópia realçadas](./images/share-query.png)

## <a name="graph-explorer-ui-features"></a><span data-ttu-id="69ffc-172">Recursos da interface do usuário do Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="69ffc-172">Graph Explorer UI features</span></span>

<span data-ttu-id="69ffc-173">Collapse and expand the sidebar component in Graph Explorer when you want to widen the request and response area.</span><span class="sxs-lookup"><span data-stu-id="69ffc-173">Collapse and expand the sidebar component in Graph Explorer when you want to widen the request and response area.</span></span> <span data-ttu-id="69ffc-174">Para fechar o componente da barra lateral, selecione o ícone de hambúrguer na parte superior esquerda da barra lateral.</span><span class="sxs-lookup"><span data-stu-id="69ffc-174">To collapse the sidebar component, select the hamburger icon on the top left of the sidebar.</span></span>

![Screenshot of Graph Explorer with the expand and collapse options highlighted](./images/expand-collapse-sidebar-component.png)

<span data-ttu-id="69ffc-176">Expanda e collapse the response preview by selecting the expand arrow in the response preview window.</span><span class="sxs-lookup"><span data-stu-id="69ffc-176">Expand and collapse the response preview by selecting the expand arrow in the response preview window.</span></span>

![Screenshot of the response pane with the expand and collapse options highlighted](./images/expand-collapse-response-preview.png)

<span data-ttu-id="69ffc-178">Acesse convenientemente o site do Programa para Desenvolvedores do Microsoft 365 a partir da interface do usuário do Graph Explorer para obter uma área de segurança gratuita com dados de exemplo para experimentar.</span><span class="sxs-lookup"><span data-stu-id="69ffc-178">Conveniently access the Microsoft 365 Developer Program site from the Graph Explorer UI to get a free sandbox with sample data to experiment with.</span></span> <span data-ttu-id="69ffc-179">Na engrenagem de configuração, selecione **Obter uma área de segurança com dados de exemplo.**</span><span class="sxs-lookup"><span data-stu-id="69ffc-179">Under the setting gear, select **Get a sandbox with sample data**.</span></span>

![Screenshot of Graph Explorer with the Get a sandbox with sample data option highlighted](./images/link-to-m365-dev-program.png)


## <a name="next-steps"></a><span data-ttu-id="69ffc-181">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="69ffc-181">Next steps</span></span>

- <span data-ttu-id="69ffc-182">Visite [o Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer/) e explore as consultas de exemplo.</span><span class="sxs-lookup"><span data-stu-id="69ffc-182">Visit [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) and explore sample queries.</span></span>
- <span data-ttu-id="69ffc-183">Explore a [documentação do Microsoft Graph Toolkit.](/graph/toolkit/overview)</span><span class="sxs-lookup"><span data-stu-id="69ffc-183">Explore the [Microsoft Graph Toolkit documentation](/graph/toolkit/overview).</span></span>
- <span data-ttu-id="69ffc-184">Contribuir ou fornecer comentários no repositório [gitHub do Explorador do Graph.](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose)</span><span class="sxs-lookup"><span data-stu-id="69ffc-184">Contribute or provide feedback in the [Graph Explorer GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).</span></span>
