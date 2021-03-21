---
title: Usar parâmetros de consulta para personalizar respostas
description: O Microsoft Graph fornece parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta.
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 51bf43360c3580011ab39e2c385b4c23d3bfc5a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962410"
---
# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="20a54-103">Usar parâmetros de consulta para personalizar respostas</span><span class="sxs-lookup"><span data-stu-id="20a54-103">Use query parameters to customize responses</span></span>

<span data-ttu-id="20a54-104">O Microsoft Graph fornece suporte a parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="20a54-104">Microsoft Graph supports optional query parameters that you can use to specify and control the amount of data returned in a response.</span></span> <span data-ttu-id="20a54-105">O suporte para os parâmetros de consulta exatos variam de uma operação de API para outra e, dependendo da API, podem diferir entre os pontos de extremidade v1.0 e beta.</span><span class="sxs-lookup"><span data-stu-id="20a54-105">The support for the exact query parameters varies from one API operation to another, and depending on the API, can differ between the v1.0 and beta endpoints.</span></span> 

> [!TIP] 
> <span data-ttu-id="20a54-106">No ponto de extremidade beta, o prefixo `$` é opcional.</span><span class="sxs-lookup"><span data-stu-id="20a54-106">On the beta endpoint, the `$` prefix is optional.</span></span> <span data-ttu-id="20a54-107">Por exemplo, em vez de `$filter`, você pode usar `filter`.</span><span class="sxs-lookup"><span data-stu-id="20a54-107">For example, instead of `$filter`, you can use `filter`.</span></span> <span data-ttu-id="20a54-108">No ponto de extremidade v1, o prefixo `$` é opcional apenas para um subconjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="20a54-108">On the v1 endpoint, the `$` prefix is optional for only a subset of APIs.</span></span> <span data-ttu-id="20a54-109">Para simplificar, inclua sempre `$` se estiver usando o ponto de extremidade v1.</span><span class="sxs-lookup"><span data-stu-id="20a54-109">For simplicity, always include `$` if using the v1 endpoint.</span></span>

<span data-ttu-id="20a54-110">Os parâmetros de consulta podem ser opções de consulta de sistema OData ou outros parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="20a54-110">Query parameters can be OData system query options or other query parameters.</span></span> 

> [!VIDEO https://www.youtube-nocookie.com/embed/7BuFv3yETi4]

## <a name="odata-system-query-options"></a><span data-ttu-id="20a54-111">Opções de consulta de sistema OData</span><span class="sxs-lookup"><span data-stu-id="20a54-111">OData system query options</span></span>
<span data-ttu-id="20a54-112">Uma operação de API do Microsoft Graph pode oferecer suporte a uma ou mais das seguintes opções de consulta de sistema OData.</span><span class="sxs-lookup"><span data-stu-id="20a54-112">A Microsoft Graph API operation might support one or more of the following OData system query options.</span></span> <span data-ttu-id="20a54-113">Essas opções de consulta são compatíveis com a [linguagem de consulta OData V4][odata-query].</span><span class="sxs-lookup"><span data-stu-id="20a54-113">These query options are compatible with the [OData V4 query language][odata-query].</span></span>

><span data-ttu-id="20a54-114">**Observação:** o OData 4.0 oferece suporte às opções de consulta do sistema apenas em operações GET.</span><span class="sxs-lookup"><span data-stu-id="20a54-114">**Note:** OData 4.0 supports system query options in only GET operations.</span></span>

<span data-ttu-id="20a54-115">Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="20a54-115">Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="20a54-116">Nome</span><span class="sxs-lookup"><span data-stu-id="20a54-116">Name</span></span>                     | <span data-ttu-id="20a54-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="20a54-117">Description</span></span> | <span data-ttu-id="20a54-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20a54-118">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="20a54-119">$count</span><span class="sxs-lookup"><span data-stu-id="20a54-119">$count</span></span>](#count-parameter)         | <span data-ttu-id="20a54-120">Recupera a contagem total de recursos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="20a54-120">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="20a54-121">$expand</span><span class="sxs-lookup"><span data-stu-id="20a54-121">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="20a54-122">Recupera os recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="20a54-122">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="20a54-123">$filter</span><span class="sxs-lookup"><span data-stu-id="20a54-123">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="20a54-124">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="20a54-124">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="20a54-125">$format</span><span class="sxs-lookup"><span data-stu-id="20a54-125">$format</span></span>](#format-parameter)       | <span data-ttu-id="20a54-126">Retorna os resultados no formato de mídia especificado.</span><span class="sxs-lookup"><span data-stu-id="20a54-126">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="20a54-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="20a54-127">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="20a54-128">Ordena os resultados.</span><span class="sxs-lookup"><span data-stu-id="20a54-128">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="20a54-129">$search</span><span class="sxs-lookup"><span data-stu-id="20a54-129">$search</span></span>](#search-parameter)       | <span data-ttu-id="20a54-130">Retorna os resultados com base nos critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="20a54-130">Returns results based on search criteria.</span></span> |[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="20a54-131">$select</span><span class="sxs-lookup"><span data-stu-id="20a54-131">$select</span></span>](#select-parameter)       | <span data-ttu-id="20a54-132">Filtra as propriedades (colunas).</span><span class="sxs-lookup"><span data-stu-id="20a54-132">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="20a54-133">$skip</span><span class="sxs-lookup"><span data-stu-id="20a54-133">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="20a54-p104">Índices em um conjunto de resultados. Também usado por algumas APIs para implementar a paginação e pode ser usado com `$top` para paginar resultados manualmente.</span><span class="sxs-lookup"><span data-stu-id="20a54-p104">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="20a54-136">$top</span><span class="sxs-lookup"><span data-stu-id="20a54-136">$top</span></span>](#top-parameter)             | <span data-ttu-id="20a54-137">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="20a54-137">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a><span data-ttu-id="20a54-138">Outros parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="20a54-138">Other query parameters</span></span>

| <span data-ttu-id="20a54-139">Nome</span><span class="sxs-lookup"><span data-stu-id="20a54-139">Name</span></span>                     | <span data-ttu-id="20a54-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="20a54-140">Description</span></span> | <span data-ttu-id="20a54-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20a54-141">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="20a54-142">$skipToken</span><span class="sxs-lookup"><span data-stu-id="20a54-142">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="20a54-p105">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas. (Algumas APIs usam `$skip` em vez disso.)</span><span class="sxs-lookup"><span data-stu-id="20a54-p105">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a><span data-ttu-id="20a54-145">Outros recursos de URL OData</span><span class="sxs-lookup"><span data-stu-id="20a54-145">Other OData URL capabilities</span></span>

<span data-ttu-id="20a54-146">Os seguintes recursos OData 4.0 são segmentos de URL, não parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="20a54-146">The following OData 4.0 capabilities are URL segments, not query parameters.</span></span>

| <span data-ttu-id="20a54-147">Nome</span><span class="sxs-lookup"><span data-stu-id="20a54-147">Name</span></span>                     | <span data-ttu-id="20a54-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="20a54-148">Description</span></span> | <span data-ttu-id="20a54-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20a54-149">Example</span></span> 
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="20a54-150">$ref</span><span class="sxs-lookup"><span data-stu-id="20a54-150">$ref</span></span>](/graph/api/group-post-members) | <span data-ttu-id="20a54-151">Atualiza a associação de entidades a uma coleção.</span><span class="sxs-lookup"><span data-stu-id="20a54-151">Updates entities membership to a collection.</span></span> | `POST /groups/{id}/members/$ref` |
| [<span data-ttu-id="20a54-152">$value</span><span class="sxs-lookup"><span data-stu-id="20a54-152">$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="20a54-153">Recupera ou atualiza o valor binário de um item.</span><span class="sxs-lookup"><span data-stu-id="20a54-153">Retrieves or updates the binary value of an item.</span></span> | `GET /me/photo/$value` |

## <a name="encoding-query-parameters"></a><span data-ttu-id="20a54-154">Codificação de parâmetros da consulta</span><span class="sxs-lookup"><span data-stu-id="20a54-154">Encoding query parameters</span></span>

<span data-ttu-id="20a54-155">Os valores dos parâmetros da consulta devem ser codificados por porcentagem.</span><span class="sxs-lookup"><span data-stu-id="20a54-155">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="20a54-156">Muitas ferramentas, navegadores e clientes HTTP (como o [Explorador do Graph][graph-explorer]) ajudarão você com isso.</span><span class="sxs-lookup"><span data-stu-id="20a54-156">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="20a54-157">Se uma consulta está falhando, uma causa possível é a falha na codificação adequada dos valores dos parâmetros da consulta.</span><span class="sxs-lookup"><span data-stu-id="20a54-157">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="20a54-158">Uma URL descodificada é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="20a54-158">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="20a54-159">Uma URL codificada adequadamente é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="20a54-159">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

### <a name="escaping-single-quotes"></a><span data-ttu-id="20a54-160">Escape de aspas simples</span><span class="sxs-lookup"><span data-stu-id="20a54-160">Escaping single quotes</span></span>

<span data-ttu-id="20a54-161">Para pedidos que usem aspas simples, se os valores de qualquer parâmetro também contém aspas, elas devem ter escape duplo. Caso contrário, a solicitação falhará devido a sintaxe inválida.</span><span class="sxs-lookup"><span data-stu-id="20a54-161">For requests that use single quotes, if any parameter values also contain single quotes, those must be double escaped; otherwise, the request will fail due to invalid syntax.</span></span> <span data-ttu-id="20a54-162">No exemplo, o valor de cadeia de caracteres `let''s meet for lunch?` tem o escape de aspas simples.</span><span class="sxs-lookup"><span data-stu-id="20a54-162">In the example, the string value `let''s meet for lunch?` has the single quote escaped.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a><span data-ttu-id="20a54-163">parâmetro count</span><span class="sxs-lookup"><span data-stu-id="20a54-163">count parameter</span></span>

<span data-ttu-id="20a54-164">Use o parâmetro de consulta `$count` para incluir uma contagem do número total de itens em um conjunto, juntamente com a página de valores de dados retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="20a54-164">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="20a54-165">Por exemplo, a solicitação a seguir retornará tanto o conjunto **contato** do usuário atual quanto o número de itens no conjunto **contato** na propriedade `@odata.count`.</span><span class="sxs-lookup"><span data-stu-id="20a54-165">For example, the following request returns both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="20a54-166">Experimente o Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="20a54-166">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


<span data-ttu-id="20a54-167">O parâmetro de consulta `$count` é compatível com esses conjuntos de recursos e suas relações, derivadas do [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true):</span><span class="sxs-lookup"><span data-stu-id="20a54-167">The `$count` query parameter is supported for these collections of resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true):</span></span>
- [<span data-ttu-id="20a54-168">application</span><span class="sxs-lookup"><span data-stu-id="20a54-168">application</span></span>](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="20a54-169">orgContact</span><span class="sxs-lookup"><span data-stu-id="20a54-169">orgContact</span></span>](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="20a54-170">device</span><span class="sxs-lookup"><span data-stu-id="20a54-170">device</span></span>](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="20a54-171">group</span><span class="sxs-lookup"><span data-stu-id="20a54-171">group</span></span>](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="20a54-172">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="20a54-172">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)
- <span data-ttu-id="20a54-173">[users](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="20a54-173">[users](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true).</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="20a54-174">parâmetro expand</span><span class="sxs-lookup"><span data-stu-id="20a54-174">expand parameter</span></span>

<span data-ttu-id="20a54-175">Muitos recursos do Microsoft Graph expõem as propriedades declaradas do recurso, bem como as relações delas com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="20a54-175">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="20a54-176">Essas relações também são chamadas de propriedades de referência ou propriedades de navegação e podem fazer referência a um único recurso ou a um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="20a54-176">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="20a54-177">Por exemplo, as pastas de email, gerente e subordinados diretos de um usuário são todas expostas como relações.</span><span class="sxs-lookup"><span data-stu-id="20a54-177">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="20a54-p109">Normalmente, você pode consultar as propriedades de um recurso ou uma de suas relações em uma única solicitação, mas não ambas. Você pode usar o parâmetro de cadeia de caracteres de consulta `$expand` para incluir o recurso expandido ou o conjunto referenciado por uma única relação (propriedade de navegação) nos resultados.</span><span class="sxs-lookup"><span data-stu-id="20a54-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="20a54-180">O seguinte exemplo obtém informações de unidade raiz juntamente com os itens filho de nível superior em uma unidade:</span><span class="sxs-lookup"><span data-stu-id="20a54-180">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="20a54-181">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="20a54-181">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="20a54-p110">Com alguns conjuntos de recursos, você também pode especificar as propriedades a serem retornadas nos recursos expandidos adicionando um parâmetro `$select`. O exemplo a seguir executa a mesma consulta que o exemplo anterior, mas usa uma instrução [`$select`](#select-parameter) para limitar as propriedades retornadas para os itens filho expandidos para as propriedades **id** e **name**.</span><span class="sxs-lookup"><span data-stu-id="20a54-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="20a54-184">[Experimentar no Explorador do Graph][expand-example]</span><span class="sxs-lookup"><span data-stu-id="20a54-184">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="20a54-p111">**Observação:** nem todas as relações e recursos dão suporte ao parâmetro de consulta `$expand`. Por exemplo, você pode expandir as relações **directReports**, **manager** e **memberOf** em um usuário, mas não pode expandir suas relações **events**, **messages** ou **photo**. Nem todos os recursos ou relações dão suporte ao uso de `$select` em itens expandidos.</span><span class="sxs-lookup"><span data-stu-id="20a54-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="20a54-188">Com recursos do Azure AD derivados de [directoryObject](/graph/api/resources/directoryobject), como [user](/graph/api/resources/user) e [group](/graph/api/resources/group), `$expand` só há suporte para `beta`, e normalmente são retornados no máximo 20 itens para a relação expandida.</span><span class="sxs-lookup"><span data-stu-id="20a54-188">With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject), like [user](/graph/api/resources/user) and [group](/graph/api/resources/group), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="20a54-189">parâmetro filter</span><span class="sxs-lookup"><span data-stu-id="20a54-189">filter parameter</span></span>

<span data-ttu-id="20a54-190">Use o parâmetro de consulta `$filter` para recuperar apenas um subconjunto de um conjunto.</span><span class="sxs-lookup"><span data-stu-id="20a54-190">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> <span data-ttu-id="20a54-191">O parâmetro de consulta `$filter` também pode ser usado para recuperar relações como members, memberOf, transitiveMembers e transitiveMemberOf.</span><span class="sxs-lookup"><span data-stu-id="20a54-191">The `$filter` query parameter can also be used to retrieve relationships like members, memberOf, transitiveMembers, and transitiveMemberOf.</span></span> <span data-ttu-id="20a54-192">Por exemplo, obter todos os grupos de segurança dos quais sou membro.</span><span class="sxs-lookup"><span data-stu-id="20a54-192">For example, get all the security groups I'm a member of.</span></span>

<span data-ttu-id="20a54-193">O exemplo a seguir pode ser usado para encontrar usuários cujo nome de exibição começa com a letra “J’: use `startsWith`.</span><span class="sxs-lookup"><span data-stu-id="20a54-193">The following example can be used to find users whose display name starts with the letter 'J', use `startsWith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startsWith(displayName,'J')
```

<span data-ttu-id="20a54-194">[Experimentar no Explorador do Graph][filter-example]</span><span class="sxs-lookup"><span data-stu-id="20a54-194">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="20a54-195">O suporte para operadores `$filter` varia entre as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="20a54-195">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="20a54-196">Os seguintes operadores lógicos geralmente são suportados:</span><span class="sxs-lookup"><span data-stu-id="20a54-196">The following logical operators are generally supported:</span></span>

- <span data-ttu-id="20a54-197">é igual a `eq` / não é igual a `ne`</span><span class="sxs-lookup"><span data-stu-id="20a54-197">equals `eq` / not equals `ne`</span></span>
- <span data-ttu-id="20a54-198">menor que `lt` / maior que `gt`</span><span class="sxs-lookup"><span data-stu-id="20a54-198">less than `lt` / greater than `gt`</span></span>
- <span data-ttu-id="20a54-199">menor que ou igual a `le` / maior que ou igual a `ge`</span><span class="sxs-lookup"><span data-stu-id="20a54-199">less than or equal to `le` / greater than or equal to `ge`</span></span>
- <span data-ttu-id="20a54-200">e `and` / ou `or`</span><span class="sxs-lookup"><span data-stu-id="20a54-200">and `and` / or `or`</span></span>
- <span data-ttu-id="20a54-201">em `in`</span><span class="sxs-lookup"><span data-stu-id="20a54-201">in `in`</span></span>
- <span data-ttu-id="20a54-202">Negação `not`</span><span class="sxs-lookup"><span data-stu-id="20a54-202">Negation `not`</span></span>
- <span data-ttu-id="20a54-203">operador lambda qualquer `any`</span><span class="sxs-lookup"><span data-stu-id="20a54-203">lambda operator any `any`</span></span>
- <span data-ttu-id="20a54-204">operador lambda todos `all`</span><span class="sxs-lookup"><span data-stu-id="20a54-204">lambda operator all `all`</span></span>
- <span data-ttu-id="20a54-205">Começa com`startsWith`</span><span class="sxs-lookup"><span data-stu-id="20a54-205">Starts with `startsWith`</span></span>
- <span data-ttu-id="20a54-206">Termina com`endsWith`</span><span class="sxs-lookup"><span data-stu-id="20a54-206">Ends with `endsWith`</span></span>

> <span data-ttu-id="20a54-207">**Observação:** o suporte a esses operadores varia de acordo com a entidade.</span><span class="sxs-lookup"><span data-stu-id="20a54-207">**Note:** Support for these operators varies by entity.</span></span> <span data-ttu-id="20a54-208">Confira a documentação específica da entidade para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="20a54-208">See the specific entity documentation for details.</span></span> 
>
> <span data-ttu-id="20a54-209">O operador da cadeia de caracteres `contains` atualmente não tem suporte em nenhum recurso do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="20a54-209">The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

<span data-ttu-id="20a54-210">Para ver alguns exemplos de uso, consulte a tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="20a54-210">For some usage examples, see the following table.</span></span> <span data-ttu-id="20a54-211">Para obter mais detalhes sobre a sintaxe `$filter`, confira o [protocolo OData][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="20a54-211">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  
<span data-ttu-id="20a54-212">A tabela a seguir mostra alguns exemplos que usam o parâmetro de consulta `$filter`.</span><span class="sxs-lookup"><span data-stu-id="20a54-212">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="20a54-213">**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="20a54-213">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="20a54-214">Descrição</span><span class="sxs-lookup"><span data-stu-id="20a54-214">Description</span></span> | <span data-ttu-id="20a54-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20a54-215">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="20a54-216">Pesquisar por usuários com o nome Clara entre várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="20a54-216">Get all users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| <span data-ttu-id="20a54-217">Obtenha todos os usuários com o domínio de email igual a 'hotmail.com'</span><span class="sxs-lookup"><span data-stu-id="20a54-217">Get all users with mail domain equal to 'hotmail.com'</span></span> | [`https://graph.microsoft.com/v1.0/users?$count=true&$filter=endsWith(mail,'@hotmail.com')`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) |
| <span data-ttu-id="20a54-218">Obter todos os eventos do usuário conectado que começaram após 01/07/2017.</span><span class="sxs-lookup"><span data-stu-id="20a54-218">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| <span data-ttu-id="20a54-219">Obter todos os emails de um endereço específico recebidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="20a54-219">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| <span data-ttu-id="20a54-220">Obter todos os emails recebidos pelo usuário conectado em abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="20a54-220">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| <span data-ttu-id="20a54-221">Obter todos os emails não lidos na caixa de entrada do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="20a54-221">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| <span data-ttu-id="20a54-222">Listar todos os grupos do Microsoft 365 em uma organização.</span><span class="sxs-lookup"><span data-stu-id="20a54-222">List all Microsoft 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |
| <span data-ttu-id="20a54-223">Use a conversão OData para obter uma participação transitória em grupos com um nome de exibição que comece com “a”, incluindo o número de objetos retornados.</span><span class="sxs-lookup"><span data-stu-id="20a54-223">Use OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects.</span></span> | [`https://graph.microsoft.com/beta/me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`](https://developer.microsoft.com/graph/graph-explorer?request=me/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName,'a')&method=GET&version=v1.0) |

## <a name="format-parameter"></a><span data-ttu-id="20a54-224">parâmetro format</span><span class="sxs-lookup"><span data-stu-id="20a54-224">format parameter</span></span>

<span data-ttu-id="20a54-225">Use o parâmetro de consulta `$format` para especificar o formato de mídia dos itens retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="20a54-225">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="20a54-226">Por exemplo, a seguinte solicitação retorna os usuários na organização no formato json:</span><span class="sxs-lookup"><span data-stu-id="20a54-226">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="20a54-227">[Experimentar no Explorador do Graph][format-example]</span><span class="sxs-lookup"><span data-stu-id="20a54-227">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="20a54-228">**Observação:** o parâmetro de consulta `$format` é compatível com vários formatos (por exemplo, atom, xml e json), mas os resultados podem não ser retornados em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="20a54-228">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="20a54-229">parâmetro orderby</span><span class="sxs-lookup"><span data-stu-id="20a54-229">orderby parameter</span></span>

<span data-ttu-id="20a54-230">Use o parâmetro de consulta `$orderby` para especificar a ordem de classificação dos itens retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="20a54-230">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="20a54-231">Por exemplo, a solicitação a seguir retorna os usuários da organização ordenados por seu nome de exibição:</span><span class="sxs-lookup"><span data-stu-id="20a54-231">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="20a54-232">[Experimentar no Explorador do Graph][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="20a54-232">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="20a54-p116">Você também pode classificar por entidades de tipo complexo. A solicitação abaixo obtém mensagens e as classifica pelo campo **address** da propriedade **from**, que é do tipo complexo **emailAddress**:</span><span class="sxs-lookup"><span data-stu-id="20a54-p116">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="20a54-235">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="20a54-235">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="20a54-236">Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="20a54-236">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="20a54-237">Com algumas APIs, você pode ordenar os resultados em várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="20a54-237">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="20a54-238">Por exemplo, a solicitação a seguir ordena as mensagens na caixa de entrada do usuário primeiro pelo nome da pessoa que enviou, em ordem decrescente (Z – A) e, em seguida, por assunto, em ordem ascendente (padrão).</span><span class="sxs-lookup"><span data-stu-id="20a54-238">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="20a54-239">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="20a54-239">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

> <span data-ttu-id="20a54-240">**Observação:** quando você especifica $filter, o servidor deduz uma ordem de classificação para os resultados.</span><span class="sxs-lookup"><span data-stu-id="20a54-240">**Note:** When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="20a54-241">Se você usar `$orderby` e `$filter` juntos para receber mensagens, como o servidor sempre infere uma ordem de classificação para os resultados de `$filter`, você deve [especificar propriedades de determinadas maneiras](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query).</span><span class="sxs-lookup"><span data-stu-id="20a54-241">If you use both `$orderby` and `$filter` to get messages, because the server always infers a sort order for the results of a `$filter`, you must [specify properties in certain ways](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query).</span></span>


<span data-ttu-id="20a54-242">O exemplo a seguir mostra uma consulta filtrada pelas propriedades **subject** e **priority** e classificadas pelas propriedades **subject**, **priority** e **receivedDateTime** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="20a54-242">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="20a54-243">Experimente o Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="20a54-243">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

> <span data-ttu-id="20a54-244">**Observação:** Combinar `$orderby` e parâmetros de consulta `$filter` é suportado no ponto de extremidade beta para os seguintes recursos do Microsoft Azure Active Directory e suas relações que derivam de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true):</span><span class="sxs-lookup"><span data-stu-id="20a54-244">**Note:** Combining `$orderby` and `$filter` query parameters is supported on the beta endpoint for the following AD resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true):</span></span>
>
>- [<span data-ttu-id="20a54-245">aplicativo</span><span class="sxs-lookup"><span data-stu-id="20a54-245">application</span></span>](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)
>- [<span data-ttu-id="20a54-246">orgContact</span><span class="sxs-lookup"><span data-stu-id="20a54-246">orgContact</span></span>](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true)
>- [<span data-ttu-id="20a54-247">device</span><span class="sxs-lookup"><span data-stu-id="20a54-247">device</span></span>](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true)
>- [<span data-ttu-id="20a54-248">group</span><span class="sxs-lookup"><span data-stu-id="20a54-248">group</span></span>](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)
>- [<span data-ttu-id="20a54-249">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="20a54-249">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)
>- [<span data-ttu-id="20a54-250">user</span><span class="sxs-lookup"><span data-stu-id="20a54-250">user</span></span>](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)
>
> <span data-ttu-id="20a54-251">Para usar `$orderby` e `$filter` junto ou `$filter` com `endsWith` você precisa:</span><span class="sxs-lookup"><span data-stu-id="20a54-251">To use `$orderby` and `$filter` together, or `$filter` with `endsWith` you need to:</span></span>
>
> - <span data-ttu-id="20a54-252">Adicionar `$count=true` aos parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="20a54-252">Add `$count=true` to the query parameters</span></span>
> - <span data-ttu-id="20a54-253">Adicionar `ConsistencyLevel: eventual` ao cabeçalho de solicitação</span><span class="sxs-lookup"><span data-stu-id="20a54-253">Add `ConsistencyLevel: eventual` request header</span></span>
>
> <span data-ttu-id="20a54-254">Confira [parâmetros opcionais de consulta de usuário](/graph/api/user-list?view=graph-rest-beta&preserve-view=true#optional-query-parameters) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="20a54-254">See [optional user query parameters](/graph/api/user-list?view=graph-rest-beta&preserve-view=true#optional-query-parameters) for more information.</span></span>

## <a name="search-parameter"></a><span data-ttu-id="20a54-255">parâmetro search</span><span class="sxs-lookup"><span data-stu-id="20a54-255">search parameter</span></span>

<span data-ttu-id="20a54-256">Use o parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="20a54-256">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="20a54-257">Usando $search em conjuntos de mensagens</span><span class="sxs-lookup"><span data-stu-id="20a54-257">Using $search on message collections</span></span>

<span data-ttu-id="20a54-258">Você pode pesquisar mensagens com base em um valor nas propriedades de mensagens específicas.</span><span class="sxs-lookup"><span data-stu-id="20a54-258">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="20a54-259">Os resultados da pesquisa são classificados pela data e hora em que a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="20a54-259">The results of the search are sorted by the date and time that the message was sent.</span></span> <span data-ttu-id="20a54-260">Uma solicitação de `$search` retorna até 250 resultados.</span><span class="sxs-lookup"><span data-stu-id="20a54-260">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="20a54-261">Se você realizar uma pesquisa em mensagens e especificar apenas um valor sem as propriedades de mensagens específicas, a pesquisa será realizada nas propriedades de pesquisa padrão **from**, **subject** e **body**.</span><span class="sxs-lookup"><span data-stu-id="20a54-261">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="20a54-262">O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:</span><span class="sxs-lookup"><span data-stu-id="20a54-262">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="20a54-263">[Experimentar no Explorador do Graph][search-example]</span><span class="sxs-lookup"><span data-stu-id="20a54-263">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="20a54-264">Como alternativa, você pode pesquisar mensagens especificando os nomes de propriedade da mensagem na tabela a seguir, que são reconhecidos pela sintaxe da Linguagem de Consulta de Palavra-chave (KQL).</span><span class="sxs-lookup"><span data-stu-id="20a54-264">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="20a54-265">Esses nomes de propriedades correspondem às propriedades definidas na entidade **mensagem** do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="20a54-265">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="20a54-266">O Outlook e outros aplicativos do Microsoft 365 como o SharePoint são compatíveis com a sintaxe KQL, proporcionando a conveniência de um domínio de descoberta comum para seus repositórios de dados.</span><span class="sxs-lookup"><span data-stu-id="20a54-266">Outlook and other Microsoft 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="20a54-267">Propriedades de emails pesquisáveis</span><span class="sxs-lookup"><span data-stu-id="20a54-267">Searchable email property</span></span>                | <span data-ttu-id="20a54-268">Descrição</span><span class="sxs-lookup"><span data-stu-id="20a54-268">Description</span></span> | <span data-ttu-id="20a54-269">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20a54-269">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="20a54-270">**attachment**</span><span class="sxs-lookup"><span data-stu-id="20a54-270">**attachment**</span></span>           | <span data-ttu-id="20a54-271">Os nomes dos arquivos anexados a uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="20a54-271">The names of files attached to an email message.</span></span>|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| <span data-ttu-id="20a54-272">**bcc**</span><span class="sxs-lookup"><span data-stu-id="20a54-272">**bcc**</span></span>           | <span data-ttu-id="20a54-273">O campo **Cco** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="20a54-273">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| <span data-ttu-id="20a54-274">**body**</span><span class="sxs-lookup"><span data-stu-id="20a54-274">**body**</span></span>           | <span data-ttu-id="20a54-275">O corpo de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="20a54-275">The body of an email message.</span></span>|[`me/messages?$search="body:excitement"`][search-body-example]
| <span data-ttu-id="20a54-276">**cc**</span><span class="sxs-lookup"><span data-stu-id="20a54-276">**cc**</span></span>           | <span data-ttu-id="20a54-277">O campo **Cc** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="20a54-277">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| <span data-ttu-id="20a54-278">**from**</span><span class="sxs-lookup"><span data-stu-id="20a54-278">**from**</span></span>           | <span data-ttu-id="20a54-279">O remetente de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="20a54-279">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| <span data-ttu-id="20a54-280">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="20a54-280">**hasAttachment**</span></span> | <span data-ttu-id="20a54-281">Verdadeiro se uma mensagem de email contiver um anexo que não seja um anexo embutido, caso contrário, falso.</span><span class="sxs-lookup"><span data-stu-id="20a54-281">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> |[`me/messages?$search="hasAttachments:true"`][search-from-example]
| <span data-ttu-id="20a54-282">**importance**</span><span class="sxs-lookup"><span data-stu-id="20a54-282">**importance**</span></span>           | <span data-ttu-id="20a54-283">A prioridade de uma mensagem de email, que um remetente pode especificar ao enviar uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="20a54-283">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="20a54-284">Os valores possíveis são `low`, `medium` ou `high`.</span><span class="sxs-lookup"><span data-stu-id="20a54-284">The possible values are `low`, `medium`, or `high`.</span></span>|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| <span data-ttu-id="20a54-285">**kind**</span><span class="sxs-lookup"><span data-stu-id="20a54-285">**kind**</span></span>           | <span data-ttu-id="20a54-286">O tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="20a54-286">The type of message.</span></span> <span data-ttu-id="20a54-287">Os valores possíveis são `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` ou `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="20a54-287">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| <span data-ttu-id="20a54-288">**participants**</span><span class="sxs-lookup"><span data-stu-id="20a54-288">**participants**</span></span>           | <span data-ttu-id="20a54-289">Os campos **de**, **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="20a54-289">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="participants:danas"`][search-part-example]
| <span data-ttu-id="20a54-290">**received**</span><span class="sxs-lookup"><span data-stu-id="20a54-290">**received**</span></span>           | <span data-ttu-id="20a54-291">A data em que uma mensagem de email foi recebida pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="20a54-291">The date that an email message was received by a recipient.</span></span>|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| <span data-ttu-id="20a54-292">**recipients**</span><span class="sxs-lookup"><span data-stu-id="20a54-292">**recipients**</span></span>           | <span data-ttu-id="20a54-293">Os campos **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="20a54-293">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| <span data-ttu-id="20a54-294">**sent**</span><span class="sxs-lookup"><span data-stu-id="20a54-294">**sent**</span></span>           | <span data-ttu-id="20a54-295">A data em que uma mensagem de email foi enviada pelo remetente.</span><span class="sxs-lookup"><span data-stu-id="20a54-295">The date that an email message was sent by the sender.</span></span>|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| <span data-ttu-id="20a54-296">**size**</span><span class="sxs-lookup"><span data-stu-id="20a54-296">**size**</span></span>           | <span data-ttu-id="20a54-297">O tamanho de um item em bytes.</span><span class="sxs-lookup"><span data-stu-id="20a54-297">The size of an item in bytes.</span></span>|[`me/messages?$search="size:1..500000"`][search-size-example]
| <span data-ttu-id="20a54-298">**subject**</span><span class="sxs-lookup"><span data-stu-id="20a54-298">**subject**</span></span>           | <span data-ttu-id="20a54-299">O texto na linha de assunto de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="20a54-299">The text in the subject line of an email message.</span></span> <span data-ttu-id="20a54-300">.</span><span class="sxs-lookup"><span data-stu-id="20a54-300">.</span></span>|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| <span data-ttu-id="20a54-301">**to**</span><span class="sxs-lookup"><span data-stu-id="20a54-301">**to**</span></span>           | <span data-ttu-id="20a54-302">O campo **para** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="20a54-302">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


<span data-ttu-id="20a54-303">Para saber mais sobre as propriedades de email pesquisáveis, KQL como a sintaxe, operadores com suporte e dicas de pesquisa, confira os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="20a54-303">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="20a54-304">[Propriedades pesquisáveis no Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span><span class="sxs-lookup"><span data-stu-id="20a54-304">[Searchable properties in Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- [<span data-ttu-id="20a54-305">Referência de sintaxe da Linguagem de Consulta de Palavra-chave (KQL)</span><span class="sxs-lookup"><span data-stu-id="20a54-305">Keyword Query Language (KQL) syntax reference</span></span>](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- [<span data-ttu-id="20a54-306">Propriedades da mensagem e operadores de pesquisa para a Descoberta eletrônica In-loco no Exchange 2016</span><span class="sxs-lookup"><span data-stu-id="20a54-306">Message properties and search operators for In-Place eDiscovery in Exchange 2016</span></span>](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators)

### <a name="using-search-on-person-collections"></a><span data-ttu-id="20a54-307">Usando $search em conjuntos de pessoas</span><span class="sxs-lookup"><span data-stu-id="20a54-307">Using $search on person collections</span></span>

<span data-ttu-id="20a54-308">Você pode usar a API de Pessoas do Microsoft Graph para recuperar as pessoas mais relevantes para um usuário.</span><span class="sxs-lookup"><span data-stu-id="20a54-308">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user.</span></span> <span data-ttu-id="20a54-309">A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="20a54-309">Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="20a54-310">A API de Pessoas é compatível com o parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="20a54-310">The People API supports the `$search` query parameter.</span></span> <span data-ttu-id="20a54-311">Uma solicitação de `$search` retorna até 250 resultados.</span><span class="sxs-lookup"><span data-stu-id="20a54-311">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="20a54-312">As pesquisas de pessoas ocorrem nas propriedades **displayName** e **emailAddress** do recurso [person](/graph/api/resources/person).</span><span class="sxs-lookup"><span data-stu-id="20a54-312">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](/graph/api/resources/person) resource.</span></span>

<span data-ttu-id="20a54-313">A seguinte solicitação faz uma pesquisa por uma pessoa chamada "Clara Barbosa" nas propriedades **displayName** e **emailAddress** em todos os indivíduos no conjunto de **Pessoas** do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="20a54-313">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="20a54-314">Como uma pessoa denominada "Clara Barbosa" é relevante para o usuário conectado, as informações para "Clara Barbosa" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="20a54-314">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="20a54-315">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="20a54-315">The following example shows the response.</span></span> 

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

<span data-ttu-id="20a54-316">Saiba mais sobre a API de Pessoas em [Obter informações sobre pessoas relevantes](./people-example.md#search-people).</span><span class="sxs-lookup"><span data-stu-id="20a54-316">To learn more about the People API, see [Get information about relevant people](./people-example.md#search-people).</span></span>  

### <a name="using-search-on-directory-object-collections"></a><span data-ttu-id="20a54-317">Como usar $search nos conjuntos de objetos do diretório</span><span class="sxs-lookup"><span data-stu-id="20a54-317">Using $search on directory object collections</span></span>

<span data-ttu-id="20a54-318">Você pode usar um parâmetro de consulta de `$search` para filtrar resultados usando a geração de tokens.</span><span class="sxs-lookup"><span data-stu-id="20a54-318">You can use a `$search` query parameter to filter results using tokenization.</span></span> <span data-ttu-id="20a54-319">A pesquisa tokenizada funciona extraindo palavras da cadeia de caracteres de entrada e de saída, usando espaços, números, uso de maiúsculas/minúsculas e símbolos para separar as palavras, da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="20a54-319">Tokenized search works by extracting words from your input and output string, using spaces, numbers, different casing, and symbols to separate the words, as follow:</span></span>

* <span data-ttu-id="20a54-320">**Espaços**: `hello world` => `hello`, `world`</span><span class="sxs-lookup"><span data-stu-id="20a54-320">**Spaces**: `hello world` => `hello`, `world`</span></span>
* <span data-ttu-id="20a54-321">**Caixa diferente**⁽¹⁾: `HelloWorld` ou `helloWORLD` => `hello`, `world`</span><span class="sxs-lookup"><span data-stu-id="20a54-321">**Different casing**⁽¹⁾: `HelloWorld` or `helloWORLD` => `hello`, `world`</span></span>
* <span data-ttu-id="20a54-322">**Símbolos**⁽²⁾: `hello.world` => `hello`, `.`,`world`, `helloworld`</span><span class="sxs-lookup"><span data-stu-id="20a54-322">**Symbols**⁽²⁾: `hello.world` => `hello`, `.`, `world`, `helloworld`</span></span>
* <span data-ttu-id="20a54-323">**Números**: `hello123world` => `hello`,`123`, `world`</span><span class="sxs-lookup"><span data-stu-id="20a54-323">**Numbers**: `hello123world` => `hello`, `123`, `world`</span></span>

<span data-ttu-id="20a54-324">⁽¹⁾ Atualmente, a tokenização só funciona quando a caixa está mudando de minúsculas para maiúsculas, portanto, `HELLOworld` é considerada um único token: `helloworld`, e `HelloWORld` tem dois tokens: `hello`, `world`.</span><span class="sxs-lookup"><span data-stu-id="20a54-324">⁽¹⁾ Currently, tokenization only works when the casing is changing from lowercase to uppercase, so `HELLOworld` is considered a single token: `helloworld`, and `HelloWORld` is two tokens: `hello`, `world`.</span></span> <span data-ttu-id="20a54-325">⁽²⁾ A lógica de tokenização também combina palavras que são separadas apenas por símbolos; por exemplo, pesquisar por `helloworld` irá localizar `hello-world` e `hello.world`.</span><span class="sxs-lookup"><span data-stu-id="20a54-325">⁽²⁾ Tokenization logic also combines words that are separated only by symbols; for example, searching for `helloworld` will find `hello-world` and `hello.world`.</span></span>

> <span data-ttu-id="20a54-326">**Observação**: após a geração de tokens, os tokens são combinados independentemente da capitalização original e são combinados em qualquer ordem.</span><span class="sxs-lookup"><span data-stu-id="20a54-326">**Note**: after tokenization, the tokens are matched independently of the original casing, and they are matched in any order.</span></span>
> <span data-ttu-id="20a54-327">O parâmetro de consulta de `$search` em coleções de objetos de diretório **requer** um cabeçalho de solicitação especial: `ConsistencyLevel: eventual`.</span><span class="sxs-lookup"><span data-stu-id="20a54-327">`$search` query parameter on directory objects collections **requires** a special request header: `ConsistencyLevel: eventual`.</span></span>

<span data-ttu-id="20a54-328">O suporte tokenizado à pesquisa funciona apenas nos campos **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="20a54-328">The tokenized search support works only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="20a54-329">Qualquer campo pode ser inserido em `$search`; campos diferentes de **displayName** e **descrição** padrão para `$filter` comportamento de startswith.</span><span class="sxs-lookup"><span data-stu-id="20a54-329">Any field can be put in `$search`; fields other than **displayName** and **description** default to `$filter` startswith behavior.</span></span> <span data-ttu-id="20a54-330">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="20a54-330">For example:</span></span>

`https://graph.microsoft.com/beta/groups/?$search="displayName:OneVideo"`

<span data-ttu-id="20a54-331">procurar todos os grupos com nomes de exibição que se pareçam com "OneVideo".</span><span class="sxs-lookup"><span data-stu-id="20a54-331">This looks for all groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="20a54-332">O parâmetro `$search` também pode ser usado junto com o `$filter`.</span><span class="sxs-lookup"><span data-stu-id="20a54-332">`$search` can be used together with `$filter` as well.</span></span> <span data-ttu-id="20a54-333">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="20a54-333">For example:</span></span>

`https://graph.microsoft.com/beta/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"`

<span data-ttu-id="20a54-334">procurar todos os grupos habilitados para email com nomes de exibição que se pareçam com "OneVideo".</span><span class="sxs-lookup"><span data-stu-id="20a54-334">This looks for all mail-enabled groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="20a54-335">Os resultados são restringidos com base em uma conjunção lógica (um “AND”) do parâmetro `$filter` e na consulta inteira no parâmetro `$search`.</span><span class="sxs-lookup"><span data-stu-id="20a54-335">The results are restricted based on a logical conjunction (an "AND") of the `$filter` and the entire query in the `$search`.</span></span> <span data-ttu-id="20a54-336">O texto da pesquisa é tokenizado com base nas letras maiúsculas ou minúsculas, mas as equiparações são executadas de maneira insensível ao fato de a letra ser maiúscula ou minúscula.</span><span class="sxs-lookup"><span data-stu-id="20a54-336">The search text is tokenized based on casing, but matches are performed in a case-insensitive manner.</span></span> <span data-ttu-id="20a54-337">Por exemplo, "OneVideo" seria dividido em dois tokens de entrada "one" e "video", mas correspondendo a propriedades que não diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="20a54-337">For example, "OneVideo" would be split into two input tokens "one" and "video", but matches properties insensitive to case.</span></span>

<span data-ttu-id="20a54-338">A sintaxe da pesquisa segue as seguintes regras:</span><span class="sxs-lookup"><span data-stu-id="20a54-338">The syntax of search follows these rules:</span></span>

* <span data-ttu-id="20a54-339">Formato genérico: $search="clause1" \[AND \| OR\] "\[clauseX\]"\.</span><span class="sxs-lookup"><span data-stu-id="20a54-339">Generic format: $search="clause1" \[AND \| OR\] "\[clauseX\]"\.</span></span>
* <span data-ttu-id="20a54-340">O número de cláusulas (clause) não é limitado.</span><span class="sxs-lookup"><span data-stu-id="20a54-340">Any number of clauses is supported.</span></span> <span data-ttu-id="20a54-341">O uso de parênteses para a precedência também é suportado.</span><span class="sxs-lookup"><span data-stu-id="20a54-341">Parentheses for precedence is also supported.</span></span>
* <span data-ttu-id="20a54-342">A sintaxe para cada cláusula é: “\<property>:\<text to search>”.</span><span class="sxs-lookup"><span data-stu-id="20a54-342">The syntax for each clause is: "\<property>:\<text to search>".</span></span>
* <span data-ttu-id="20a54-343">O nome da propriedade deve ser especificado na cláusula.</span><span class="sxs-lookup"><span data-stu-id="20a54-343">The property name must be specified in clause.</span></span> <span data-ttu-id="20a54-344">Qualquer propriedade que possa ser usada em `$filter` também pode ser usada dentro de `$search`.</span><span class="sxs-lookup"><span data-stu-id="20a54-344">Any property that can be used in `$filter` can also be used inside `$search`.</span></span> <span data-ttu-id="20a54-345">Dependendo da propriedade, o comportamento da pesquisa será "search" ou, se “search” não for suportado na propriedade, "startswith".</span><span class="sxs-lookup"><span data-stu-id="20a54-345">Depending on the property, the search behavior is either "search" or "startswith" if search is not supported on the property.</span></span>
* <span data-ttu-id="20a54-346">Todas as partes de cláusula devem ser colocadas entre aspas duplas.</span><span class="sxs-lookup"><span data-stu-id="20a54-346">The whole clause part must be put inside double quotes.</span></span>
* <span data-ttu-id="20a54-347">Os operadores lógicos “AND” e “OR” devem ser colocados fora das aspas duplas.</span><span class="sxs-lookup"><span data-stu-id="20a54-347">Logical operator 'AND' 'OR' must be put outside double quotes.</span></span> <span data-ttu-id="20a54-348">Devem sempre ser grafados em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="20a54-348">They must be in upper case.</span></span>
* <span data-ttu-id="20a54-349">Considerando que toda a parte da cláusula precisa ser colocada entre aspas duplas, se contiver aspas duplas e barra invertida, as barras invertidas deverão ser usadas para escapar as aspas.</span><span class="sxs-lookup"><span data-stu-id="20a54-349">Given that the whole clause part needs to be put inside double quotes, if it contains double quote and backslash, it needs to be escaped with a backslash.</span></span> <span data-ttu-id="20a54-350">Não é preciso escapar nenhum outro caractere.</span><span class="sxs-lookup"><span data-stu-id="20a54-350">No other characters need to be escaped.</span></span>

<span data-ttu-id="20a54-351">A tabela a seguir mostra alguns exemplos.</span><span class="sxs-lookup"><span data-stu-id="20a54-351">The following table shows some examples.</span></span>

| <span data-ttu-id="20a54-352">Classe de objeto</span><span class="sxs-lookup"><span data-stu-id="20a54-352">Object class</span></span> | <span data-ttu-id="20a54-353">Descrição</span><span class="sxs-lookup"><span data-stu-id="20a54-353">Description</span></span> | <span data-ttu-id="20a54-354">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20a54-354">Example</span></span> |
| ------------ | ----------- | ------- |
| <span data-ttu-id="20a54-355">Usuário</span><span class="sxs-lookup"><span data-stu-id="20a54-355">User</span></span> | <span data-ttu-id="20a54-356">O caderno de endereços exibe o nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="20a54-356">Address book display name of the user.</span></span> | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr"` |
| <span data-ttu-id="20a54-357">Usuário</span><span class="sxs-lookup"><span data-stu-id="20a54-357">User</span></span> | <span data-ttu-id="20a54-358">O caderno de endereços exibe o nome ou o email do usuário.</span><span class="sxs-lookup"><span data-stu-id="20a54-358">Address book display name or mail of the user.</span></span> | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"` |
| <span data-ttu-id="20a54-359">Grupo</span><span class="sxs-lookup"><span data-stu-id="20a54-359">Group</span></span> | <span data-ttu-id="20a54-360">O caderno de endereços exibe o nome ou a descrição de um grupo.</span><span class="sxs-lookup"><span data-stu-id="20a54-360">Address book display name or description of the group.</span></span> | `https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")` |
| <span data-ttu-id="20a54-361">Grupo</span><span class="sxs-lookup"><span data-stu-id="20a54-361">Group</span></span> | <span data-ttu-id="20a54-362">Nome de exibição do catálogo de endereços em um grupo habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="20a54-362">Address book display name on a mail-enabled group.</span></span> | `https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"` |

<span data-ttu-id="20a54-363">Ambas as entradas da cadeia de caracteres fornecidas em `$search`, bem como as propriedades pesquisáveis, são divididas em partes por espaços, uso de maiúsculas/minúsculas e tipos de caracteres (números e caracteres especiais).</span><span class="sxs-lookup"><span data-stu-id="20a54-363">Both the string inputs you provide in `$search`, as well as the searchable properties, are split up into parts by spaces, different casing, and character types (numbers and special characters).</span></span>

## <a name="select-parameter"></a><span data-ttu-id="20a54-364">parâmetro select</span><span class="sxs-lookup"><span data-stu-id="20a54-364">select parameter</span></span>

<span data-ttu-id="20a54-365">Use o parâmetro de consulta `$select` para retornar um conjunto de propriedades diferente do padrão definido para um recurso individual ou um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="20a54-365">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="20a54-366">Com $select, você pode especificar um subconjunto ou um superconjunto das propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="20a54-366">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="20a54-367">Por exemplo, ao recuperar as mensagens do usuário conectado, você pode especificar que somente as propriedades **from** e **subject** sejam retornadas:</span><span class="sxs-lookup"><span data-stu-id="20a54-367">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="20a54-368">[Experimentar no Explorador do Graph][select-example]</span><span class="sxs-lookup"><span data-stu-id="20a54-368">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="20a54-369">**Importante:** Em geral, recomendamos que você use `$select` para limitar as propriedades retornadas por uma consulta àqueles exigidas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="20a54-369">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="20a54-370">Isso se aplica particularmente a consultas com o potencial de retornar um conjunto de resultados amplo.</span><span class="sxs-lookup"><span data-stu-id="20a54-370">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="20a54-371">Limitar as propriedades retornadas em cada linha reduzirá a carga de rede e ajudará a melhorar o desempenho do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="20a54-371">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="20a54-p138">No `v1.0`, alguns recursos do Azure AD que derivam de [directoryObject](/graph/api/resources/directoryobject), como [usuário](/graph/api/resources/user) e [grupo](/graph/api/resources/group), retornam um subconjunto limitado padrão de propriedades em leituras. Para esses recursos, você deve usar `$select` para retornar propriedades fora do conjunto padrão.</span><span class="sxs-lookup"><span data-stu-id="20a54-p138">In `v1.0`, some Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject), like [user](/graph/api/resources/user) and [group](/graph/api/resources/group), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="20a54-374">parâmetro skip</span><span class="sxs-lookup"><span data-stu-id="20a54-374">skip parameter</span></span>

<span data-ttu-id="20a54-p139">Use o parâmetro de consulta `$skip` para definir o número de itens para ignorar no início de um conjunto. Por exemplo, a solicitação a seguir retorna eventos para o usuário classificadas por data de criação, começando com o evento 21 no conjunto:</span><span class="sxs-lookup"><span data-stu-id="20a54-p139">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="20a54-377">[Experimentar no Explorador do Graph][skip-example]</span><span class="sxs-lookup"><span data-stu-id="20a54-377">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="20a54-378">**Observação:** algumas APIs do Microsoft Graph, como Email e Calendário do Outlook (**message**, **event** e **calendar**), usam `$skip` para implementar a paginação.</span><span class="sxs-lookup"><span data-stu-id="20a54-378">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="20a54-379">Quando os resultados de uma consulta ocuparem várias páginas, essas APIs retornarão uma propriedade `@odata:nextLink` com uma URL que contém um parâmetro `$skip`.</span><span class="sxs-lookup"><span data-stu-id="20a54-379">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="20a54-380">Você pode usar essa URL para retornar a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="20a54-380">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="20a54-381">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="20a54-381">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="20a54-382">parâmetro skipToken</span><span class="sxs-lookup"><span data-stu-id="20a54-382">skipToken parameter</span></span>

<span data-ttu-id="20a54-383">Algumas solicitações retornam várias páginas de dados, devido à paginação do lado do servidor ou devido ao uso do parâmetro [`$top`](#top-parameter) para limitar o tamanho da página da resposta.</span><span class="sxs-lookup"><span data-stu-id="20a54-383">Some requests return multiple pages of data, either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response.</span></span> <span data-ttu-id="20a54-384">Muitas APIs do Microsoft Graph usam o parâmetro de consulta `skipToken` para fazer referência a páginas subsequentes do resultado.</span><span class="sxs-lookup"><span data-stu-id="20a54-384">Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result.</span></span>  
<span data-ttu-id="20a54-385">O parâmetro `$skiptoken` contém um token opaco que faz referência à próxima página de resultados e é retornado na URL fornecida na propriedade `@odata.nextLink` na resposta.</span><span class="sxs-lookup"><span data-stu-id="20a54-385">The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response.</span></span> <span data-ttu-id="20a54-386">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="20a54-386">To learn more, see [Paging](./paging.md).</span></span>
> <span data-ttu-id="20a54-387">**Observação:** se você estiver usando OData Count (adicionando `$count=true` na querystring), a propriedade `@odata.count` estará presente somente na primeira página.</span><span class="sxs-lookup"><span data-stu-id="20a54-387">**Note:** if you're using OData Count (adding `$count=true` in the querystring), the `@odata.count` property will be present only in the first page.</span></span>

## <a name="top-parameter"></a><span data-ttu-id="20a54-388">parâmetro top</span><span class="sxs-lookup"><span data-stu-id="20a54-388">top parameter</span></span>

<span data-ttu-id="20a54-389">Use o parâmetro de consulta `$top` para especificar o tamanho de página do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="20a54-389">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="20a54-390">Se restarem mais itens no conjunto de resultados, o corpo da resposta conterá um parâmetro `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="20a54-390">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="20a54-391">Esse parâmetro contém uma URL que você pode usar para obter a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="20a54-391">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="20a54-392">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="20a54-392">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="20a54-393">O valor mínimo de $top é 1 e o máximo depende da API correspondente.</span><span class="sxs-lookup"><span data-stu-id="20a54-393">The minimum value of $top is 1 and the maximum depends on the corresponding API.</span></span>  

<span data-ttu-id="20a54-394">Por exemplo, a seguinte solicitação de [lista de mensagens](/graph/api/user-list-messages) retorna as cinco primeiras mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="20a54-394">For example, the following [list messages](/graph/api/user-list-messages) request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="20a54-395">[Experimentar no Explorador do Graph][top-example]</span><span class="sxs-lookup"><span data-stu-id="20a54-395">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="20a54-396">Tratamento de erro para parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="20a54-396">Error handling for query parameters</span></span>

<span data-ttu-id="20a54-p144">Algumas solicitações retornarão uma mensagem de erro se não houver suporte para um parâmetro de consulta especificado. Por exemplo, você não pode usar `$expand` na relação `user/photo`.</span><span class="sxs-lookup"><span data-stu-id="20a54-p144">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="20a54-399">No entanto, é importante observar que os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente.</span><span class="sxs-lookup"><span data-stu-id="20a54-399">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="20a54-400">Isso pode ser verdadeiro para parâmetros de consulta sem suporte, bem como para combinações de parâmetros de consulta sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20a54-400">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="20a54-401">Nesses casos, você deve examinar os dados retornados pela solicitação para determinar se os parâmetros de consulta que especificou tiveram o efeito desejado.</span><span class="sxs-lookup"><span data-stu-id="20a54-401">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

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

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.0
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0



## <a name="see-also"></a><span data-ttu-id="20a54-402">Confira também</span><span class="sxs-lookup"><span data-stu-id="20a54-402">See also</span></span>

- [<span data-ttu-id="20a54-403">Limitações de parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="20a54-403">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)
