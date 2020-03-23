---
title: Visão geral da API Microsoft Search no Microsoft Graph (visualização)
description: Use a API da Pesquisa da Microsoft para indexar conteúdo e adicionar pesquisa ao Office e o conteúdo indexado em seus aplicativos.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 76cc0a1e9b8ccd7ec3eef1fb9ddf7e381b0fd19b
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892790"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph-preview"></a><span data-ttu-id="9ac12-103">Visão geral da API Microsoft Search no Microsoft Graph (visualização)</span><span class="sxs-lookup"><span data-stu-id="9ac12-103">Overview of the Microsoft Search API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="9ac12-104">A Pesquisa da Microsoft é um mecanismo de pesquisa empresarial que proporciona ganhos de produtividade e resultados de pesquisa relevantes para sua organização.</span><span class="sxs-lookup"><span data-stu-id="9ac12-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="9ac12-105">Ela reúne o conhecimento coletivo e a produtividade de uma organização, e apresenta um conteúdo relevante para manter os usuários finais atualizados.</span><span class="sxs-lookup"><span data-stu-id="9ac12-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="9ac12-106">A Pesquisa da Microsoft está disponível em várias experiências, inclusive no Office, SharePoint, Delve, Windows e Bing.</span><span class="sxs-lookup"><span data-stu-id="9ac12-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="9ac12-107">Você pode usar a API de pesquisa da Microsoft no Microsoft Graph para estender a pesquisa da Microsoft para seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="9ac12-107">You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="9ac12-108">Por que usar a API de Pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="9ac12-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="9ac12-109">Um ponto de extremidade de pesquisa unificado para dados de nuvem da Microsoft</span><span class="sxs-lookup"><span data-stu-id="9ac12-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="9ac12-110">A API da Pesquisa da Microsoft fornece um ponto de extremidade de pesquisa que você pode usar para permitir que os desenvolvedores [consultem](/graph/api/search-query?view=graph-rest-beta) dados na nuvem da Microsoft que a Pesquisa da Microsoft já indexa, como mensagens e eventos nas caixas de correio do Outlook e arquivos no OneDrive e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9ac12-110">The Microsoft Search API provides one unified search endpoint that you can use to [query](/graph/api/search-query?view=graph-rest-beta) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience"></a><span data-ttu-id="9ac12-111">Incluir dados externos personalizados na experiência de pesquisa</span><span class="sxs-lookup"><span data-stu-id="9ac12-111">Include custom external data in search experience</span></span>

<span data-ttu-id="9ac12-112">Os clientes que queiram incluir dados que estejam fora da nuvem da Microsoft em suas pesquisas poderão usar [conectores](/microsoftsearch/connectors-overview) que se conectem a uma fonte de dados específica, como um banco de dados de recursos humanos ou catálogo de produtos da organização. Para [consultar](/graph/api/search-query?view=graph-rest-beta) diretamente a fonte de dados externa, use a API de Pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9ac12-112">Customers who want to include data outside of the Microsoft cloud in their search experience can use [connectors](/microsoftsearch/connectors-overview) to connect to a specific data source such as an organization's human resources database or product catalog, and use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta) the external data source.</span></span> <span data-ttu-id="9ac12-113">A [Galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery) lista vários conectores prontos para uso.</span><span class="sxs-lookup"><span data-stu-id="9ac12-113">The [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) lists a number of ready-to-use connectors.</span></span> <span data-ttu-id="9ac12-114">Como alternativa, os clientes podem [criar conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), indexar itens personalizados externos e também consultar fontes de dados externas específicas.</span><span class="sxs-lookup"><span data-stu-id="9ac12-114">Alternatively, customers can [build connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), index external custom items, and query specific external data sources as well.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="9ac12-115">Experiência de pesquisa atualizada e consistente</span><span class="sxs-lookup"><span data-stu-id="9ac12-115">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="9ac12-116">Ao usar a API de pesquisa da Microsoft, seus clientes se beneficiam dos resultados de pesquisa relevantes mais personalizados com a plataforma Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9ac12-116">When you use the Microsoft Search API, your customers benefit from more personalized, relevant search results powered by Microsoft Graph.</span></span> <span data-ttu-id="9ac12-117">A experiência de pesquisa em seus aplicativos retorna resultados que são consistentes com a pesquisa em aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="9ac12-117">The search experience in your apps will return results that are consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a><span data-ttu-id="9ac12-118">Quais dados posso adicionar ou acessar usando a API de pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="9ac12-118">What data can I add or access by using the Microsoft Search API?</span></span>

<span data-ttu-id="9ac12-119">A API de pesquisa da Microsoft suporta para pesquisar o seguinte conteúdo na nuvem da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="9ac12-119">The Microsoft Search API supports searching the following content in the Microsoft cloud:</span></span>

- <span data-ttu-id="9ac12-120">Objetos [message](/graph/api/resources/message?view=graph-rest-beta) e [event](/graph/api/resources/event?view=graph-rest-beta) do Outlook</span><span class="sxs-lookup"><span data-stu-id="9ac12-120">Outlook [message](/graph/api/resources/message?view=graph-rest-beta) and [event](/graph/api/resources/event?view=graph-rest-beta) objects</span></span>
- <span data-ttu-id="9ac12-121">Objetos de arquivos [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) do SharePoint e do OneDrive</span><span class="sxs-lookup"><span data-stu-id="9ac12-121">SharePoint and OneDrive [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) file objects</span></span>

<span data-ttu-id="9ac12-122">Além disso, você pode indexar e pesquisar conteúdo externo através do objeto [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="9ac12-122">In addition, you can index and search external content via the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) object.</span></span>

## <a name="api-reference"></a><span data-ttu-id="9ac12-123">Referência da API</span><span class="sxs-lookup"><span data-stu-id="9ac12-123">API reference</span></span>

<span data-ttu-id="9ac12-124">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="9ac12-124">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="9ac12-125">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="9ac12-125">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="9ac12-126">Usar a API de Pesquisa da Microsoft para indexar dados</span><span class="sxs-lookup"><span data-stu-id="9ac12-126">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="9ac12-127">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9ac12-127">Next steps</span></span>

- <span data-ttu-id="9ac12-128">Saiba mais sobre a [Pesquisa da Microsoft](/microsoftsearch/).</span><span class="sxs-lookup"><span data-stu-id="9ac12-128">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="9ac12-129">Saiba mais sobre alguns dos principais casos de uso:</span><span class="sxs-lookup"><span data-stu-id="9ac12-129">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="9ac12-130">Pesquisar mensagens do Outlook</span><span class="sxs-lookup"><span data-stu-id="9ac12-130">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="9ac12-131">Pesquisar eventos do calendário</span><span class="sxs-lookup"><span data-stu-id="9ac12-131">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="9ac12-132">Gerenciar conexões para indexar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="9ac12-132">Manage connections to index external content</span></span>](search-index-manage-connections.md)
  - [<span data-ttu-id="9ac12-133">Indexar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="9ac12-133">Index external content</span></span>](search-index-manage-items.md)
  - [<span data-ttu-id="9ac12-134">Pesquisar tipos personalizados (externalItem)</span><span class="sxs-lookup"><span data-stu-id="9ac12-134">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
  - [<span data-ttu-id="9ac12-135">Pesquisar arquivos (incluindo externalFile)</span><span class="sxs-lookup"><span data-stu-id="9ac12-135">Search files (including externalFile)</span></span>](search-concept-files.md)
- <span data-ttu-id="9ac12-136">Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="9ac12-136">Explore the search APIs in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="9ac12-137">Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="9ac12-137">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="9ac12-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="9ac12-138">See also</span></span>

- <span data-ttu-id="9ac12-139">Entre em contato com a Comunidade no [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search).</span><span class="sxs-lookup"><span data-stu-id="9ac12-139">Engage with the community on [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search).</span></span>
