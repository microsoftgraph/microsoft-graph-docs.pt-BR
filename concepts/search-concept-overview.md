---
title: Visão geral da API de pesquisa (versão prévia)
description: Saiba mais sobre como usar a API da Pesquisa da Microsoft para indexar conteúdo e adicionar pesquisa ao Office e o conteúdo indexado em seus aplicativos.
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 4196a2b01576e11f2b9db28a4ea1f89d76f467c5
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955908"
---
# <a name="overview-for-extending-the-microsoft-search-experience-for-apps-on-microsoft-graph-preview"></a><span data-ttu-id="07be1-103">Visão geral de como estender a experiência da Pesquisa da Microsoft para aplicativos no Microsoft Graph (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="07be1-103">Overview for extending the Microsoft Search experience for apps on Microsoft Graph (preview)</span></span>

<span data-ttu-id="07be1-104">A Pesquisa da Microsoft é um mecanismo de pesquisa empresarial que proporciona ganhos de produtividade e resultados de pesquisa relevantes para sua organização.</span><span class="sxs-lookup"><span data-stu-id="07be1-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="07be1-105">Ela reúne o conhecimento coletivo e a produtividade de uma organização, e apresenta um conteúdo relevante para manter os usuários finais atualizados.</span><span class="sxs-lookup"><span data-stu-id="07be1-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="07be1-106">A Pesquisa da Microsoft está disponível em várias experiências, inclusive no Office, SharePoint, Delve, Windows e Bing.</span><span class="sxs-lookup"><span data-stu-id="07be1-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="07be1-107">A API do Microsoft Search permite aos aplicativos estender a experiência de pesquisa semelhante aos clientes dos aplicativos.</span><span class="sxs-lookup"><span data-stu-id="07be1-107">The Microsoft Search API allows apps to extend the similar search experience for their app customers.</span></span> 

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="07be1-108">Por que usar a API de Pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="07be1-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="07be1-109">Um ponto de extremidade de pesquisa unificado para dados de nuvem da Microsoft</span><span class="sxs-lookup"><span data-stu-id="07be1-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="07be1-110">A API da Pesquisa da Microsoft fornece um ponto de extremidade de pesquisa unificado para permitir que os desenvolvedores [consultem](/graph/api/search-query?view=graph-rest-beta) dados na nuvem da Microsoft que a Pesquisa da Microsoft já indexa, como mensagens e eventos nas caixas de correio do Outlook e arquivos no OneDrive e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="07be1-110">The Microsoft Search API provides one unified search endpoint to let developers [query](/graph/api/search-query?view=graph-rest-beta) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - data that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience"></a><span data-ttu-id="07be1-111">Incluir dados externos personalizados na experiência de pesquisa</span><span class="sxs-lookup"><span data-stu-id="07be1-111">Include custom external data in search experience</span></span>

<span data-ttu-id="07be1-112">Os clientes que queiram incluir dados que estejam fora da nuvem da Microsoft em suas pesquisas poderão usar [conectores](/microsoftsearch/connectors-overview) que se conectem a uma fonte de dados específica, como um banco de dados de recursos humanos ou catálogo de produtos da organização. Para [consultar](/graph/api/search-query?view=graph-rest-beta) diretamente a fonte de dados externa, use a API de Pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="07be1-112">Customers who want to include data outside of the Microsoft cloud in their search experience can use [connectors](/microsoftsearch/connectors-overview) to connect to a specific data source such as an organization's human resources database or product catalog, and use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta) the external data source.</span></span> <span data-ttu-id="07be1-113">A [Galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery) lista vários conectores prontos para uso.</span><span class="sxs-lookup"><span data-stu-id="07be1-113">The [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) lists a number of ready-to-use connectors.</span></span> <span data-ttu-id="07be1-114">Como alternativa, os clientes podem [criar conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), indexar arquivos e itens personalizados externos e consultar fontes de dados externas específicas.</span><span class="sxs-lookup"><span data-stu-id="07be1-114">Alternatively, customers can [build connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), index external custom items and files, and query specific external data sources as well.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="07be1-115">Experiência de pesquisa atualizada e consistente</span><span class="sxs-lookup"><span data-stu-id="07be1-115">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="07be1-116">Ao usar a API da Pesquisa da Microsoft, os clientes se beneficiam ao obter resultados relevantes mais personalizados com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="07be1-116">Using the Microsoft Search API, customers benefit from getting more personalized relevant results powered by Microsoft Graph.</span></span> <span data-ttu-id="07be1-117">Isso também faz com que a pesquisa nos aplicativos retorne resultados consistentes com a pesquisa em aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="07be1-117">This also makes search in your apps return results consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-these-apis"></a><span data-ttu-id="07be1-118">Quais dados posso adicionar ou acessar usando essas APIs?</span><span class="sxs-lookup"><span data-stu-id="07be1-118">What data can I add or access by using these APIs?</span></span>

<span data-ttu-id="07be1-119">A Pesquisa da Microsoft proporciona suporte para pesquisar conteúdo na nuvem da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="07be1-119">Microsoft Search supports searching content in the Microsoft cloud:</span></span>

- <span data-ttu-id="07be1-120">Objetos [message](/graph/api/resources/message?view=graph-rest-beta) e [event](/graph/api/resources/event?view=graph-rest-beta) do Outlook</span><span class="sxs-lookup"><span data-stu-id="07be1-120">Outlook [message](/graph/api/resources/message?view=graph-rest-beta) and [event](/graph/api/resources/event?view=graph-rest-beta) objects</span></span>
- <span data-ttu-id="07be1-121">Objetos de arquivos [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) do SharePoint e do OneDrive</span><span class="sxs-lookup"><span data-stu-id="07be1-121">SharePoint and OneDrive [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) file objects</span></span>

<span data-ttu-id="07be1-122">Além disso, você pode indexar e pesquisar conteúdos externos:</span><span class="sxs-lookup"><span data-stu-id="07be1-122">In addition, you can index and search external content:</span></span>

- <span data-ttu-id="07be1-123">Objetos [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) que são de tipos personalizados</span><span class="sxs-lookup"><span data-stu-id="07be1-123">[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) objects which are of custom types</span></span>
- <span data-ttu-id="07be1-124">Objetos [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) que são de tipos conhecidos</span><span class="sxs-lookup"><span data-stu-id="07be1-124">[externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) objects which are of well-known types</span></span>

## <a name="api-reference"></a><span data-ttu-id="07be1-125">Referência da API</span><span class="sxs-lookup"><span data-stu-id="07be1-125">API reference</span></span>

<span data-ttu-id="07be1-126">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="07be1-126">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="07be1-127">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="07be1-127">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="07be1-128">Usar a API de Pesquisa da Microsoft para indexar dados</span><span class="sxs-lookup"><span data-stu-id="07be1-128">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="07be1-129">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="07be1-129">Next steps</span></span>

- <span data-ttu-id="07be1-130">Saiba mais sobre a [Pesquisa da Microsoft](/microsoftsearch/).</span><span class="sxs-lookup"><span data-stu-id="07be1-130">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="07be1-131">Saiba mais sobre alguns dos principais casos de uso:</span><span class="sxs-lookup"><span data-stu-id="07be1-131">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="07be1-132">Pesquisar mensagens do Outlook</span><span class="sxs-lookup"><span data-stu-id="07be1-132">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="07be1-133">Pesquisar eventos do calendário</span><span class="sxs-lookup"><span data-stu-id="07be1-133">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="07be1-134">Gerenciar conexões para indexar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="07be1-134">Manage connections to index external content</span></span>](search-index-manage-connections.md)
  - [<span data-ttu-id="07be1-135">Indexar conteúdo externo</span><span class="sxs-lookup"><span data-stu-id="07be1-135">Index external content</span></span>](search-index-manage-items.md)
  - [<span data-ttu-id="07be1-136">Pesquisar tipos personalizados (externalItem)</span><span class="sxs-lookup"><span data-stu-id="07be1-136">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
  - [<span data-ttu-id="07be1-137">Pesquisar arquivos (incluindo externalFile)</span><span class="sxs-lookup"><span data-stu-id="07be1-137">Search files (including externalFile)</span></span>](search-concept-files.md)
- <span data-ttu-id="07be1-138">Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="07be1-138">Explore the search APIs in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="07be1-139">Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="07be1-139">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="07be1-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="07be1-140">See also</span></span>

<span data-ttu-id="07be1-141">Participe da comunidade:</span><span class="sxs-lookup"><span data-stu-id="07be1-141">Engage with the community:</span></span>

- [<span data-ttu-id="07be1-142">Discussão no StackOverflow</span><span class="sxs-lookup"><span data-stu-id="07be1-142">Discuss on StackOverflow</span></span>](https://stackoverflow.com/questions/tagged/microsoft-graph-search)
