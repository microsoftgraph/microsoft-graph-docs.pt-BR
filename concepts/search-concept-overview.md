---
title: Visão geral da API de pesquisa (versão prévia)
description: Saiba mais sobre como usar a API da Pesquisa da Microsoft para indexar conteúdo e adicionar pesquisa ao Office e o conteúdo indexado em seus aplicativos.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 9f80df09f982d91a4034c6b2af8e03ea8643cc03
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704383"
---
# <a name="overview-for-extending-the-microsoft-search-experience-for-apps-on-microsoft-graph-preview"></a><span data-ttu-id="8beaa-103">Visão geral de como estender a experiência da Pesquisa da Microsoft para aplicativos no Microsoft Graph (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="8beaa-103">Overview for extending the Microsoft Search experience for apps on Microsoft Graph (preview)</span></span>

<span data-ttu-id="8beaa-104">A Pesquisa da Microsoft é um mecanismo de pesquisa empresarial que proporciona ganhos de produtividade e resultados de pesquisa relevantes para sua organização.</span><span class="sxs-lookup"><span data-stu-id="8beaa-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="8beaa-105">Ela reúne o conhecimento coletivo e a produtividade de uma organização, e apresenta um conteúdo relevante para manter os usuários finais atualizados.</span><span class="sxs-lookup"><span data-stu-id="8beaa-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="8beaa-106">A Pesquisa da Microsoft está disponível em várias experiências, inclusive no Office, SharePoint, Delve, Windows e Bing.</span><span class="sxs-lookup"><span data-stu-id="8beaa-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="8beaa-107">Por que usar a API de Pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="8beaa-107">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="8beaa-108">Um ponto de extremidade de pesquisa unificado para dados de nuvem da Microsoft</span><span class="sxs-lookup"><span data-stu-id="8beaa-108">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="8beaa-109">A API da Pesquisa da Microsoft fornece um ponto de extremidade de pesquisa unificado para permitir que os desenvolvedores [consultem](/graph/api/search-query?view=graph-rest-beta) dados na nuvem da Microsoft que a Pesquisa da Microsoft já indexa, como mensagens e eventos nas caixas de correio do Outlook e arquivos no OneDrive e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8beaa-109">The Microsoft Search API provides one unified search endpoint to let developers [query](/graph/api/search-query?view=graph-rest-beta) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - data that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience"></a><span data-ttu-id="8beaa-110">Incluir dados externos personalizados na experiência de pesquisa</span><span class="sxs-lookup"><span data-stu-id="8beaa-110">Include custom external data in search experience</span></span>

<span data-ttu-id="8beaa-111">Os clientes que queiram incluir dados que estejam fora da nuvem da Microsoft em suas pesquisas poderão usar [conectores](/microsoftsearch/connectors-overview) que se conectem a uma fonte de dados específica, como um banco de dados de recursos humanos ou catálogo de produtos da organização. Para [consultar](/graph/api/search-query?view=graph-rest-beta) diretamente a fonte de dados externa, use a API de Pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8beaa-111">Customers who want to include data outside of the Microsoft cloud in their search experience can use [connectors](/microsoftsearch/connectors-overview) to connect to a specific data source such as an organization's human resources database or product catalog, and use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta) the external data source.</span></span> <span data-ttu-id="8beaa-112">A [Galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery) lista vários conectores prontos para uso.</span><span class="sxs-lookup"><span data-stu-id="8beaa-112">The [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) lists a number of ready-to-use connectors.</span></span> <span data-ttu-id="8beaa-113">Como alternativa, os clientes podem [criar conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), indexar arquivos e itens personalizados externos e consultar fontes de dados externas específicas.</span><span class="sxs-lookup"><span data-stu-id="8beaa-113">Alternatively, customers can [build connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), index external custom items and files, and query specific external data sources as well.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="8beaa-114">Experiência de pesquisa atualizada e consistente</span><span class="sxs-lookup"><span data-stu-id="8beaa-114">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="8beaa-115">Ao usar a API da Pesquisa da Microsoft, os clientes se beneficiam ao obter resultados relevantes mais personalizados com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8beaa-115">Using the Microsoft Search API, customers benefit from getting more personalized relevant results powered by Microsoft Graph.</span></span> <span data-ttu-id="8beaa-116">Isso também faz com que a pesquisa nos aplicativos retorne resultados consistentes com a pesquisa em aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="8beaa-116">This also makes search in your apps return results consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-these-apis"></a><span data-ttu-id="8beaa-117">Quais dados posso adicionar ou acessar usando essas APIs?</span><span class="sxs-lookup"><span data-stu-id="8beaa-117">What data can I add or access by using these APIs?</span></span>

<span data-ttu-id="8beaa-118">A Pesquisa da Microsoft proporciona suporte para pesquisar conteúdo na nuvem da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="8beaa-118">Microsoft Search supports searching content in the Microsoft cloud:</span></span>

- <span data-ttu-id="8beaa-119">Objetos [message](/graph/api/resources/message?view=graph-rest-beta) e [event](/graph/api/resources/event?view=graph-rest-beta) do Outlook</span><span class="sxs-lookup"><span data-stu-id="8beaa-119">Outlook [message](/graph/api/resources/message?view=graph-rest-beta) and [event](/graph/api/resources/event?view=graph-rest-beta) objects</span></span>
- <span data-ttu-id="8beaa-120">Objetos de arquivos [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) do SharePoint e do OneDrive</span><span class="sxs-lookup"><span data-stu-id="8beaa-120">SharePoint and OneDrive [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) file objects</span></span>

<span data-ttu-id="8beaa-121">Além disso, você pode indexar e pesquisar conteúdos externos:</span><span class="sxs-lookup"><span data-stu-id="8beaa-121">In addition, you can index and search external content:</span></span>

- <span data-ttu-id="8beaa-122">Objetos [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) que são de tipos personalizados</span><span class="sxs-lookup"><span data-stu-id="8beaa-122">[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) objects which are of custom types</span></span>
- <span data-ttu-id="8beaa-123">Objetos [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) que são de tipos conhecidos</span><span class="sxs-lookup"><span data-stu-id="8beaa-123">[externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) objects which are of well-known types</span></span>

## <a name="api-reference"></a><span data-ttu-id="8beaa-124">Referência da API</span><span class="sxs-lookup"><span data-stu-id="8beaa-124">API reference</span></span>

<span data-ttu-id="8beaa-125">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="8beaa-125">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="8beaa-126">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="8beaa-126">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="8beaa-127">Usar a API de Pesquisa da Microsoft para indexar dados</span><span class="sxs-lookup"><span data-stu-id="8beaa-127">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="8beaa-128">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8beaa-128">Next steps</span></span>

- <span data-ttu-id="8beaa-129">Saiba mais sobre a [Pesquisa da Microsoft](/microsoftsearch/).</span><span class="sxs-lookup"><span data-stu-id="8beaa-129">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="8beaa-130">Saiba mais sobre alguns dos principais casos de uso:</span><span class="sxs-lookup"><span data-stu-id="8beaa-130">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="8beaa-131">Pesquisar mensagens do Outlook</span><span class="sxs-lookup"><span data-stu-id="8beaa-131">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="8beaa-132">Pesquisar eventos do calendário</span><span class="sxs-lookup"><span data-stu-id="8beaa-132">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="8beaa-133">Gerenciar conexões para indexar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="8beaa-133">Manage connections to index external content</span></span>](search-index-manage-connections.md)
  - [<span data-ttu-id="8beaa-134">Indexar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="8beaa-134">Index external content</span></span>](search-index-manage-items.md)
  - [<span data-ttu-id="8beaa-135">Pesquisar tipos personalizados (externalItem)</span><span class="sxs-lookup"><span data-stu-id="8beaa-135">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
  - [<span data-ttu-id="8beaa-136">Pesquisar arquivos (incluindo externalFile)</span><span class="sxs-lookup"><span data-stu-id="8beaa-136">Search files (including externalFile)</span></span>](search-concept-files.md)
- <span data-ttu-id="8beaa-137">Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="8beaa-137">Explore the search APIs in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="8beaa-138">Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="8beaa-138">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="8beaa-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="8beaa-139">See also</span></span>

<span data-ttu-id="8beaa-140">Participe da comunidade:</span><span class="sxs-lookup"><span data-stu-id="8beaa-140">Engage with the community:</span></span>

- [<span data-ttu-id="8beaa-141">Discussão no StackOverflow</span><span class="sxs-lookup"><span data-stu-id="8beaa-141">Discuss on StackOverflow</span></span>](https://stackoverflow.com/questions/tagged/microsoft-search)
