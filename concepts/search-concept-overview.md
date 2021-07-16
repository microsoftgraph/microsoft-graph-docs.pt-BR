---
title: Visão geral da API da Pesquisa da Microsoft no Microsoft Graph
description: Use a API da Pesquisa da Microsoft para indexar conteúdo e adicionar pesquisa ao Office e o conteúdo indexado em seus aplicativos.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 3a6c02b4f70cce4ac44090f5981372096fa17bce
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443123"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph"></a><span data-ttu-id="6649f-103">Visão geral da API da Pesquisa da Microsoft no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6649f-103">Overview of the Microsoft Search API in Microsoft Graph</span></span>

<span data-ttu-id="6649f-104">A Pesquisa da Microsoft é um mecanismo de pesquisa empresarial que proporciona ganhos de produtividade e resultados de pesquisa relevantes para sua organização.</span><span class="sxs-lookup"><span data-stu-id="6649f-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="6649f-105">Ela reúne o conhecimento coletivo e a produtividade de uma organização, e apresenta um conteúdo relevante para manter os usuários finais atualizados.</span><span class="sxs-lookup"><span data-stu-id="6649f-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="6649f-106">A Pesquisa da Microsoft está disponível em várias experiências, inclusive no Office, SharePoint, Delve, Windows e Bing.</span><span class="sxs-lookup"><span data-stu-id="6649f-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="6649f-107">Você pode usar a API de pesquisa da Microsoft no Microsoft Graph para estender a pesquisa da Microsoft para seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="6649f-107">You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.</span></span>


<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="6649f-108">Por que usar a API de Pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="6649f-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="6649f-109">Um ponto de extremidade de pesquisa unificado para dados de nuvem da Microsoft</span><span class="sxs-lookup"><span data-stu-id="6649f-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="6649f-110">A API da Pesquisa da Microsoft fornece um ponto de extremidade de pesquisa que você pode usar para permitir que os desenvolvedores [consultem](/graph/api/search-query) dados na nuvem da Microsoft que a Pesquisa da Microsoft já indexa, como mensagens e eventos nas caixas de correio do Outlook e arquivos no OneDrive e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6649f-110">The Microsoft Search API provides one unified search endpoint that you can use to [query](/graph/api/search-query) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience-preview"></a><span data-ttu-id="6649f-111">Incluir dados externos personalizados na experiência de pesquisa (visualização)</span><span class="sxs-lookup"><span data-stu-id="6649f-111">Include custom external data in search experience (preview)</span></span>

<span data-ttu-id="6649f-112">Use[conectores do Microsoft Graph](/microsoftsearch/connectors-overview) para incluir dados de fora da nuvem da Microsoft em sua experiência de busca.</span><span class="sxs-lookup"><span data-stu-id="6649f-112">Use [Microsoft Graph connectors](/microsoftsearch/connectors-overview) to include data outside of the Microsoft cloud in your search experience.</span></span> <span data-ttu-id="6649f-113">Por exemplo, estabeleça uma conexão com o banco de dados de recursos humanos ou com o catálogo de produtos de uma organização.</span><span class="sxs-lookup"><span data-stu-id="6649f-113">For instance, connect to an organization's human resources database or product catalog.</span></span> <span data-ttu-id="6649f-114">Em seguida, utilize a API de Pesquisa da Microsoft para [consultar](/graph/api/search-query) perfeitamente a fonte de dados externa.</span><span class="sxs-lookup"><span data-stu-id="6649f-114">Then use the Microsoft Search API to seamlessly [query](/graph/api/search-query) the external data source.</span></span> 

<span data-ttu-id="6649f-115">Navegue na [galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery) para encontrar conectores prontos para uso.</span><span class="sxs-lookup"><span data-stu-id="6649f-115">Browse the [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) to find ready-to-use connectors.</span></span> <span data-ttu-id="6649f-116">Alternativamente, você pode [construir seus próprios conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases) para indexar itens personalizados externos e consultar fontes de dados externas específicas.</span><span class="sxs-lookup"><span data-stu-id="6649f-116">Alternatively, you can [build your own connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases) to index external custom items and query specific external data sources.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="6649f-117">Experiência de pesquisa atualizada e consistente</span><span class="sxs-lookup"><span data-stu-id="6649f-117">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="6649f-118">Ao usar a API de pesquisa da Microsoft, seus clientes se beneficiam dos resultados de pesquisa relevantes mais personalizados com a plataforma Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6649f-118">When you use the Microsoft Search API, your customers benefit from more personalized, relevant search results powered by Microsoft Graph.</span></span> <span data-ttu-id="6649f-119">A experiência de pesquisa em seus aplicativos retorna resultados que são consistentes com a pesquisa em aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="6649f-119">The search experience in your apps will return results that are consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a><span data-ttu-id="6649f-120">Quais dados posso adicionar ou acessar usando a API de pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="6649f-120">What data can I add or access by using the Microsoft Search API?</span></span>

<span data-ttu-id="6649f-121">A API de pesquisa da Microsoft suporta para pesquisar o seguinte conteúdo na nuvem da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="6649f-121">The Microsoft Search API supports searching the following content in the Microsoft cloud:</span></span> 

- <span data-ttu-id="6649f-122">Recursos de [mensagens](/graph/api/resources/message) de email e [eventos](/graph/api/resources/event) do calendário do Outlook.</span><span class="sxs-lookup"><span data-stu-id="6649f-122">Outlook email [message](/graph/api/resources/message) and calendar [event](/graph/api/resources/event) resources.</span></span>
- <span data-ttu-id="6649f-123">Arquivos e pastas do SharePoint e OneDrive (recursos [driveItem](/graph/api/resources/driveitem)), [lista](/graph/api/resources/list), [listItem](/graph/api/resources/listitem), [site](/graph/api/resources/site) e recursos de [unidade](/graph/api/resources/drive).</span><span class="sxs-lookup"><span data-stu-id="6649f-123">SharePoint and OneDrive files and folders ([driveItem](/graph/api/resources/driveitem) resources), [list](/graph/api/resources/list), [listItem](/graph/api/resources/listitem), [site](/graph/api/resources/site), and [drive](/graph/api/resources/drive) resources.</span></span>
- <span data-ttu-id="6649f-124">Recursos [pessoais](/graph/api/resources/person) em uma organização que são mais relevantes para um usuário.</span><span class="sxs-lookup"><span data-stu-id="6649f-124">[Person](/graph/api/resources/person) resources in an organization who are most relevant to a user.</span></span>
- <span data-ttu-id="6649f-125">Conteúdo ingerido por meio da plataforma de conectores do Microsoft Graph: recursos [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6649f-125">Content ingested through the Microsoft Graph connectors platform : [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) resources.</span></span>

## <a name="api-reference"></a><span data-ttu-id="6649f-126">Referência da API</span><span class="sxs-lookup"><span data-stu-id="6649f-126">API reference</span></span>

<span data-ttu-id="6649f-127">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="6649f-127">Looking for the API reference for this service?</span></span>

- <span data-ttu-id="6649f-128">[Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-1.0&preserve-view=true)(v1.0)</span><span class="sxs-lookup"><span data-stu-id="6649f-128">[Use the Microsoft Search API to query data](/graph/api/resources/search-api-overview?view=graph-rest-1.0&preserve-view=true) (v1.0)</span></span>
- <span data-ttu-id="6649f-129">[Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)(pré-visualização)</span><span class="sxs-lookup"><span data-stu-id="6649f-129">[Use the Microsoft Search API to query data](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true) (preview)</span></span>
- <span data-ttu-id="6649f-130">[Usar a API de Pesquisa da Microsoft para indexar dados](/graph/api/resources/indexing-api-overview) (pré-visualização)</span><span class="sxs-lookup"><span data-stu-id="6649f-130">[Use the Microsoft Search API to index data](/graph/api/resources/indexing-api-overview) (preview)</span></span>

## <a name="next-steps"></a><span data-ttu-id="6649f-131">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6649f-131">Next steps</span></span>

- <span data-ttu-id="6649f-132">Saiba mais sobre a [Pesquisa da Microsoft](/microsoftsearch/).</span><span class="sxs-lookup"><span data-stu-id="6649f-132">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="6649f-133">Saiba mais sobre alguns dos principais casos de uso:</span><span class="sxs-lookup"><span data-stu-id="6649f-133">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="6649f-134">Gerenciar conexões para indexar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="6649f-134">Manage connections to index external content</span></span>](connecting-external-content-manage-connections.md)
  - [<span data-ttu-id="6649f-135">Indexar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="6649f-135">Index external content</span></span>](connecting-external-content-manage-items.md)
  - [<span data-ttu-id="6649f-136">Pesquisar mensagens do Outlook</span><span class="sxs-lookup"><span data-stu-id="6649f-136">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="6649f-137">Pesquisar eventos do calendário</span><span class="sxs-lookup"><span data-stu-id="6649f-137">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="6649f-138">Pesquisar conteúdo no OneDrive e Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6649f-138">Search content in Sharepoint and OneDrive</span></span>](search-concept-files.md)
  - [<span data-ttu-id="6649f-139">Pesquisar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="6649f-139">Search external content</span></span>](search-concept-custom-types.md)
  - <span data-ttu-id="6649f-140">[Pesquisar pessoa](search-concept-person.md) (visualização)</span><span class="sxs-lookup"><span data-stu-id="6649f-140">[Search person](search-concept-person.md) (preview)</span></span>
  - <span data-ttu-id="6649f-141">[Classificar resultados de pesquisa](search-concept-sort.md) (pré-visualização)</span><span class="sxs-lookup"><span data-stu-id="6649f-141">[Sort search results](search-concept-sort.md) (preview)</span></span>
  - <span data-ttu-id="6649f-142">[Refinar resultados de pesquisa](search-concept-aggregation.md) (pré-visualização)</span><span class="sxs-lookup"><span data-stu-id="6649f-142">[Refine search results](search-concept-aggregation.md) (preview)</span></span>
  - <span data-ttu-id="6649f-143">[Solicitar correção ortográfica](search-concept-speller.md) (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="6649f-143">[Request spelling correction](search-concept-speller.md) (preview)</span></span>
  - <span data-ttu-id="6649f-144">[Layout de exibição de pesquisa](search-concept-display-layout.md) (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="6649f-144">[Search display layout](search-concept-display-layout.md) (preview)</span></span>
 
  
- <span data-ttu-id="6649f-145">Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="6649f-145">Explore the search APIs in  [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="6649f-146">Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="6649f-146">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="6649f-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="6649f-147">See also</span></span>

- <span data-ttu-id="6649f-148">Envolva-se com a comunidade no [Microsoft Q&A](/answers/products/m365#microsoft-graph)  ou no GitHub</span><span class="sxs-lookup"><span data-stu-id="6649f-148">Engage with the community on [Microsoft Q&A](/answers/products/m365#microsoft-graph)  or on GitHub</span></span>
