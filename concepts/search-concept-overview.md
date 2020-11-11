---
title: Visão geral da API Microsoft Search no Microsoft Graph (visualização)
description: Use a API da Pesquisa da Microsoft para indexar conteúdo e adicionar pesquisa ao Office e o conteúdo indexado em seus aplicativos.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 0ef20f80c003d880d25eff00c993bc1800545dc7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952672"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph-preview"></a><span data-ttu-id="bf416-103">Visão geral da API Microsoft Search no Microsoft Graph (visualização)</span><span class="sxs-lookup"><span data-stu-id="bf416-103">Overview of the Microsoft Search API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="bf416-104">A Pesquisa da Microsoft é um mecanismo de pesquisa empresarial que proporciona ganhos de produtividade e resultados de pesquisa relevantes para sua organização.</span><span class="sxs-lookup"><span data-stu-id="bf416-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="bf416-105">Ela reúne o conhecimento coletivo e a produtividade de uma organização, e apresenta um conteúdo relevante para manter os usuários finais atualizados.</span><span class="sxs-lookup"><span data-stu-id="bf416-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="bf416-106">A Pesquisa da Microsoft está disponível em várias experiências, inclusive no Office, SharePoint, Delve, Windows e Bing.</span><span class="sxs-lookup"><span data-stu-id="bf416-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="bf416-107">Você pode usar a API de pesquisa da Microsoft no Microsoft Graph para estender a pesquisa da Microsoft para seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="bf416-107">You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="bf416-108">Por que usar a API de Pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="bf416-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="bf416-109">Um ponto de extremidade de pesquisa unificado para dados de nuvem da Microsoft</span><span class="sxs-lookup"><span data-stu-id="bf416-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="bf416-110">A API da Pesquisa da Microsoft fornece um ponto de extremidade de pesquisa que você pode usar para permitir que os desenvolvedores [consultem](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) dados na nuvem da Microsoft que a Pesquisa da Microsoft já indexa, como mensagens e eventos nas caixas de correio do Outlook e arquivos no OneDrive e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bf416-110">The Microsoft Search API provides one unified search endpoint that you can use to [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience"></a><span data-ttu-id="bf416-111">Inclua dados externos personalizados na experiência de pesquisa</span><span class="sxs-lookup"><span data-stu-id="bf416-111">Include custom external data in search experience</span></span>

<span data-ttu-id="bf416-112">Utilize os [conectores do Microsoft Graph](/microsoftsearch/connectors-overview) para incluir dados de fora da nuvem da Microsoft em sua experiência de busca.</span><span class="sxs-lookup"><span data-stu-id="bf416-112">Use [Microsoft Graph connectors](/microsoftsearch/connectors-overview) to include data outside of the Microsoft cloud in your search experience.</span></span> <span data-ttu-id="bf416-113">Por exemplo, estabeleça uma conexão com o banco de dados de recursos humanos ou com o catálogo de produtos de uma organização.</span><span class="sxs-lookup"><span data-stu-id="bf416-113">For instance, connect to an organization's human resources database or product catalog.</span></span> <span data-ttu-id="bf416-114">Em seguida, utilize a API de Pesquisa da Microsoft para [consultar](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) perfeitamente a fonte de dados externa.</span><span class="sxs-lookup"><span data-stu-id="bf416-114">Then use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) the external data source.</span></span> 

<span data-ttu-id="bf416-115">Navegue na [galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery) para encontrar conectores prontos para uso.</span><span class="sxs-lookup"><span data-stu-id="bf416-115">Browse the [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) to find ready-to-use connectors.</span></span> <span data-ttu-id="bf416-116">Alternativamente, você pode [construir seus próprios conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases) para indexar itens personalizados externos e consultar fontes de dados externas específicas.</span><span class="sxs-lookup"><span data-stu-id="bf416-116">Alternatively, you can [build your own connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases) to index external custom items and query specific external data sources.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="bf416-117">Experiência de pesquisa atualizada e consistente</span><span class="sxs-lookup"><span data-stu-id="bf416-117">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="bf416-118">Ao usar a API de pesquisa da Microsoft, seus clientes se beneficiam dos resultados de pesquisa relevantes mais personalizados com a plataforma Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bf416-118">When you use the Microsoft Search API, your customers benefit from more personalized, relevant search results powered by Microsoft Graph.</span></span> <span data-ttu-id="bf416-119">A experiência de pesquisa em seus aplicativos retorna resultados que são consistentes com a pesquisa em aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="bf416-119">The search experience in your apps will return results that are consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a><span data-ttu-id="bf416-120">Quais dados posso adicionar ou acessar usando a API de pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="bf416-120">What data can I add or access by using the Microsoft Search API?</span></span>

<span data-ttu-id="bf416-121">A API de pesquisa da Microsoft suporta para pesquisar o seguinte conteúdo na nuvem da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="bf416-121">The Microsoft Search API supports searching the following content in the Microsoft cloud:</span></span>

- <span data-ttu-id="bf416-122">[Mensagens](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) de email do Outlook e objetos de [eventos](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) do calendário</span><span class="sxs-lookup"><span data-stu-id="bf416-122">Outlook email [messages](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) and calendar [events](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) objects</span></span>
- <span data-ttu-id="bf416-123">Arquivos e pastas do Microsoft Office SharePoint Online e do OneDrive ([driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)), [listas](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true), [listItems](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true), [sites](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) e [unidades](/graph/api/resources/drive?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="bf416-123">SharePoint and OneDrive files and folders ([driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)), [lists](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true), [listItems](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true), [sites](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) and [drives](/graph/api/resources/drive?view=graph-rest-beta&preserve-view=true)</span></span>
- <span data-ttu-id="bf416-124">Conteúdo ingerido na plataforma de conectores do Graph: [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="bf416-124">Content ingested throught the Graph Connectors platform : [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)</span></span>

## <a name="api-reference"></a><span data-ttu-id="bf416-125">Referência da API</span><span class="sxs-lookup"><span data-stu-id="bf416-125">API reference</span></span>

<span data-ttu-id="bf416-126">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="bf416-126">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="bf416-127">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="bf416-127">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="bf416-128">Usar a API de Pesquisa da Microsoft para indexar dados</span><span class="sxs-lookup"><span data-stu-id="bf416-128">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a><span data-ttu-id="bf416-129">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="bf416-129">Next steps</span></span>

- <span data-ttu-id="bf416-130">Saiba mais sobre a [Pesquisa da Microsoft](/microsoftsearch/).</span><span class="sxs-lookup"><span data-stu-id="bf416-130">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="bf416-131">Saiba mais sobre alguns dos principais casos de uso:</span><span class="sxs-lookup"><span data-stu-id="bf416-131">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="bf416-132">Gerenciar conexões para indexar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="bf416-132">Manage connections to index external content</span></span>](search-index-manage-connections.md)
  - [<span data-ttu-id="bf416-133">Indexar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="bf416-133">Index external content</span></span>](search-index-manage-items.md)
  - [<span data-ttu-id="bf416-134">Pesquisar mensagens do Outlook</span><span class="sxs-lookup"><span data-stu-id="bf416-134">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="bf416-135">Pesquisar eventos do calendário</span><span class="sxs-lookup"><span data-stu-id="bf416-135">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="bf416-136">Pesquisar conteúdo no OneDrive e Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="bf416-136">Search content in Sharepoint and OneDrive</span></span>](search-concept-files.md)
  - [<span data-ttu-id="bf416-137">Pesquisar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="bf416-137">Search external content</span></span>](search-concept-custom-types.md)
  - [<span data-ttu-id="bf416-138">Classificar resultados de pesquisa</span><span class="sxs-lookup"><span data-stu-id="bf416-138">Sort search results</span></span>](search-concept-sort.md)
  - [<span data-ttu-id="bf416-139">Refinar resultados de pesquisa</span><span class="sxs-lookup"><span data-stu-id="bf416-139">Refine search results</span></span>](search-concept-aggregation.md)
  
- <span data-ttu-id="bf416-140">Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="bf416-140">Explore the search APIs in  [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="bf416-141">Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="bf416-141">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="bf416-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="bf416-142">See also</span></span>

- <span data-ttu-id="bf416-143">Entre em contato com a Comunidade no [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) ou no GitHub.</span><span class="sxs-lookup"><span data-stu-id="bf416-143">Engage with the community on [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) or on GitHub</span></span>
