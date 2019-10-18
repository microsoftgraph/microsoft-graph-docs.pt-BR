---
title: Usar parâmetros de consulta para personalizar respostas
description: O Microsoft Graph fornece parâmetros de consulta opcional que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta. Há suporte para os parâmetros de consulta a seguir.
author: piotrci
localization_priority: Priority
scenarios: getting-started
ms.custom: graphiamtop20
ms.openlocfilehash: 89809e080696163a4794fe554f73509e7f33b9d3
ms.sourcegitcommit: e87be8765d7f2bc90c6244d84c4719468bb3fd25
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2019
ms.locfileid: "37113811"
---
# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="8f5e0-104">Usar parâmetros de consulta para personalizar respostas</span><span class="sxs-lookup"><span data-stu-id="8f5e0-104">Use query parameters to customize responses</span></span>

<span data-ttu-id="8f5e0-105">O Microsoft Graph fornece suporte a parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-105">Microsoft Graph supports optional query parameters that you can use to specify and control the amount of data returned in a response.</span></span> <span data-ttu-id="8f5e0-106">O suporte para os parâmetros de consulta exatos variam de uma operação de API para outra e, dependendo da API, podem diferir entre os pontos de extremidade v1.0 e beta.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-106">The support for the exact query parameters varies from one API operation to another, and depending on the API, can differ between the v1.0 and beta endpoints.</span></span> 

> [!TIP] 
> <span data-ttu-id="8f5e0-107">No ponto de extremidade beta, o prefixo `$` é opcional.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-107">`$` On the v1.0 and beta endpoints, the  prefix is optional.</span></span> <span data-ttu-id="8f5e0-108">Por exemplo, em vez de `$filter`, você pode usar `filter`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-108">For example, instead of `$filter`, you can use `filter`.</span></span> <span data-ttu-id="8f5e0-109">No ponto de extremidade v1, o prefixo `$` é opcional apenas para um subconjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-109">On the v1 endpoint, the `$` prefix is optional for only a subset of APIs.</span></span> <span data-ttu-id="8f5e0-110">Para simplificar, inclua sempre `$` se estiver usando o ponto de extremidade v1.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-110">For simplicity, always include `$` if using the v1 endpoint.</span></span>

<span data-ttu-id="8f5e0-111">Os parâmetros de consulta podem ser opções de consulta de sistema OData ou outros parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-111">Query parameters can be OData system query options or other query parameters.</span></span> 

> [!VIDEO https://www.youtube-nocookie.com/embed/7BuFv3yETi4]

## <a name="odata-system-query-options"></a><span data-ttu-id="8f5e0-112">Opções de consulta de sistema OData</span><span class="sxs-lookup"><span data-stu-id="8f5e0-112">OData system query options</span></span>
<span data-ttu-id="8f5e0-113">Uma operação de API do Microsoft Graph pode oferecer suporte a uma ou mais das seguintes opções de consulta de sistema OData.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-113">A Microsoft Graph API operation might support one or more of the following OData system query options.</span></span> <span data-ttu-id="8f5e0-114">Essas opções de consulta são compatíveis com a [linguagem de consulta OData V4][odata-query].</span><span class="sxs-lookup"><span data-stu-id="8f5e0-114">These query options are compatible with the [OData V4 query language][odata-query].</span></span>

><span data-ttu-id="8f5e0-115">**Observação:** o OData 4.0 oferece suporte às opções de consulta do sistema apenas em operações GET.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-115">**Note:** OData 4.0 supports system query options in only GET operations.</span></span>

<span data-ttu-id="8f5e0-116">Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="8f5e0-116">Note: Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="8f5e0-117">Nome</span><span class="sxs-lookup"><span data-stu-id="8f5e0-117">Name</span></span>                     | <span data-ttu-id="8f5e0-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f5e0-118">Description</span></span> | <span data-ttu-id="8f5e0-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f5e0-119">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="8f5e0-120">$count</span><span class="sxs-lookup"><span data-stu-id="8f5e0-120">$count</span></span>](#count-parameter)         | <span data-ttu-id="8f5e0-121">Recupera a contagem total de recursos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-121">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="8f5e0-122">$expand</span><span class="sxs-lookup"><span data-stu-id="8f5e0-122">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="8f5e0-123">Recupera os recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-123">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="8f5e0-124">$filter</span><span class="sxs-lookup"><span data-stu-id="8f5e0-124">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="8f5e0-125">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-125">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="8f5e0-126">$format</span><span class="sxs-lookup"><span data-stu-id="8f5e0-126">$format</span></span>](#format-parameter)       | <span data-ttu-id="8f5e0-127">Retorna os resultados no formato de mídia especificado.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-127">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="8f5e0-128">$orderby</span><span class="sxs-lookup"><span data-stu-id="8f5e0-128">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="8f5e0-129">Ordena os resultados.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-129">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="8f5e0-130">$search</span><span class="sxs-lookup"><span data-stu-id="8f5e0-130">$search</span></span>](#search-parameter)       | <span data-ttu-id="8f5e0-p105">Retorna os resultados com base nos critérios de pesquisa. Atualmente, com suporte em conjuntos de **mensagens** e **pessoa**.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p105">Returns results based on search criteria. Currently supported on **messages** and **person** collections.</span></span>|[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="8f5e0-133">$select</span><span class="sxs-lookup"><span data-stu-id="8f5e0-133">$select</span></span>](#select-parameter)       | <span data-ttu-id="8f5e0-134">Filtra as propriedades (colunas).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-134">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="8f5e0-135">$skip</span><span class="sxs-lookup"><span data-stu-id="8f5e0-135">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="8f5e0-p106">Índices em um conjunto de resultados. Também usado por algumas APIs para implementar a paginação e pode ser usado com `$top` para paginar resultados manualmente.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p106">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="8f5e0-138">$top</span><span class="sxs-lookup"><span data-stu-id="8f5e0-138">$top</span></span>](#top-parameter)             | <span data-ttu-id="8f5e0-139">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-139">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a><span data-ttu-id="8f5e0-140">Outros parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="8f5e0-140">Other query parameters</span></span>

| <span data-ttu-id="8f5e0-141">Nome</span><span class="sxs-lookup"><span data-stu-id="8f5e0-141">Name</span></span>                     | <span data-ttu-id="8f5e0-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f5e0-142">Description</span></span> | <span data-ttu-id="8f5e0-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f5e0-143">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="8f5e0-144">$skipToken</span><span class="sxs-lookup"><span data-stu-id="8f5e0-144">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="8f5e0-p107">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas. (Algumas APIs usam `$skip` em vez disso.)</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p107">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="encoding-query-parameters"></a><span data-ttu-id="8f5e0-147">Codificação de parâmetros da consulta</span><span class="sxs-lookup"><span data-stu-id="8f5e0-147">Encoding query parameters</span></span>

<span data-ttu-id="8f5e0-148">Os valores dos parâmetros da consulta devem ser codificados por porcentagem.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-148">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="8f5e0-149">Muitas ferramentas, navegadores e clientes HTTP (como o [Explorador do Graph][graph-explorer]) ajudarão você com isso.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-149">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="8f5e0-150">Se uma consulta está falhando, uma causa possível é a falha na codificação adequada dos valores dos parâmetros da consulta.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-150">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="8f5e0-151">Uma URL descodificada é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-151">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="8f5e0-152">Uma URL codificada adequadamente é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-152">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

### <a name="escaping-single-quotes"></a><span data-ttu-id="8f5e0-153">Escape de aspas simples</span><span class="sxs-lookup"><span data-stu-id="8f5e0-153">Escaping single quotes</span></span>

<span data-ttu-id="8f5e0-154">Para pedidos que usem aspas simples, se os valores de qualquer parâmetro também contém aspas, elas devem ter escape duplo. Caso contrário, a solicitação falhará devido a sintaxe inválida.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-154">For requests that use single quotes, if any parameter values also contain single quotes, those must be double escaped; otherwise, the request will fail due to invalid syntax.</span></span> <span data-ttu-id="8f5e0-155">No exemplo, o valor de cadeia de caracteres `let''s meet for lunch?` tem o escape de aspas simples.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-155">In the example, the string value `let''s meet for lunch?` has the single quote escaped.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a><span data-ttu-id="8f5e0-156">parâmetro count</span><span class="sxs-lookup"><span data-stu-id="8f5e0-156">count parameter</span></span>

<span data-ttu-id="8f5e0-157">Use o parâmetro de consulta `$count` para incluir uma contagem do número total de itens em um conjunto, juntamente com a página de valores de dados retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-157">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="8f5e0-158">Por exemplo, a solicitação a seguir retornará o conjunto **contato** do usuário atual e o número de itens no conjunto **contato** na propriedade `@odata.count`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-158">For example, the following request will return both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="8f5e0-159">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="8f5e0-159">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="8f5e0-160">**Observação:** `$count` não tem suporte para conjuntos de recursos derivados de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), como conjuntos de [usuários](/graph/api/resources/user?view=graph-rest-1.0) ou [grupos](/graph/api/resources/group?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-160">**Note:** `$count` is not supported for collections of resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) like collections of [users](/graph/api/resources/user?view=graph-rest-1.0) or [groups](/graph/api/resources/group?view=graph-rest-1.0).</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="8f5e0-161">parâmetro expand</span><span class="sxs-lookup"><span data-stu-id="8f5e0-161">expand parameter</span></span>

<span data-ttu-id="8f5e0-162">Muitos recursos do Microsoft Graph expõem as propriedades declaradas do recurso, bem como as relações delas com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-162">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="8f5e0-163">Essas relações também são chamadas de propriedades de referência ou propriedades de navegação e podem fazer referência a um único recurso ou a um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-163">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="8f5e0-164">Por exemplo, as pastas de email, gerente e subordinados diretos de um usuário são todas expostas como relações.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-164">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="8f5e0-p111">Normalmente, você pode consultar as propriedades de um recurso ou uma de suas relações em uma única solicitação, mas não ambas. Você pode usar o parâmetro de cadeia de caracteres de consulta `$expand` para incluir o recurso expandido ou o conjunto referenciado por uma única relação (propriedade de navegação) nos resultados.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p111">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="8f5e0-167">O seguinte exemplo obtém informações de unidade raiz juntamente com os itens filho de nível superior em uma unidade:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-167">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="8f5e0-168">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="8f5e0-168">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="8f5e0-p112">Com alguns conjuntos de recursos, você também pode especificar as propriedades a serem retornadas nos recursos expandidos adicionando um parâmetro `$select`. O exemplo a seguir executa a mesma consulta que o exemplo anterior, mas usa uma instrução [`$select`](#select-parameter) para limitar as propriedades retornadas para os itens filho expandidos para as propriedades **id** e **name**.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p112">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="8f5e0-171">[Experimentar no Explorador do Graph][expand-example]</span><span class="sxs-lookup"><span data-stu-id="8f5e0-171">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="8f5e0-p113">**Observação:** nem todas as relações e recursos dão suporte ao parâmetro de consulta `$expand`. Por exemplo, você pode expandir as relações **directReports**, **manager** e **memberOf** em um usuário, mas não pode expandir suas relações **events**, **messages** ou **photo**. Nem todos os recursos ou relações dão suporte ao uso de `$select` em itens expandidos.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p113">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="8f5e0-175">Com recursos do Azure AD derivados de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), como [user](/graph/api/resources/user?view=graph-rest-1.0) e [group](/graph/api/resources/group?view=graph-rest-1.0), `$expand` só há suporte para `beta`, e normalmente são retornados no máximo 20 itens para a relação expandida.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-175">With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="8f5e0-176">parâmetro filter</span><span class="sxs-lookup"><span data-stu-id="8f5e0-176">filter parameter</span></span>

<span data-ttu-id="8f5e0-177">Use o parâmetro de consulta `$filter` para recuperar apenas um subconjunto de um conjunto.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-177">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="8f5e0-178">Por exemplo, para localizar os usuários cujo nome de exibição se inicia com a letra "J", use `startswith`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-178">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="8f5e0-179">[Experimentar no Explorador do Graph][filter-example]</span><span class="sxs-lookup"><span data-stu-id="8f5e0-179">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="8f5e0-180">O suporte para operadores `$filter` varia entre as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-180">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="8f5e0-181">Os seguintes operadores lógicos geralmente são suportados:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-181">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="8f5e0-182">igual a (`eq`)</span><span class="sxs-lookup"><span data-stu-id="8f5e0-182">equals (`eq`)</span></span>
- <span data-ttu-id="8f5e0-183">não é igual a (`ne`)</span><span class="sxs-lookup"><span data-stu-id="8f5e0-183">not equals (`ne`)</span></span>
- <span data-ttu-id="8f5e0-184">maior que (`gt`)</span><span class="sxs-lookup"><span data-stu-id="8f5e0-184">greater than (`gt`)</span></span>
- <span data-ttu-id="8f5e0-185">maior ou igual a (`ge`)</span><span class="sxs-lookup"><span data-stu-id="8f5e0-185">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="8f5e0-186">menor que (`lt`), menor ou igual a (`le`)</span><span class="sxs-lookup"><span data-stu-id="8f5e0-186">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="8f5e0-187">e (`and`)</span><span class="sxs-lookup"><span data-stu-id="8f5e0-187">and (`and`)</span></span>
- <span data-ttu-id="8f5e0-188">ou (`or`)</span><span class="sxs-lookup"><span data-stu-id="8f5e0-188">or (`or`)</span></span>
- <span data-ttu-id="8f5e0-189">não (`not`)</span><span class="sxs-lookup"><span data-stu-id="8f5e0-189">not (`not`)</span></span>
 
<span data-ttu-id="8f5e0-190">O operador de cadeia de caracteres `startswith` geralmente é suportado.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-190">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="8f5e0-191">O operador lambda `any` tem suporte em algumas APIs.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-191">The `any` lambda operator is supported for some APIs.</span></span> 

> <span data-ttu-id="8f5e0-192">**Observação:** é necessário [especificar propriedades em determinadas maneiras](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query) ao usar `$filter` e `$orderby` na mesma consulta para obter mensagens.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-192">**Note:** You must [specify properties in certain ways](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query) when using both `$filter` and `$orderby` in the same query to get messages.</span></span>

<span data-ttu-id="8f5e0-193">Para ver alguns exemplos de uso, confira a tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-193">For some  usage examples, see the following table.</span></span> <span data-ttu-id="8f5e0-194">Para obter mais detalhes sobre a sintaxe `$filter`, confira o [protocolo OData][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="8f5e0-194">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="8f5e0-195">A tabela a seguir mostra alguns exemplos que usam o parâmetro de consulta `$filter`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-195">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="8f5e0-196">**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="8f5e0-196">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="8f5e0-197">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f5e0-197">Description</span></span> | <span data-ttu-id="8f5e0-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f5e0-198">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="8f5e0-199">Pesquisar por usuários com o nome Clara entre várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-199">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| <span data-ttu-id="8f5e0-200">Obter todos os eventos do usuário conectado que começaram após 01/07/2017.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-200">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| <span data-ttu-id="8f5e0-201">Obter todos os emails de um endereço específico recebidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-201">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| <span data-ttu-id="8f5e0-202">Obter todos os emails recebidos pelo usuário conectado em abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-202">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| <span data-ttu-id="8f5e0-203">Obter todos os emails não lidos na caixa de entrada do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-203">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| <span data-ttu-id="8f5e0-204">Listar todos os grupos do Office 365 em uma organização.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-204">List all Office 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> <span data-ttu-id="8f5e0-p117">**Observação:** Os seguintes operadores `$filter` não têm suporte para recursos do Azure AD: `ne`, `gt`, `ge`, `lt`, `le` e `not`. O operador de cadeia de caracteres `contains` atualmente não tem suporte em nenhum recurso do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p117">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="8f5e0-207">parâmetro format</span><span class="sxs-lookup"><span data-stu-id="8f5e0-207">format parameter</span></span>

<span data-ttu-id="8f5e0-208">Use o parâmetro de consulta `$format` para especificar o formato de mídia dos itens retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-208">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="8f5e0-209">Por exemplo, a seguinte solicitação retorna os usuários na organização no formato json:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-209">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="8f5e0-210">[Experimentar no Explorador do Graph][format-example]</span><span class="sxs-lookup"><span data-stu-id="8f5e0-210">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="8f5e0-211">**Observação:** o parâmetro de consulta `$format` é compatível com vários formatos (por exemplo, atom, xml e json), mas os resultados podem não ser retornados em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-211">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="8f5e0-212">parâmetro orderby</span><span class="sxs-lookup"><span data-stu-id="8f5e0-212">orderby parameter</span></span>

<span data-ttu-id="8f5e0-213">Use o parâmetro de consulta `$orderby` para especificar a ordem de classificação dos itens retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-213">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="8f5e0-214">Por exemplo, a solicitação a seguir retorna os usuários da organização ordenados por seu nome de exibição:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-214">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="8f5e0-215">[Experimentar no Explorador do Graph][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="8f5e0-215">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="8f5e0-p118">Você também pode classificar por entidades de tipo complexo. A solicitação abaixo obtém mensagens e as classifica pelo campo **address** da propriedade **from**, que é do tipo complexo **emailAddress**:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p118">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="8f5e0-218">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="8f5e0-218">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="8f5e0-219">Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-219">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="8f5e0-220">Com algumas APIs, você pode ordenar os resultados em várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-220">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="8f5e0-221">Por exemplo, a solicitação a seguir ordena as mensagens na caixa de entrada do usuário primeiro pelo nome da pessoa que enviou, em ordem decrescente (Z – A) e, em seguida, por assunto, em ordem ascendente (padrão).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-221">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="8f5e0-222">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="8f5e0-222">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

> <span data-ttu-id="8f5e0-223">**Observação:** quando você especifica $filter, o servidor deduz uma ordem de classificação para os resultados.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-223">When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="8f5e0-224">Se você usar `$orderby` e `$filter` juntos para receber mensagens, como o servidor sempre infere uma ordem de classificação para os resultados de `$filter`, você deve [especificar propriedades de determinadas maneiras](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-224">If you use both `$orderby` and `$filter` to get messages, because the server always infers a sort order for the results of a `$filter`, you must [specify properties in certain ways](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query).</span></span>


<span data-ttu-id="8f5e0-225">O exemplo a seguir mostra uma consulta filtrada pelas propriedades **subject** e **priority** e classificadas pelas propriedades **subject**, **priority** e **receivedDateTime** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-225">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="8f5e0-226">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="8f5e0-226">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > <span data-ttu-id="8f5e0-227">**Observação:** Com os recursos do Azure AD derivados de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), como [user](/graph/api/resources/user?view=graph-rest-1.0) e [group](/graph/api/resources/group?view=graph-rest-1.0), você não pode combinar `$orderby` a expressões `$filter`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-227">**Note:** With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search-parameter"></a><span data-ttu-id="8f5e0-228">parâmetro search</span><span class="sxs-lookup"><span data-stu-id="8f5e0-228">search parameter</span></span>

<span data-ttu-id="8f5e0-229">Use o parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-229">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="8f5e0-p121">**Observação:** Atualmente, é possível pesquisar **somente** coleções de [mensagens](/graph/api/resources/message?view=graph-rest-1.0) e [pessoas](/graph/api/resources/person?view=graph-rest-1.0). Uma solicitação de `$search` retorna até 250 resultados. Não é possível usar [`$filter`](#filter-parameter) ou [`$orderby`](#orderby-parameter) em uma solicitação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p121">**Note:** You can currently search **only** [message](/graph/api/resources/message?view=graph-rest-1.0) and [person](/graph/api/resources/person?view=graph-rest-1.0) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter-parameter) or [`$orderby`](#orderby-parameter) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="8f5e0-233">Usando $search em conjuntos de mensagens</span><span class="sxs-lookup"><span data-stu-id="8f5e0-233">Using $search on message collections</span></span>

<span data-ttu-id="8f5e0-234">Você pode pesquisar mensagens com base em um valor nas propriedades de mensagens específicas.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-234">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="8f5e0-235">Os resultados da pesquisa são classificados pela data e hora em que a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-235">The results of the search are sorted by the date and time that the message was sent.</span></span>

<span data-ttu-id="8f5e0-236">Se você realizar uma pesquisa em mensagens e especificar apenas um valor sem as propriedades de mensagens específicas, a pesquisa será realizada nas propriedades de pesquisa padrão **from**, **subject** e **body**.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-236">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="8f5e0-237">O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-237">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="8f5e0-238">[Experimentar no Explorador do Graph][search-example]</span><span class="sxs-lookup"><span data-stu-id="8f5e0-238">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="8f5e0-239">Como alternativa, você pode pesquisar mensagens especificando os nomes de propriedade da mensagem na tabela a seguir, que são reconhecidos pela sintaxe da Linguagem de Consulta de Palavra-chave (KQL).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-239">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="8f5e0-240">Esses nomes de propriedades correspondem às propriedades definidas na entidade **mensagem** do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-240">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="8f5e0-241">O Outlook e outros aplicativos do Office 365, como o SharePoint, oferecem suporte à sintaxe KQL, proporcionando a conveniência de um domínio de descoberta comum para os repositórios de dados.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-241">Outlook and other Office 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="8f5e0-242">Propriedades de emails pesquisáveis</span><span class="sxs-lookup"><span data-stu-id="8f5e0-242">Searchable email property</span></span>                | <span data-ttu-id="8f5e0-243">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f5e0-243">Description</span></span> | <span data-ttu-id="8f5e0-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f5e0-244">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="8f5e0-245">**attachment**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-245">**attachment**</span></span>           | <span data-ttu-id="8f5e0-246">Os nomes dos arquivos anexados a uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-246">The names of files attached to an email message.</span></span>|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| <span data-ttu-id="8f5e0-247">**bcc**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-247">**bcc**</span></span>           | <span data-ttu-id="8f5e0-248">O campo **Cco** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-248">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| <span data-ttu-id="8f5e0-249">**body**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-249">**body**</span></span>           | <span data-ttu-id="8f5e0-250">O corpo de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-250">The body of an email message.</span></span>|[`me/messages?$search="body:excitement"`][search-body-example]
| <span data-ttu-id="8f5e0-251">**cc**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-251">**cc**</span></span>           | <span data-ttu-id="8f5e0-252">O campo **Cc** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-252">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| <span data-ttu-id="8f5e0-253">**from**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-253">**from**</span></span>           | <span data-ttu-id="8f5e0-254">O remetente de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-254">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| <span data-ttu-id="8f5e0-255">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-255">**hasAttachment**</span></span> | <span data-ttu-id="8f5e0-256">Verdadeiro se uma mensagem de email contiver um anexo que não seja um anexo embutido, caso contrário, falso.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-256">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> |[`me/messages?$search="hasAttachments=true"`][search-from-example]
| <span data-ttu-id="8f5e0-257">**importance**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-257">**importance**</span></span>           | <span data-ttu-id="8f5e0-258">A prioridade de uma mensagem de email, que um remetente pode especificar ao enviar uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-258">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="8f5e0-259">Os valores possíveis são `low`, `medium` ou `high`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-259">The possible values are `low`, `medium`, or `high`.</span></span>|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| <span data-ttu-id="8f5e0-260">**kind**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-260">**kind**</span></span>           | <span data-ttu-id="8f5e0-261">O tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-261">The type of message.</span></span> <span data-ttu-id="8f5e0-262">Os valores possíveis são `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` ou `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-262">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| <span data-ttu-id="8f5e0-263">**participants**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-263">**participants**</span></span>           | <span data-ttu-id="8f5e0-264">Os campos **de**, **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-264">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="participants:danas"`][search-part-example]
| <span data-ttu-id="8f5e0-265">**received**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-265">**received**</span></span>           | <span data-ttu-id="8f5e0-266">A data em que uma mensagem de email foi recebida pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-266">The date that an email message was received by a recipient.</span></span>|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| <span data-ttu-id="8f5e0-267">**recipients**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-267">**recipients**</span></span>           | <span data-ttu-id="8f5e0-268">Os campos **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-268">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| <span data-ttu-id="8f5e0-269">**sent**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-269">**sent**</span></span>           | <span data-ttu-id="8f5e0-270">A data em que uma mensagem de email foi enviada pelo remetente.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-270">The date that an email message was sent by the sender.</span></span>|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| <span data-ttu-id="8f5e0-271">**size**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-271">**size**</span></span>           | <span data-ttu-id="8f5e0-272">O tamanho de um item em bytes.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-272">The size of an item in bytes.</span></span>|[`me/messages?$search="size:1..500000"`][search-size-example]
| <span data-ttu-id="8f5e0-273">**subject**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-273">**subject**</span></span>           | <span data-ttu-id="8f5e0-274">O texto na linha de assunto de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-274">The text in the subject line of an email message.</span></span> <span data-ttu-id="8f5e0-275">.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-275"></span></span>|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| <span data-ttu-id="8f5e0-276">**to**</span><span class="sxs-lookup"><span data-stu-id="8f5e0-276">**to**</span></span>           | <span data-ttu-id="8f5e0-277">O campo **para** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-277">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


<span data-ttu-id="8f5e0-278">Para saber mais sobre as propriedades de email pesquisáveis, KQL como a sintaxe, operadores com suporte e dicas de pesquisa, confira os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-278">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="8f5e0-279">[Propriedades pesquisáveis no Exchange](https://docs.microsoft.com/pt-BR/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-279">[Searchable properties in Exchange](https://docs.microsoft.com/pt-BR/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- [<span data-ttu-id="8f5e0-280">Referência de sintaxe da Linguagem de Consulta de Palavra-chave (KQL)</span><span class="sxs-lookup"><span data-stu-id="8f5e0-280">Keyword Query Language (KQL) syntax reference</span></span>](https://docs.microsoft.com/pt-BR/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- <span data-ttu-id="8f5e0-281">[Propriedades da mensagem e operadores de pesquisa para a Descoberta eletrônica In-loco no Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span><span class="sxs-lookup"><span data-stu-id="8f5e0-281">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="8f5e0-282">Usando $search em conjuntos de pessoas</span><span class="sxs-lookup"><span data-stu-id="8f5e0-282">Using $search on person collections</span></span>

<span data-ttu-id="8f5e0-p127">Você pode usar a API de Pessoas do Microsoft Graph para recuperar as pessoas mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. A API de Pessoas dá suporte ao parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p127">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="8f5e0-286">As pesquisas de pessoas ocorrem nas propriedades **displayName** e **emailAddress** do recurso [person](/graph/api/resources/person?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-286">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](/graph/api/resources/person?view=graph-rest-1.0) resource.</span></span>

<span data-ttu-id="8f5e0-287">A seguinte solicitação faz uma pesquisa por uma pessoa chamada "Clara Barbosa" nas propriedades **displayName** e **emailAddress** em todos os indivíduos no conjunto de **Pessoas** do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-287">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="8f5e0-288">Como uma pessoa denominada "Clara Barbosa" é relevante para o usuário conectado, as informações para "Clara Barbosa" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-288">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="8f5e0-289">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-289">The following example shows the response.</span></span> 

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

<span data-ttu-id="8f5e0-290">Saiba mais sobre a API de Pessoas em [Obter informações sobre pessoas relevantes](./people-example.md#search-people).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-290">To learn more about the People API, see [Get information about relevant people](./people-example.md#search-people).</span></span>  

## <a name="select-parameter"></a><span data-ttu-id="8f5e0-291">parâmetro select</span><span class="sxs-lookup"><span data-stu-id="8f5e0-291">select parameter</span></span>

<span data-ttu-id="8f5e0-292">Use o parâmetro de consulta `$select` para retornar um conjunto de propriedades diferente do padrão definido para um recurso individual ou um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-292">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="8f5e0-293">Com $select, você pode especificar um subconjunto ou um superconjunto das propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-293">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="8f5e0-294">Por exemplo, ao recuperar as mensagens do usuário conectado, você pode especificar que somente as propriedades **from** e **subject** sejam retornadas:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-294">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="8f5e0-295">[Experimentar no Explorador do Graph][select-example]</span><span class="sxs-lookup"><span data-stu-id="8f5e0-295">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="8f5e0-296">**Importante:** Em geral, recomendamos que você use `$select` para limitar as propriedades retornadas por uma consulta àqueles exigidas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-296">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="8f5e0-297">Isso se aplica particularmente a consultas com o potencial de retornar um conjunto de resultados amplo.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-297">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="8f5e0-298">Limitar as propriedades retornadas em cada linha reduzirá a carga de rede e ajudará a melhorar o desempenho do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-298">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="8f5e0-p131">No `v1.0`, alguns recursos do Azure AD que derivam de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), como [usuário](/graph/api/resources/user?view=graph-rest-1.0) e [grupo](/graph/api/resources/group?view=graph-rest-1.0), retornam um subconjunto limitado padrão de propriedades em leituras. Para esses recursos, você deve usar `$select` para retornar propriedades fora do conjunto padrão.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p131">In `v1.0`, some Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="8f5e0-301">parâmetro skip</span><span class="sxs-lookup"><span data-stu-id="8f5e0-301">skip parameter</span></span>

<span data-ttu-id="8f5e0-p132">Use o parâmetro de consulta `$skip` para definir o número de itens para ignorar no início de um conjunto. Por exemplo, a solicitação a seguir retorna eventos para o usuário classificadas por data de criação, começando com o evento 21 no conjunto:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p132">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="8f5e0-304">[Experimentar no Explorador do Graph][skip-example]</span><span class="sxs-lookup"><span data-stu-id="8f5e0-304">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="8f5e0-305">**Observação:** algumas APIs do Microsoft Graph, como Email e Calendário do Outlook (**message**, **event** e **calendar**), usam `$skip` para implementar a paginação.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-305">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="8f5e0-306">Quando os resultados de uma consulta ocuparem várias páginas, essas APIs retornarão uma propriedade `@odata:nextLink` com uma URL que contém um parâmetro `$skip`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-306">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="8f5e0-307">Você pode usar essa URL para retornar a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-307">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="8f5e0-308">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-308">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="8f5e0-309">parâmetro skipToken</span><span class="sxs-lookup"><span data-stu-id="8f5e0-309">skipToken parameter</span></span>

<span data-ttu-id="8f5e0-p134">Algumas solicitações retornam várias páginas de dados devido à paginação do lado do servidor ou devido ao uso do parâmetro [`$top`](#top-parameter) para limitar o tamanho da página da resposta. Muitas APIs do Microsoft Graph usam o parâmetro de consulta `skipToken` para fazer referência a páginas subsequentes do resultado. O parâmetro `$skiptoken` contém um token opaco que faz referência à próxima página de resultados e é retornado na URL fornecida na propriedade `@odata.nextLink` na resposta. Para saber mais, confira [paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p134">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="8f5e0-314">parâmetro top</span><span class="sxs-lookup"><span data-stu-id="8f5e0-314">top parameter</span></span>

<span data-ttu-id="8f5e0-315">Use o parâmetro de consulta `$top` para especificar o tamanho de página do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-315">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="8f5e0-316">Se restarem mais itens no conjunto de resultados, o corpo da resposta conterá um parâmetro `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-316">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="8f5e0-317">Esse parâmetro contém uma URL que você pode usar para obter a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-317">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="8f5e0-318">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="8f5e0-318">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="8f5e0-319">Por exemplo, a solicitação a seguir retorna as primeiras cinco mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="8f5e0-319">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="8f5e0-320">[Experimentar no Explorador do Graph][top-example]</span><span class="sxs-lookup"><span data-stu-id="8f5e0-320">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="8f5e0-321">Tratamento de erro para parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="8f5e0-321">Error handling for query parameters</span></span>

<span data-ttu-id="8f5e0-p136">Algumas solicitações retornarão uma mensagem de erro se não houver suporte para um parâmetro de consulta especificado. Por exemplo, você não pode usar `$expand` na relação `user/photo`.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-p136">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="8f5e0-324">No entanto, é importante observar que os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-324">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="8f5e0-325">Isso pode ser verdadeiro para parâmetros de consulta sem suporte, bem como para combinações de parâmetros de consulta sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-325">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="8f5e0-326">Nesses casos, você deve examinar os dados retornados pela solicitação para determinar se os parâmetros de consulta que especificou tiveram o efeito desejado.</span><span class="sxs-lookup"><span data-stu-id="8f5e0-326">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

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

