---
title: Usar a API de Pesquisa da Microsoft para consultar dados
description: Utilizando a API de pesquisa, os aplicativos podem pesquisar os dados do Microsoft 365 no contexto do usuário autenticado
localization_priority: Priority
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e77c0170487b0762538d98376921565857c9b3c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985780"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a><span data-ttu-id="e3f7d-103">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="e3f7d-103">Use the Microsoft Search API to query data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3f7d-104">Você pode utilizar a API de Pesquisa da Microsoft para consultar os dados do Microsoft 365 nos seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-104">You can use the Microsoft Search API to query Microsoft 365 data in your apps.</span></span>

<span data-ttu-id="e3f7d-105">As solicitações de pesquisa são executadas no contexto do usuário conectado, identificado usando um [token de acesso com permissões delegadas](/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="e3f7d-105">Search requests run in the context of the signed-in user, identified using an [access token with delegated permissions](/graph/auth-v2-user).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a><span data-ttu-id="e3f7d-106">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="e3f7d-106">Common use cases</span></span>

<span data-ttu-id="e3f7d-107">A API de Pesquisa da Microsoft fornece um método de [query](../api/search-query.md) para pesquisar os dados na Pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-107">The Microsoft Search API provides a [query](../api/search-query.md) method to search across your data in Microsoft Search.</span></span> <span data-ttu-id="e3f7d-108">Esta seção lista os casos de uso comuns, com base nas propriedades definidas no corpo da solicitação **query**.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-108">This section lists the common use cases, based on the properties you set in the **query** request body.</span></span>

<span data-ttu-id="e3f7d-109">As solicitações de pesquisa são executadas em nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-109">Search requests run on behalf of the user.</span></span> <span data-ttu-id="e3f7d-110">Os resultados da pesquisa têm escopo para impor o controle de acesso aplicado aos itens.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-110">Search results are scoped to enforce any access control applied to the items.</span></span>  <span data-ttu-id="e3f7d-111">Por exemplo, no contexto de arquivos, as permissões em relação aos arquivos serão avaliadas como parte da solicitação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-111">For example, in the context of files, permissions on the files are evaluated as part of the search request.</span></span> <span data-ttu-id="e3f7d-112">Os usuários não podem acessar mais itens em uma pesquisa do que na API de enumeração.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-112">Users cannot access more items in a search than they can from the enumeration API.</span></span>

| <span data-ttu-id="e3f7d-113">Casos de uso</span><span class="sxs-lookup"><span data-stu-id="e3f7d-113">Use cases</span></span> | <span data-ttu-id="e3f7d-114">Propriedades a serem definidas no corpo da solicitação de consulta</span><span class="sxs-lookup"><span data-stu-id="e3f7d-114">Properties to define in the query request body</span></span> |
|:------------------|:---------|
|[<span data-ttu-id="e3f7d-115">Pesquisa de escopo com base em tipos de entidade</span><span class="sxs-lookup"><span data-stu-id="e3f7d-115">Scope search based on entity types</span></span>](#scope-search-based-on-entity-types)| <span data-ttu-id="e3f7d-116">**entityTypes**</span><span class="sxs-lookup"><span data-stu-id="e3f7d-116">**entityTypes**</span></span> |
|[<span data-ttu-id="e3f7d-117">Resultados da página</span><span class="sxs-lookup"><span data-stu-id="e3f7d-117">Page results</span></span>](#page-search-results) | <span data-ttu-id="e3f7d-118">**from** e **size**</span><span class="sxs-lookup"><span data-stu-id="e3f7d-118">**from** and **size**</span></span> |
|[<span data-ttu-id="e3f7d-119">Obter os emails mais relevantes</span><span class="sxs-lookup"><span data-stu-id="e3f7d-119">Get the most relevant emails</span></span>](#get-the-most-relevant-emails) | <span data-ttu-id="e3f7d-120">**enableTopResults**</span><span class="sxs-lookup"><span data-stu-id="e3f7d-120">**enableTopResults**</span></span> |
|[<span data-ttu-id="e3f7d-121">Obter as propriedades selecionadas</span><span class="sxs-lookup"><span data-stu-id="e3f7d-121">Get selected properties</span></span>](#get-selected-properties) | <span data-ttu-id="e3f7d-122">**stored_fields**</span><span class="sxs-lookup"><span data-stu-id="e3f7d-122">**stored_fields**</span></span> |
|[<span data-ttu-id="e3f7d-123">Usar KQL em termos de consulta</span><span class="sxs-lookup"><span data-stu-id="e3f7d-123">Use KQL in query terms</span></span>](#keyword-query-language-kql-support) | <span data-ttu-id="e3f7d-124">**query**</span><span class="sxs-lookup"><span data-stu-id="e3f7d-124">**query**</span></span> |
|[<span data-ttu-id="e3f7d-125">Pesquisar arquivos externos</span><span class="sxs-lookup"><span data-stu-id="e3f7d-125">Search external Files</span></span>](/graph/search-concept-files)| <span data-ttu-id="e3f7d-126">**entityTypes**</span><span class="sxs-lookup"><span data-stu-id="e3f7d-126">**entityTypes**</span></span> |
|[<span data-ttu-id="e3f7d-127">Pesquisar em um contentSource específico (API de indexação)</span><span class="sxs-lookup"><span data-stu-id="e3f7d-127">Search within a specific contentSource (indexing API)</span></span>](/graph/search-concept-custom-types)| <span data-ttu-id="e3f7d-128">**contentSources**</span><span class="sxs-lookup"><span data-stu-id="e3f7d-128">**contentSources**</span></span> |

### <a name="scope-search-based-on-entity-types"></a><span data-ttu-id="e3f7d-129">Pesquisa de escopo com base em tipos de entidade</span><span class="sxs-lookup"><span data-stu-id="e3f7d-129">Scope search based on entity types</span></span>

<span data-ttu-id="e3f7d-130">Defina o escopo da solicitação de pesquisa usando a propriedade **entityTypes** no conteúdo da solicitação **query**.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-130">Define the scope of the search request using the **entityTypes** property in the **query** request payload.</span></span>
<span data-ttu-id="e3f7d-131">Estes são os tipos de entidade com suporte:</span><span class="sxs-lookup"><span data-stu-id="e3f7d-131">The following are the supported entity types:</span></span>

- [<span data-ttu-id="e3f7d-132">event</span><span class="sxs-lookup"><span data-stu-id="e3f7d-132">event</span></span>](event.md)
- [<span data-ttu-id="e3f7d-133">message</span><span class="sxs-lookup"><span data-stu-id="e3f7d-133">message</span></span>](message.md)
- [<span data-ttu-id="e3f7d-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="e3f7d-134">driveItem</span></span>](driveitem.md)
- [<span data-ttu-id="e3f7d-135">externalFile</span><span class="sxs-lookup"><span data-stu-id="e3f7d-135">externalFile</span></span>](externalfile.md)
- [<span data-ttu-id="e3f7d-136">externalItem</span><span class="sxs-lookup"><span data-stu-id="e3f7d-136">externalItem</span></span>](externalitem.md)

### <a name="page-search-results"></a><span data-ttu-id="e3f7d-137">Resultados da pesquisa de página</span><span class="sxs-lookup"><span data-stu-id="e3f7d-137">Page search results</span></span>

<span data-ttu-id="e3f7d-138">Para controlar a paginação dos resultados da pesquisa, especifique as duas seguintes propriedades no corpo da solicitação **query**:</span><span class="sxs-lookup"><span data-stu-id="e3f7d-138">Control pagination of the search results by specifying the following two properties in the **query** request body:</span></span>

- <span data-ttu-id="e3f7d-139">**from** – um número inteiro que indica o ponto de partida baseado em 0 para listar os resultados da pesquisa na página.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-139">**from** - An integer that indicates the 0-based starting point to list search results on the page.</span></span> <span data-ttu-id="e3f7d-140">O valor padrão é 0.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-140">The default value is 0.</span></span>

- <span data-ttu-id="e3f7d-141">**size** – um número inteiro que indica o número de resultados a serem retornados para uma página.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-141">**size** - An integer that indicates the number of results to be returned for a page.</span></span> <span data-ttu-id="e3f7d-142">O valor padrão é 25.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-142">The default value is 25.</span></span>

<span data-ttu-id="e3f7d-143">Observe os seguintes limites se você estiver pesquisando a entidade **event** ou **message**:</span><span class="sxs-lookup"><span data-stu-id="e3f7d-143">Note the following limits if you're searching the **event** or **message** entity:</span></span>

- <span data-ttu-id="e3f7d-144">**from** deve começar em zero na primeira solicitação de página; caso contrário, a solicitação resultará em um HTTP 400 `Bad request`.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-144">**from** must start at zero in the first page request; otherwise, the request results in an HTTP 400 `Bad request`.</span></span>
- <span data-ttu-id="e3f7d-145">O máximo de resultados por página (**size**) é 200.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-145">The maximum results per page (**size**) is 200.</span></span>
- <span data-ttu-id="e3f7d-146">O número máximo total de itens que podem ser retornados por meio de paginação é 1000.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-146">The maximum total number of items that can be returned by paginating is 1000.</span></span>
- <span data-ttu-id="e3f7d-147">Se os limites forem excedidos, será retornada uma resposta de melhor esforço.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-147">Going beyond the limits returns a best effort response.</span></span> <span data-ttu-id="e3f7d-148">A solicitação não resulta em um HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-148">The request does not result in an HTTP 400.</span></span>

<span data-ttu-id="e3f7d-149">Práticas recomendadas:</span><span class="sxs-lookup"><span data-stu-id="e3f7d-149">Best practices:</span></span>

- <span data-ttu-id="e3f7d-150">Especifique uma primeira página menor na solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-150">Specify a smaller first page in the initial request.</span></span> <span data-ttu-id="e3f7d-151">Por exemplo, especifique **from** como 0 e **size** como 25.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-151">For example, specify **from** as 0, **size** as 25.</span></span>
- <span data-ttu-id="e3f7d-152">Pagine as páginas subsequentes atualizando as propriedades **from** e **size**.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-152">Paginate subsequent pages by updating the **from** and **size** properties.</span></span> <span data-ttu-id="e3f7d-153">Você pode aumentar o tamanho de página em cada solicitação subsequente.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-153">You can increase the page size in each subsequent request.</span></span> <span data-ttu-id="e3f7d-154">A tabela a seguir mostra um exemplo.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-154">The following table shows an example.</span></span>

    | <span data-ttu-id="e3f7d-155">Página</span><span class="sxs-lookup"><span data-stu-id="e3f7d-155">Page</span></span> | <span data-ttu-id="e3f7d-156">from</span><span class="sxs-lookup"><span data-stu-id="e3f7d-156">from</span></span> | <span data-ttu-id="e3f7d-157">size</span><span class="sxs-lookup"><span data-stu-id="e3f7d-157">size</span></span> |
    |:-----|:-----|:-----|
    | <span data-ttu-id="e3f7d-158">1</span><span class="sxs-lookup"><span data-stu-id="e3f7d-158">1</span></span>    | <span data-ttu-id="e3f7d-159">0</span><span class="sxs-lookup"><span data-stu-id="e3f7d-159">0</span></span> | <span data-ttu-id="e3f7d-160">25</span><span class="sxs-lookup"><span data-stu-id="e3f7d-160">25</span></span> |
    | <span data-ttu-id="e3f7d-161">2</span><span class="sxs-lookup"><span data-stu-id="e3f7d-161">2</span></span>    | <span data-ttu-id="e3f7d-162">25</span><span class="sxs-lookup"><span data-stu-id="e3f7d-162">25</span></span> | <span data-ttu-id="e3f7d-163">50</span><span class="sxs-lookup"><span data-stu-id="e3f7d-163">50</span></span> |
    | <span data-ttu-id="e3f7d-164">3</span><span class="sxs-lookup"><span data-stu-id="e3f7d-164">3</span></span>    | <span data-ttu-id="e3f7d-165">75</span><span class="sxs-lookup"><span data-stu-id="e3f7d-165">75</span></span> | <span data-ttu-id="e3f7d-166">75</span><span class="sxs-lookup"><span data-stu-id="e3f7d-166">75</span></span> |
    | <span data-ttu-id="e3f7d-167">4</span><span class="sxs-lookup"><span data-stu-id="e3f7d-167">4</span></span>    | <span data-ttu-id="e3f7d-168">150</span><span class="sxs-lookup"><span data-stu-id="e3f7d-168">150</span></span> | <span data-ttu-id="e3f7d-169">100</span><span class="sxs-lookup"><span data-stu-id="e3f7d-169">100</span></span> |

### <a name="get-the-most-relevant-emails"></a><span data-ttu-id="e3f7d-170">Obter os emails mais relevantes</span><span class="sxs-lookup"><span data-stu-id="e3f7d-170">Get the most relevant emails</span></span>

<span data-ttu-id="e3f7d-171">Quando você pesquisa na entidade **message**, a especificação de **enableTopResults** como `true` retorna uma lista híbrida de mensagens: as três primeiras mensagens na resposta são classificadas por relevância; as mensagens restantes são classificadas por data.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-171">When searching the **message** entity, specifying **enableTopResults** as `true` returns a hybrid list of messages: the first three messages in the response are sorted by relevance; the remaining messages are sorted by date.</span></span>

### <a name="get-selected-properties"></a><span data-ttu-id="e3f7d-172">Obter as propriedades selecionadas</span><span class="sxs-lookup"><span data-stu-id="e3f7d-172">Get selected properties</span></span>

<span data-ttu-id="e3f7d-173">Ao pesquisar em uma entidade **externalItem**, use a propriedade **stored_fields** para especificar os campos a serem retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-173">When searching an **externalItem** entity, use the **stored_fields** property to specify the fields to be returned in the response.</span></span>

<span data-ttu-id="e3f7d-174">Os campos especificados em **stored_fields** devem ser propriedades gerenciadas recuperáveis que foram configuradas para a conexão por meio da administração de locatário da Pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-174">The fields specified in **stored_fields** should be retrievable managed properties that have been configured for the connection via the Microsoft Search tenant administration.</span></span>

### <a name="keyword-query-language-kql-support"></a><span data-ttu-id="e3f7d-175">Suporte a KQL (Linguagem de Consulta de Palavra-chave)</span><span class="sxs-lookup"><span data-stu-id="e3f7d-175">Keyword Query Language (KQL) support</span></span>

<span data-ttu-id="e3f7d-176">Especifique palavras-chave de texto livre, operadores (como `AND`, `OR`) e restrições de propriedade na sintaxe KQL na cadeia de caracteres de consulta de pesquisa real (propriedade **query** do corpo da solicitação **query**).</span><span class="sxs-lookup"><span data-stu-id="e3f7d-176">Specify free text keywords, operators (such as `AND`, `OR`), and property restrictions in KQL syntax in the actual search query string (**query** property of the **query** request body).</span></span> <span data-ttu-id="e3f7d-177">A sintaxe e o comando dependem dos tipos de entidade (na propriedade **entityTypes**) que você direciona no corpo da solicitação **query**.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-177">The syntax and command depend on the entity types (in the **entityTypes** property) you target in the same **query** request body.</span></span>

<span data-ttu-id="e3f7d-178">Dependendo do tipo de entidade, as propriedades pesquisáveis variam.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-178">Depending on the entity type, the searchable properties vary.</span></span> <span data-ttu-id="e3f7d-179">Veja mais detalhes em:</span><span class="sxs-lookup"><span data-stu-id="e3f7d-179">For details, see:</span></span>

- [<span data-ttu-id="e3f7d-180">Propriedades do email</span><span class="sxs-lookup"><span data-stu-id="e3f7d-180">Email properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [<span data-ttu-id="e3f7d-181">Propriedades do site</span><span class="sxs-lookup"><span data-stu-id="e3f7d-181">Site properties</span></span>](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="error-handling"></a><span data-ttu-id="e3f7d-182">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="e3f7d-182">Error handling</span></span>

<span data-ttu-id="e3f7d-183">A API de pesquisa retorna respostas de erro conforme estipulado pela [definição de objeto de erro OData](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse). Cada uma delas é um objeto JSON que contém um código e uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-183">The search API returns error responses as defined by [OData error object definition](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse), each of which is a JSON object containing a code and a message.</span></span>

<!---TODO Describe the know errors : bad requests.--->

## <a name="known-limitations"></a><span data-ttu-id="e3f7d-184">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="e3f7d-184">Known limitations</span></span>

<span data-ttu-id="e3f7d-185">A API de pesquisa tem as seguintes limitações:</span><span class="sxs-lookup"><span data-stu-id="e3f7d-185">The search API has the following limitations:</span></span>

- <span data-ttu-id="e3f7d-186">O método **query** é definido para permitir a passagem de um conjunto de uma ou mais instâncias de **searchRequest** de uma só vez.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-186">The **query** method is defined to allow passing a collection of one or more **searchRequest** instances at once.</span></span> <span data-ttu-id="e3f7d-187">No entanto, atualmente o serviço dá suporte apenas a um único [searchRequest](./searchrequest.md) por vez.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-187">However, the service currently supports only a single [searchRequest](./searchrequest.md) at a time.</span></span>

- <span data-ttu-id="e3f7d-188">O recurso [searchRequest](./searchrequest.md) dá suporte à passagem de vários tipos de entidades por vez.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-188">The [searchRequest](./searchrequest.md) resource supports passing multiple types of entities at a time.</span></span> <span data-ttu-id="e3f7d-189">No entanto, atualmente a única combinação com suporte é **driveItem** e **externalfile**.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-189">However, currently the only supported combination is **driveItem** and **externalFile**.</span></span> <span data-ttu-id="e3f7d-190">Outras combinações são inválidas.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-190">Other combinations are invalid.</span></span>

- <span data-ttu-id="e3f7d-191">A propriedade **contentSource**, que define a conexão a ser usada, só será aplicável quando **entityType** for especificada como `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-191">The **contentSource** property, which defines the connection to use, is only applicable when **entityType** is specified as `externalItem`.</span></span>
<!--todo nmoreauteam Fix the link to ContentSource  pls provide the content source url--->

- <span data-ttu-id="e3f7d-192">A API de pesquisa não dá suporte à classificação personalizada e sempre classifica os resultados da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="e3f7d-192">The search API does not support custom sort and always sorts results in the following ways:</span></span>

  - <span data-ttu-id="e3f7d-193">Classificar resultados dos tipos **message** ou **event** por data.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-193">Sort **message** or **event** type results by date.</span></span>

  - <span data-ttu-id="e3f7d-194">Classificar resultados dos tipos **driveItem**, **externalfile** ou **externalItem** por relevância.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-194">Sort **driveItem**, **externalFile**, or **externalItem** type results by relevance.</span></span>

## <a name="whats-new"></a><span data-ttu-id="e3f7d-195">O que há de novo</span><span class="sxs-lookup"><span data-stu-id="e3f7d-195">What's new</span></span>
<span data-ttu-id="e3f7d-196">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="e3f7d-196">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>


