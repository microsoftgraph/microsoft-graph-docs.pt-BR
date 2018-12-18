---
title: Usar parâmetros de consulta para personalizar respostas
description: O Microsoft Graph fornece parâmetros de consulta opcional que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta. Há suporte para os parâmetros de consulta a seguir.
author: piotrci
ms.openlocfilehash: 6cdc4ce0f502e941e24a6197e7ba4b65cac13b20
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311834"
---
# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="70d1a-104">Usar parâmetros de consulta para personalizar respostas</span><span class="sxs-lookup"><span data-stu-id="70d1a-104">Use query parameters to customize responses</span></span>

<span data-ttu-id="70d1a-105">O Microsoft Graph fornece suporte a parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="70d1a-105">Microsoft Graph supports optional query parameters that you can use to specify and control the amount of data returned in a response.</span></span> <span data-ttu-id="70d1a-106">O suporte para os parâmetros de consulta exatos variam de uma operação de API para outra e, dependendo da API, podem diferir entre os pontos de extremidade v1.0 e beta.</span><span class="sxs-lookup"><span data-stu-id="70d1a-106">The support for the exact query parameters varies from one API operation to another, and depending on the API, can differ between the v1.0 and beta endpoints.</span></span> 

> <span data-ttu-id="70d1a-107">**Observação:** nos pontos de extremidade v1.0 e beta, o prefixo `$` é opcional.</span><span class="sxs-lookup"><span data-stu-id="70d1a-107">**Note:** On the v1.0 and beta endpoints, the `$` prefix is optional.</span></span> <span data-ttu-id="70d1a-108">Por exemplo, em vez de `$filter`, você pode usar `filter`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-108">For example, instead of `$filter`, you can use `filter`.</span></span>

<span data-ttu-id="70d1a-109">Os parâmetros de consulta podem ser opções de consulta de sistema OData ou outros parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="70d1a-109">Query parameters can be OData system query options or other query parameters.</span></span> 

## <a name="odata-system-query-options"></a><span data-ttu-id="70d1a-110">Opções de consulta de sistema OData</span><span class="sxs-lookup"><span data-stu-id="70d1a-110">OData system query options</span></span>
<span data-ttu-id="70d1a-111">Uma operação de API do Microsoft Graph pode oferecer suporte a uma ou mais das seguintes opções de consulta de sistema OData.</span><span class="sxs-lookup"><span data-stu-id="70d1a-111">A Microsoft Graph API operation might support one or more of the following OData system query options.</span></span> <span data-ttu-id="70d1a-112">Essas opções de consulta são compatíveis com a [linguagem de consulta OData V4][odata-query].</span><span class="sxs-lookup"><span data-stu-id="70d1a-112">These query options are compatible with the [OData V4 query language][odata-query].</span></span>

><span data-ttu-id="70d1a-113">**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="70d1a-113">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="70d1a-114">Nome</span><span class="sxs-lookup"><span data-stu-id="70d1a-114">Name</span></span>                     | <span data-ttu-id="70d1a-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="70d1a-115">Description</span></span> | <span data-ttu-id="70d1a-116">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70d1a-116">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="70d1a-117">$count</span><span class="sxs-lookup"><span data-stu-id="70d1a-117">$count</span></span>](#count-parameter)         | <span data-ttu-id="70d1a-118">Recupera a contagem total de recursos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="70d1a-118">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="70d1a-119">$expand</span><span class="sxs-lookup"><span data-stu-id="70d1a-119">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="70d1a-120">Recupera os recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="70d1a-120">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="70d1a-121">$filter</span><span class="sxs-lookup"><span data-stu-id="70d1a-121">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="70d1a-122">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="70d1a-122">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="70d1a-123">$format</span><span class="sxs-lookup"><span data-stu-id="70d1a-123">$format</span></span>](#format-parameter)       | <span data-ttu-id="70d1a-124">Retorna os resultados no formato de mídia especificado.</span><span class="sxs-lookup"><span data-stu-id="70d1a-124">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="70d1a-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="70d1a-125">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="70d1a-126">Ordena os resultados.</span><span class="sxs-lookup"><span data-stu-id="70d1a-126">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="70d1a-127">$search</span><span class="sxs-lookup"><span data-stu-id="70d1a-127">$search</span></span>](#search-parameter)       | <span data-ttu-id="70d1a-p105">Retorna os resultados com base nos critérios de pesquisa. Atualmente, com suporte em conjuntos de **mensagens** e **pessoa**.</span><span class="sxs-lookup"><span data-stu-id="70d1a-p105">Returns results based on search criteria. Currently supported on **messages** and **person** collections.</span></span>|[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="70d1a-130">$select</span><span class="sxs-lookup"><span data-stu-id="70d1a-130">$select</span></span>](#select-parameter)       | <span data-ttu-id="70d1a-131">Filtra as propriedades (colunas).</span><span class="sxs-lookup"><span data-stu-id="70d1a-131">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="70d1a-132">$skip</span><span class="sxs-lookup"><span data-stu-id="70d1a-132">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="70d1a-p106">Índices em um conjunto de resultados. Também usado por algumas APIs para implementar a paginação e pode ser usado com `$top` para paginar resultados manualmente.</span><span class="sxs-lookup"><span data-stu-id="70d1a-p106">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="70d1a-135">$top</span><span class="sxs-lookup"><span data-stu-id="70d1a-135">$top</span></span>](#top-parameter)             | <span data-ttu-id="70d1a-136">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="70d1a-136">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a><span data-ttu-id="70d1a-137">Outros parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="70d1a-137">Other query parameters</span></span>

| <span data-ttu-id="70d1a-138">Nome</span><span class="sxs-lookup"><span data-stu-id="70d1a-138">Name</span></span>                     | <span data-ttu-id="70d1a-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="70d1a-139">Description</span></span> | <span data-ttu-id="70d1a-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70d1a-140">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="70d1a-141">$skipToken</span><span class="sxs-lookup"><span data-stu-id="70d1a-141">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="70d1a-p107">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas. (Algumas APIs usam `$skip` em vez disso.)</span><span class="sxs-lookup"><span data-stu-id="70d1a-p107">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="encoding-query-parameters"></a><span data-ttu-id="70d1a-144">Codificação de parâmetros da consulta</span><span class="sxs-lookup"><span data-stu-id="70d1a-144">Encoding query parameters</span></span>

<span data-ttu-id="70d1a-145">Os valores dos parâmetros da consulta devem ser codificados por porcentagem.</span><span class="sxs-lookup"><span data-stu-id="70d1a-145">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="70d1a-146">Muitas ferramentas, navegadores e clientes HTTP (como o [Explorador do Graph][graph-explorer]) ajudarão você com isso.</span><span class="sxs-lookup"><span data-stu-id="70d1a-146">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="70d1a-147">Se uma consulta está falhando, uma causa possível é a falha na codificação adequada dos valores dos parâmetros da consulta.</span><span class="sxs-lookup"><span data-stu-id="70d1a-147">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="70d1a-148">Uma URL descodificada é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="70d1a-148">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="70d1a-149">Uma URL codificada adequadamente é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="70d1a-149">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count-parameter"></a><span data-ttu-id="70d1a-150">parâmetro count</span><span class="sxs-lookup"><span data-stu-id="70d1a-150">count parameter</span></span>

<span data-ttu-id="70d1a-151">Use o parâmetro de consulta `$count` para incluir uma contagem do número total de itens em um conjunto, juntamente com a página de valores de dados retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="70d1a-151">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="70d1a-152">Por exemplo, a solicitação a seguir retornará o conjunto **contato** do usuário atual e o número de itens no conjunto **contato** na propriedade `@odata.count`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-152">For example, the following request will return both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="70d1a-153">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="70d1a-153">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="70d1a-154">**Observação:** `$count` não tem suporte para conjuntos de recursos derivados de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), como conjuntos de [usuários](/graph/api/resources/user?view=graph-rest-1.0) ou [grupos](/graph/api/resources/group?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="70d1a-154">**Note:** `$count` is not supported for collections of resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) like collections of [users](/graph/api/resources/user?view=graph-rest-1.0) or [groups](/graph/api/resources/group?view=graph-rest-1.0).</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="70d1a-155">parâmetro expand</span><span class="sxs-lookup"><span data-stu-id="70d1a-155">expand parameter</span></span>

<span data-ttu-id="70d1a-156">Muitos recursos do Microsoft Graph expõem as propriedades declaradas do recurso, bem como as relações delas com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="70d1a-156">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="70d1a-157">Essas relações também são chamadas de propriedades de referência ou propriedades de navegação e podem fazer referência a um único recurso ou a um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="70d1a-157">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="70d1a-158">Por exemplo, as pastas de email, gerente e subordinados diretos de um usuário são todas expostas como relações.</span><span class="sxs-lookup"><span data-stu-id="70d1a-158">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="70d1a-p110">Normalmente, você pode consultar as propriedades de um recurso ou uma de suas relações em uma única solicitação, mas não ambas. Você pode usar o parâmetro de cadeia de caracteres de consulta `$expand` para incluir o recurso expandido ou o conjunto referenciado por uma única relação (propriedade de navegação) nos resultados.</span><span class="sxs-lookup"><span data-stu-id="70d1a-p110">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="70d1a-161">O seguinte exemplo obtém informações de unidade raiz juntamente com os itens filho de nível superior em uma unidade:</span><span class="sxs-lookup"><span data-stu-id="70d1a-161">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="70d1a-162">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="70d1a-162">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="70d1a-p111">Com alguns conjuntos de recursos, você também pode especificar as propriedades a serem retornadas nos recursos expandidos adicionando um parâmetro `$select`. O exemplo a seguir executa a mesma consulta que o exemplo anterior, mas usa uma instrução [`$select`](#select-parameter) para limitar as propriedades retornadas para os itens filho expandidos para as propriedades **id** e **name**.</span><span class="sxs-lookup"><span data-stu-id="70d1a-p111">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="70d1a-165">[Experimentar no Explorador do Graph][expand-example]</span><span class="sxs-lookup"><span data-stu-id="70d1a-165">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="70d1a-p112">**Observação:** nem todas as relações e recursos dão suporte ao parâmetro de consulta `$expand`. Por exemplo, você pode expandir as relações **directReports**, **manager** e **memberOf** em um usuário, mas não pode expandir suas relações **events**, **messages** ou **photo**. Nem todos os recursos ou relações dão suporte ao uso de `$select` em itens expandidos.</span><span class="sxs-lookup"><span data-stu-id="70d1a-p112">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="70d1a-169">Com recursos do Azure AD derivados de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), como [user](/graph/api/resources/user?view=graph-rest-1.0) e [group](/graph/api/resources/group?view=graph-rest-1.0), `$expand` só há suporte para `beta`, e normalmente são retornados no máximo 20 itens para a relação expandida.</span><span class="sxs-lookup"><span data-stu-id="70d1a-169">With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="70d1a-170">parâmetro filter</span><span class="sxs-lookup"><span data-stu-id="70d1a-170">filter parameter</span></span>

<span data-ttu-id="70d1a-171">Use o parâmetro de consulta `$filter` para recuperar apenas um subconjunto de um conjunto.</span><span class="sxs-lookup"><span data-stu-id="70d1a-171">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="70d1a-172">Por exemplo, para localizar os usuários cujo nome de exibição se inicia com a letra "J", use `startswith`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-172">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="70d1a-173">[Experimentar no Explorador do Graph][filter-example]</span><span class="sxs-lookup"><span data-stu-id="70d1a-173">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="70d1a-174">O suporte para operadores `$filter` varia entre as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="70d1a-174">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="70d1a-175">Os seguintes operadores lógicos geralmente são suportados:</span><span class="sxs-lookup"><span data-stu-id="70d1a-175">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="70d1a-176">igual a (`eq`)</span><span class="sxs-lookup"><span data-stu-id="70d1a-176">equals (`eq`)</span></span>
- <span data-ttu-id="70d1a-177">não é igual a (`ne`)</span><span class="sxs-lookup"><span data-stu-id="70d1a-177">not equals (`ne`)</span></span>
- <span data-ttu-id="70d1a-178">maior que (`gt`)</span><span class="sxs-lookup"><span data-stu-id="70d1a-178">greater than (`gt`)</span></span>
- <span data-ttu-id="70d1a-179">maior ou igual a (`ge`)</span><span class="sxs-lookup"><span data-stu-id="70d1a-179">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="70d1a-180">menor que (`lt`), menor ou igual a (`le`)</span><span class="sxs-lookup"><span data-stu-id="70d1a-180">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="70d1a-181">e (`and`)</span><span class="sxs-lookup"><span data-stu-id="70d1a-181">and (`and`)</span></span>
- <span data-ttu-id="70d1a-182">ou (`or`)</span><span class="sxs-lookup"><span data-stu-id="70d1a-182">or (`or`)</span></span>
- <span data-ttu-id="70d1a-183">não (`not`)</span><span class="sxs-lookup"><span data-stu-id="70d1a-183">not (`not`)</span></span>
 
<span data-ttu-id="70d1a-184">O operador de cadeia de caracteres `startswith` geralmente é suportado.</span><span class="sxs-lookup"><span data-stu-id="70d1a-184">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="70d1a-185">O operador lambda `any` tem suporte em algumas APIs.</span><span class="sxs-lookup"><span data-stu-id="70d1a-185">The `any` lambda operator is supported for some APIs.</span></span> <span data-ttu-id="70d1a-186">Para ver alguns exemplos de uso, confira a tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="70d1a-186">For some  usage examples, see the following table.</span></span> <span data-ttu-id="70d1a-187">Para obter mais detalhes sobre a sintaxe `$filter`, confira o [protocolo OData][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="70d1a-187">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="70d1a-188">A tabela a seguir mostra alguns exemplos que usam o parâmetro de consulta `$filter`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-188">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="70d1a-189">**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="70d1a-189">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="70d1a-190">Descrição</span><span class="sxs-lookup"><span data-stu-id="70d1a-190">Description</span></span> | <span data-ttu-id="70d1a-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70d1a-191">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="70d1a-192">Pesquisar por usuários com o nome Clara entre várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="70d1a-192">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| <span data-ttu-id="70d1a-193">Obter todos os eventos do usuário conectado que começaram após 01/07/2017.</span><span class="sxs-lookup"><span data-stu-id="70d1a-193">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| <span data-ttu-id="70d1a-194">Obter todos os emails de um endereço específico recebidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="70d1a-194">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| <span data-ttu-id="70d1a-195">Obter todos os emails recebidos pelo usuário conectado em abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="70d1a-195">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| <span data-ttu-id="70d1a-196">Obter todos os emails não lidos na caixa de entrada do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="70d1a-196">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| <span data-ttu-id="70d1a-197">Listar todos os grupos do Office 365 em uma organização.</span><span class="sxs-lookup"><span data-stu-id="70d1a-197">List all Office 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> <span data-ttu-id="70d1a-p115">**Observação:** Os seguintes operadores `$filter` não têm suporte para recursos do Azure AD: `ne`, `gt`, `ge`, `lt`, `le` e `not`. O operador de cadeia de caracteres `contains` atualmente não tem suporte em nenhum recurso do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="70d1a-p115">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="70d1a-200">parâmetro format</span><span class="sxs-lookup"><span data-stu-id="70d1a-200">format parameter</span></span>

<span data-ttu-id="70d1a-201">Use o parâmetro de consulta `$format` para especificar o formato de mídia dos itens retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="70d1a-201">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="70d1a-202">Por exemplo, a seguinte solicitação retorna os usuários na organização no formato json:</span><span class="sxs-lookup"><span data-stu-id="70d1a-202">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="70d1a-203">[Experimentar no Explorador do Graph][format-example]</span><span class="sxs-lookup"><span data-stu-id="70d1a-203">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="70d1a-204">**Observação:** o parâmetro de consulta `$format` é compatível com vários formatos (por exemplo, atom, xml e json), mas os resultados podem não ser retornados em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="70d1a-204">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="70d1a-205">parâmetro orderby</span><span class="sxs-lookup"><span data-stu-id="70d1a-205">orderby parameter</span></span>

<span data-ttu-id="70d1a-206">Use o parâmetro de consulta `$orderby` para especificar a ordem de classificação dos itens retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="70d1a-206">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="70d1a-207">Por exemplo, a solicitação a seguir retorna os usuários da organização ordenados por seu nome de exibição:</span><span class="sxs-lookup"><span data-stu-id="70d1a-207">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="70d1a-208">[Experimentar no Explorador do Graph][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="70d1a-208">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="70d1a-p116">Você também pode classificar por entidades de tipo complexo. A solicitação abaixo obtém mensagens e as classifica pelo campo **address** da propriedade **from**, que é do tipo complexo **emailAddress**:</span><span class="sxs-lookup"><span data-stu-id="70d1a-p116">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="70d1a-211">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="70d1a-211">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="70d1a-212">Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-212">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="70d1a-213">Com algumas APIs, você pode ordenar os resultados em várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="70d1a-213">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="70d1a-214">Por exemplo, a solicitação a seguir ordena as mensagens na caixa de entrada do usuário primeiro pelo nome da pessoa que enviou, em ordem decrescente (Z – A) e, em seguida, por assunto, em ordem ascendente (padrão).</span><span class="sxs-lookup"><span data-stu-id="70d1a-214">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="70d1a-215">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="70d1a-215">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

<span data-ttu-id="70d1a-216">Quando você especifica $filter, servidor deduz uma ordem de classificação para os resultados.</span><span class="sxs-lookup"><span data-stu-id="70d1a-216">When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="70d1a-217">Se você usar `$orderby` e `$filter`, como o servidor sempre deduz a ordem de classificação dos resultados de um `$filter`, as propriedades do `$filter` devem estar listadas primeiro no `$orderby` antes de outras propriedades e devem estar listadas na ordem que aparecem no parâmetro `$filter`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-217">If you use both `$orderby` and `$filter`, because the server always infers a sort order for the results of a `$filter`, the properties in the `$filter` must be listed first in the `$orderby` before any other properties, and they must be listed in the order that they appear in the `$filter` parameter.</span></span> 

<span data-ttu-id="70d1a-218">O exemplo a seguir mostra uma consulta filtrada pelas propriedades **subject** e **priority** e classificadas pelas propriedades **subject**, **priority** e **receivedDateTime** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="70d1a-218">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="70d1a-219">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="70d1a-219">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > <span data-ttu-id="70d1a-220">**Observação:** Com os recursos do Azure AD derivados de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), como [user](/graph/api/resources/user?view=graph-rest-1.0) e [group](/graph/api/resources/group?view=graph-rest-1.0), você não pode combinar `$orderby` a expressões `$filter`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-220">**Note:** With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search-parameter"></a><span data-ttu-id="70d1a-221">parâmetro search</span><span class="sxs-lookup"><span data-stu-id="70d1a-221">search parameter</span></span>

<span data-ttu-id="70d1a-222">Use o parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="70d1a-222">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="70d1a-p119">**Observação:** Atualmente, é possível pesquisar **somente** coleções de [mensagens](/graph/api/resources/message?view=graph-rest-1.0) e [pessoas](/graph/api/resources/person?view=graph-rest-1.0). Uma solicitação de `$search` retorna até 250 resultados. Não é possível usar [`$filter`](#filter-parameter) ou [`$orderby`](#orderby-parameter) em uma solicitação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="70d1a-p119">**Note:** You can currently search **only** [message](/graph/api/resources/message?view=graph-rest-1.0) and [person](/graph/api/resources/person?view=graph-rest-1.0) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter-parameter) or [`$orderby`](#orderby-parameter) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="70d1a-226">Usando $search em conjuntos de mensagens</span><span class="sxs-lookup"><span data-stu-id="70d1a-226">Using $search on message collections</span></span>

<span data-ttu-id="70d1a-227">Você pode pesquisar mensagens com base em um valor nas propriedades de mensagens específicas.</span><span class="sxs-lookup"><span data-stu-id="70d1a-227">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="70d1a-228">Os resultados da pesquisa são classificados pela data e hora em que a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="70d1a-228">The results of the search are sorted by the date and time that the message was sent.</span></span>

<span data-ttu-id="70d1a-229">Se você realizar uma pesquisa em mensagens e especificar apenas um valor sem as propriedades de mensagens específicas, a pesquisa será realizada nas propriedades de pesquisa padrão **from**, **subject** e **body**.</span><span class="sxs-lookup"><span data-stu-id="70d1a-229">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="70d1a-230">O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:</span><span class="sxs-lookup"><span data-stu-id="70d1a-230">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="70d1a-231">[Experimentar no Explorador do Graph][search-example]</span><span class="sxs-lookup"><span data-stu-id="70d1a-231">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="70d1a-232">Como alternativa, você pode pesquisar mensagens especificando os nomes de propriedade da mensagem na tabela a seguir, que são reconhecidos pela sintaxe da Linguagem de Consulta de Palavra-chave (KQL).</span><span class="sxs-lookup"><span data-stu-id="70d1a-232">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="70d1a-233">Esses nomes de propriedades correspondem às propriedades definidas na entidade **mensagem** do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="70d1a-233">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="70d1a-234">O Outlook e outros aplicativos do Office 365, como o SharePoint, oferecem suporte à sintaxe KQL, proporcionando a conveniência de um domínio de descoberta comum para os repositórios de dados.</span><span class="sxs-lookup"><span data-stu-id="70d1a-234">Outlook and other Office 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="70d1a-235">Propriedades de emails pesquisáveis</span><span class="sxs-lookup"><span data-stu-id="70d1a-235">Searchable email property</span></span>                | <span data-ttu-id="70d1a-236">Descrição</span><span class="sxs-lookup"><span data-stu-id="70d1a-236">Description</span></span> | <span data-ttu-id="70d1a-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70d1a-237">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="70d1a-238">**attachment**</span><span class="sxs-lookup"><span data-stu-id="70d1a-238">**attachment**</span></span>           | <span data-ttu-id="70d1a-239">Os nomes dos arquivos anexados a uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="70d1a-239">The names of files attached to an email message.</span></span>|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| <span data-ttu-id="70d1a-240">**bcc**</span><span class="sxs-lookup"><span data-stu-id="70d1a-240">**bcc**</span></span>           | <span data-ttu-id="70d1a-241">O campo **Cco** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="70d1a-241">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| <span data-ttu-id="70d1a-242">**body**</span><span class="sxs-lookup"><span data-stu-id="70d1a-242">**body**</span></span>           | <span data-ttu-id="70d1a-243">O corpo de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="70d1a-243">The body of an email message.</span></span>|[`me/messages?$search="body:excitement"`][search-body-example]
| <span data-ttu-id="70d1a-244">**cc**</span><span class="sxs-lookup"><span data-stu-id="70d1a-244">**cc**</span></span>           | <span data-ttu-id="70d1a-245">O campo **Cc** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="70d1a-245">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| <span data-ttu-id="70d1a-246">**from**</span><span class="sxs-lookup"><span data-stu-id="70d1a-246">**from**</span></span>           | <span data-ttu-id="70d1a-247">O remetente de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="70d1a-247">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| <span data-ttu-id="70d1a-248">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="70d1a-248">**hasAttachment**</span></span> | <span data-ttu-id="70d1a-249">Verdadeiro se uma mensagem de email contiver um anexo que não seja um anexo embutido, caso contrário, falso.</span><span class="sxs-lookup"><span data-stu-id="70d1a-249">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> |[`me/messages?$search="hasAttachments=true"`][search-from-example]
| <span data-ttu-id="70d1a-250">**importance**</span><span class="sxs-lookup"><span data-stu-id="70d1a-250">**importance**</span></span>           | <span data-ttu-id="70d1a-251">A prioridade de uma mensagem de email, que um remetente pode especificar ao enviar uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="70d1a-251">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="70d1a-252">Os valores possíveis são `low`, `medium` ou `high`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-252">The possible values are `low`, `medium`, or `high`.</span></span>|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| <span data-ttu-id="70d1a-253">**kind**</span><span class="sxs-lookup"><span data-stu-id="70d1a-253">**kind**</span></span>           | <span data-ttu-id="70d1a-254">O tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="70d1a-254">The type of message.</span></span> <span data-ttu-id="70d1a-255">Os valores possíveis são `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` ou `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-255">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| <span data-ttu-id="70d1a-256">**participants**</span><span class="sxs-lookup"><span data-stu-id="70d1a-256">**participants**</span></span>           | <span data-ttu-id="70d1a-257">Os campos **de**, **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="70d1a-257">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="participants:danas"`][search-part-example]
| <span data-ttu-id="70d1a-258">**received**</span><span class="sxs-lookup"><span data-stu-id="70d1a-258">**received**</span></span>           | <span data-ttu-id="70d1a-259">A data em que uma mensagem de email foi recebida pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="70d1a-259">The date that an email message was received by a recipient.</span></span>|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| <span data-ttu-id="70d1a-260">**recipients**</span><span class="sxs-lookup"><span data-stu-id="70d1a-260">**recipients**</span></span>           | <span data-ttu-id="70d1a-261">Os campos **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="70d1a-261">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| <span data-ttu-id="70d1a-262">**sent**</span><span class="sxs-lookup"><span data-stu-id="70d1a-262">**sent**</span></span>           | <span data-ttu-id="70d1a-263">A data em que uma mensagem de email foi enviada pelo remetente.</span><span class="sxs-lookup"><span data-stu-id="70d1a-263">The date that an email message was sent by the sender.</span></span>|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| <span data-ttu-id="70d1a-264">**size**</span><span class="sxs-lookup"><span data-stu-id="70d1a-264">**size**</span></span>           | <span data-ttu-id="70d1a-265">O tamanho de um item em bytes.</span><span class="sxs-lookup"><span data-stu-id="70d1a-265">The size of an item in bytes.</span></span>|[`me/messages?$search="size:1..500000"`][search-size-example]
| <span data-ttu-id="70d1a-266">**subject**</span><span class="sxs-lookup"><span data-stu-id="70d1a-266">**subject**</span></span>           | <span data-ttu-id="70d1a-267">O texto na linha de assunto de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="70d1a-267">The text in the subject line of an email message.</span></span> <span data-ttu-id="70d1a-268">.</span><span class="sxs-lookup"><span data-stu-id="70d1a-268">.</span></span>|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| <span data-ttu-id="70d1a-269">**to**</span><span class="sxs-lookup"><span data-stu-id="70d1a-269">**to**</span></span>           | <span data-ttu-id="70d1a-270">O campo **para** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="70d1a-270">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


<span data-ttu-id="70d1a-271">Para saber mais sobre as propriedades de email pesquisáveis, KQL como a sintaxe, operadores com suporte e dicas de pesquisa, confira os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="70d1a-271">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="70d1a-272">[Propriedades pesquisáveis no Exchange](https://docs.microsoft.com/pt-BR/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span><span class="sxs-lookup"><span data-stu-id="70d1a-272">[Searchable properties in Exchange](https://docs.microsoft.com/pt-BR/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- [<span data-ttu-id="70d1a-273">Referência de sintaxe da Linguagem de Consulta de Palavra-chave (KQL)</span><span class="sxs-lookup"><span data-stu-id="70d1a-273">Keyword Query Language (KQL) syntax reference</span></span>](https://docs.microsoft.com/pt-BR/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- <span data-ttu-id="70d1a-274">
  [Propriedades da mensagem e operadores de pesquisa para a Descoberta eletrônica In-loco no Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span><span class="sxs-lookup"><span data-stu-id="70d1a-274">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="70d1a-275">Usando $search em conjuntos de pessoas</span><span class="sxs-lookup"><span data-stu-id="70d1a-275">Using $search on person collections</span></span>

<span data-ttu-id="70d1a-p125">Você pode usar a API de Pessoas do Microsoft Graph para recuperar as pessoas mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. A API de Pessoas dá suporte ao parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-p125">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="70d1a-279">As pesquisas de pessoas ocorrem nas propriedades **displayName** e **emailAddress** do recurso [person](/graph/api/resources/person?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="70d1a-279">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](/graph/api/resources/person?view=graph-rest-1.0) resource.</span></span>

<span data-ttu-id="70d1a-280">A seguinte solicitação faz uma pesquisa por uma pessoa chamada "Clara Barbosa" nas propriedades **displayName** e **emailAddress** em todos os indivíduos no conjunto de **Pessoas** do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="70d1a-280">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="70d1a-281">Como uma pessoa denominada "Clara Barbosa" é relevante para o usuário conectado, as informações para "Clara Barbosa" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="70d1a-281">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="70d1a-282">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="70d1a-282">The following example shows the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

<span data-ttu-id="70d1a-283">Saiba mais sobre a API de Pessoas em [Obter informações sobre pessoas relevantes](./people-example.md#search-people).</span><span class="sxs-lookup"><span data-stu-id="70d1a-283">To learn more about the People API, see [Get information about relevant people](./people-example.md#search-people).</span></span>  

## <a name="select-parameter"></a><span data-ttu-id="70d1a-284">parâmetro select</span><span class="sxs-lookup"><span data-stu-id="70d1a-284">select parameter</span></span>

<span data-ttu-id="70d1a-285">Use o parâmetro de consulta `$select` para retornar um conjunto de propriedades diferente do padrão definido para um recurso individual ou um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="70d1a-285">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="70d1a-286">Com $select, você pode especificar um subconjunto ou um superconjunto das propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="70d1a-286">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="70d1a-287">Por exemplo, ao recuperar as mensagens do usuário conectado, você pode especificar que somente as propriedades **from** e **subject** sejam retornadas:</span><span class="sxs-lookup"><span data-stu-id="70d1a-287">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="70d1a-288">[Experimentar no Explorador do Graph][select-example]</span><span class="sxs-lookup"><span data-stu-id="70d1a-288">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="70d1a-289">**Importante:** Em geral, recomendamos que você use `$select` para limitar as propriedades retornadas por uma consulta àqueles exigidas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70d1a-289">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="70d1a-290">Isso se aplica particularmente a consultas com o potencial de retornar um conjunto de resultados amplo.</span><span class="sxs-lookup"><span data-stu-id="70d1a-290">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="70d1a-291">Limitar as propriedades retornadas em cada linha reduzirá a carga de rede e ajudará a melhorar o desempenho do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70d1a-291">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="70d1a-p129">No `v1.0`, alguns recursos do Azure AD que derivam de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), como [usuário](/graph/api/resources/user?view=graph-rest-1.0) e [grupo](/graph/api/resources/group?view=graph-rest-1.0), retornam um subconjunto limitado padrão de propriedades em leituras. Para esses recursos, você deve usar `$select` para retornar propriedades fora do conjunto padrão.</span><span class="sxs-lookup"><span data-stu-id="70d1a-p129">In `v1.0`, some Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="70d1a-294">parâmetro skip</span><span class="sxs-lookup"><span data-stu-id="70d1a-294">skip parameter</span></span>

<span data-ttu-id="70d1a-p130">Use o parâmetro de consulta `$skip` para definir o número de itens para ignorar no início de um conjunto. Por exemplo, a solicitação a seguir retorna eventos para o usuário classificadas por data de criação, começando com o evento 21 no conjunto:</span><span class="sxs-lookup"><span data-stu-id="70d1a-p130">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="70d1a-297">[Experimentar no Explorador do Graph][skip-example]</span><span class="sxs-lookup"><span data-stu-id="70d1a-297">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="70d1a-298">**Observação:** algumas APIs do Microsoft Graph, como Email e Calendário do Outlook (**message**, **event** e **calendar**), usam `$skip` para implementar a paginação.</span><span class="sxs-lookup"><span data-stu-id="70d1a-298">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="70d1a-299">Quando os resultados de uma consulta ocuparem várias páginas, essas APIs retornarão uma propriedade `@odata:nextLink` com uma URL que contém um parâmetro `$skip`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-299">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="70d1a-300">Você pode usar essa URL para retornar a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="70d1a-300">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="70d1a-301">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="70d1a-301">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="70d1a-302">parâmetro skipToken</span><span class="sxs-lookup"><span data-stu-id="70d1a-302">skipToken parameter</span></span>

<span data-ttu-id="70d1a-p132">Algumas solicitações retornam várias páginas de dados devido à paginação do lado do servidor ou devido ao uso do parâmetro [`$top`](#top-parameter) para limitar o tamanho da página da resposta. Muitas APIs do Microsoft Graph usam o parâmetro de consulta `skipToken` para fazer referência a páginas subsequentes do resultado. O parâmetro `$skiptoken` contém um token opaco que faz referência à próxima página de resultados e é retornado na URL fornecida na propriedade `@odata.nextLink` na resposta. Para saber mais, confira [paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="70d1a-p132">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="70d1a-307">parâmetro top</span><span class="sxs-lookup"><span data-stu-id="70d1a-307">top parameter</span></span>

<span data-ttu-id="70d1a-308">Use o parâmetro de consulta `$top` para especificar o tamanho de página do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="70d1a-308">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="70d1a-309">Se restarem mais itens no conjunto de resultados, o corpo da resposta conterá um parâmetro `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-309">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="70d1a-310">Esse parâmetro contém uma URL que você pode usar para obter a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="70d1a-310">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="70d1a-311">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="70d1a-311">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="70d1a-312">Por exemplo, a solicitação a seguir retorna as primeiras cinco mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="70d1a-312">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="70d1a-313">[Experimentar no Explorador do Graph][top-example]</span><span class="sxs-lookup"><span data-stu-id="70d1a-313">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="70d1a-314">Tratamento de erro para parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="70d1a-314">Error handling for query parameters</span></span>

<span data-ttu-id="70d1a-p134">Algumas solicitações retornarão uma mensagem de erro se não houver suporte para um parâmetro de consulta especificado. Por exemplo, você não pode usar `$expand` na relação `user/photo`.</span><span class="sxs-lookup"><span data-stu-id="70d1a-p134">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

```http
https://graph.microsoft.com/beta/me?$expand=photo
```

```json
{
    "error":{
        "code":"ExpandNotSupported",
        "message":"Expand is not allowed for property 'Photo' according to the entity schema.",
        "innerError":{
            "request-id":"1653fefd-bc31-484b-bb10-8dc33cb853ec",
            "date":"2017-07-31T20:55:01"
        }
    }
}
```

<span data-ttu-id="70d1a-317">No entanto, é importante observar que os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente.</span><span class="sxs-lookup"><span data-stu-id="70d1a-317">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="70d1a-318">Isso pode ser verdadeiro para parâmetros de consulta sem suporte, bem como para combinações de parâmetros de consulta sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70d1a-318">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="70d1a-319">Nesses casos, você deve examinar os dados retornados pela solicitação para determinar se os parâmetros de consulta que especificou tiveram o efeito desejado.</span><span class="sxs-lookup"><span data-stu-id="70d1a-319">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups?$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0

