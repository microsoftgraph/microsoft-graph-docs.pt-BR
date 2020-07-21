---
title: Usar parâmetros de consulta para personalizar respostas
description: O Microsoft Graph fornece parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta.
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: bd87841a6c7a46d485c7ccd2b0f601f012712f63
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183838"
---
# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="b9226-103">Usar parâmetros de consulta para personalizar respostas</span><span class="sxs-lookup"><span data-stu-id="b9226-103">Use query parameters to customize responses</span></span>

<span data-ttu-id="b9226-104">O Microsoft Graph fornece suporte a parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b9226-104">Microsoft Graph supports optional query parameters that you can use to specify and control the amount of data returned in a response.</span></span> <span data-ttu-id="b9226-105">O suporte para os parâmetros de consulta exatos variam de uma operação de API para outra e, dependendo da API, podem diferir entre os pontos de extremidade v1.0 e beta.</span><span class="sxs-lookup"><span data-stu-id="b9226-105">The support for the exact query parameters varies from one API operation to another, and depending on the API, can differ between the v1.0 and beta endpoints.</span></span> 

> [!TIP] 
> <span data-ttu-id="b9226-106">No ponto de extremidade beta, o prefixo `$` é opcional.</span><span class="sxs-lookup"><span data-stu-id="b9226-106">On the beta endpoint, the `$` prefix is optional.</span></span> <span data-ttu-id="b9226-107">Por exemplo, em vez de `$filter`, você pode usar `filter`.</span><span class="sxs-lookup"><span data-stu-id="b9226-107">For example, instead of `$filter`, you can use `filter`.</span></span> <span data-ttu-id="b9226-108">No ponto de extremidade v1, o prefixo `$` é opcional apenas para um subconjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="b9226-108">On the v1 endpoint, the `$` prefix is optional for only a subset of APIs.</span></span> <span data-ttu-id="b9226-109">Para simplificar, inclua sempre `$` se estiver usando o ponto de extremidade v1.</span><span class="sxs-lookup"><span data-stu-id="b9226-109">For simplicity, always include `$` if using the v1 endpoint.</span></span>

<span data-ttu-id="b9226-110">Os parâmetros de consulta podem ser opções de consulta de sistema OData ou outros parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="b9226-110">Query parameters can be OData system query options or other query parameters.</span></span> 

> [!VIDEO https://www.youtube-nocookie.com/embed/7BuFv3yETi4]

## <a name="odata-system-query-options"></a><span data-ttu-id="b9226-111">Opções de consulta de sistema OData</span><span class="sxs-lookup"><span data-stu-id="b9226-111">OData system query options</span></span>
<span data-ttu-id="b9226-112">Uma operação de API do Microsoft Graph pode oferecer suporte a uma ou mais das seguintes opções de consulta de sistema OData.</span><span class="sxs-lookup"><span data-stu-id="b9226-112">A Microsoft Graph API operation might support one or more of the following OData system query options.</span></span> <span data-ttu-id="b9226-113">Essas opções de consulta são compatíveis com a [linguagem de consulta OData V4][odata-query].</span><span class="sxs-lookup"><span data-stu-id="b9226-113">These query options are compatible with the [OData V4 query language][odata-query].</span></span>

><span data-ttu-id="b9226-114">**Observação:** o OData 4.0 oferece suporte às opções de consulta do sistema apenas em operações GET.</span><span class="sxs-lookup"><span data-stu-id="b9226-114">**Note:** OData 4.0 supports system query options in only GET operations.</span></span>

<span data-ttu-id="b9226-115">Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="b9226-115">Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="b9226-116">Nome</span><span class="sxs-lookup"><span data-stu-id="b9226-116">Name</span></span>                     | <span data-ttu-id="b9226-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9226-117">Description</span></span> | <span data-ttu-id="b9226-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9226-118">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="b9226-119">$count</span><span class="sxs-lookup"><span data-stu-id="b9226-119">$count</span></span>](#count-parameter)         | <span data-ttu-id="b9226-120">Recupera a contagem total de recursos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="b9226-120">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="b9226-121">$expand</span><span class="sxs-lookup"><span data-stu-id="b9226-121">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="b9226-122">Recupera os recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="b9226-122">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="b9226-123">$filter</span><span class="sxs-lookup"><span data-stu-id="b9226-123">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="b9226-124">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="b9226-124">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="b9226-125">$format</span><span class="sxs-lookup"><span data-stu-id="b9226-125">$format</span></span>](#format-parameter)       | <span data-ttu-id="b9226-126">Retorna os resultados no formato de mídia especificado.</span><span class="sxs-lookup"><span data-stu-id="b9226-126">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="b9226-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="b9226-127">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="b9226-128">Ordena os resultados.</span><span class="sxs-lookup"><span data-stu-id="b9226-128">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="b9226-129">$search</span><span class="sxs-lookup"><span data-stu-id="b9226-129">$search</span></span>](#search-parameter)       | <span data-ttu-id="b9226-130">Retorna os resultados com base nos critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="b9226-130">Returns results based on search criteria.</span></span> |[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="b9226-131">$select</span><span class="sxs-lookup"><span data-stu-id="b9226-131">$select</span></span>](#select-parameter)       | <span data-ttu-id="b9226-132">Filtra as propriedades (colunas).</span><span class="sxs-lookup"><span data-stu-id="b9226-132">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="b9226-133">$skip</span><span class="sxs-lookup"><span data-stu-id="b9226-133">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="b9226-p104">Índices em um conjunto de resultados. Também usado por algumas APIs para implementar a paginação e pode ser usado com `$top` para paginar resultados manualmente.</span><span class="sxs-lookup"><span data-stu-id="b9226-p104">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="b9226-136">$top</span><span class="sxs-lookup"><span data-stu-id="b9226-136">$top</span></span>](#top-parameter)             | <span data-ttu-id="b9226-137">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="b9226-137">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a><span data-ttu-id="b9226-138">Outros parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="b9226-138">Other query parameters</span></span>

| <span data-ttu-id="b9226-139">Nome</span><span class="sxs-lookup"><span data-stu-id="b9226-139">Name</span></span>                     | <span data-ttu-id="b9226-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9226-140">Description</span></span> | <span data-ttu-id="b9226-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9226-141">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="b9226-142">$skipToken</span><span class="sxs-lookup"><span data-stu-id="b9226-142">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="b9226-p105">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas. (Algumas APIs usam `$skip` em vez disso.)</span><span class="sxs-lookup"><span data-stu-id="b9226-p105">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a><span data-ttu-id="b9226-145">Outros recursos de URL OData</span><span class="sxs-lookup"><span data-stu-id="b9226-145">Other OData URL capabilities</span></span>

<span data-ttu-id="b9226-146">Os seguintes recursos OData 4.0 são segmentos de URL, não parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="b9226-146">The following OData 4.0 capabilities are URL segments, not query parameters.</span></span>

| <span data-ttu-id="b9226-147">Nome</span><span class="sxs-lookup"><span data-stu-id="b9226-147">Name</span></span>                     | <span data-ttu-id="b9226-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9226-148">Description</span></span> | <span data-ttu-id="b9226-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9226-149">Example</span></span> 
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="b9226-150">$ref</span><span class="sxs-lookup"><span data-stu-id="b9226-150">$ref</span></span>](/graph/api/group-post-members?view=graph-rest-1.0&tabs=http) | <span data-ttu-id="b9226-151">Atualiza a associação de entidades a uma coleção.</span><span class="sxs-lookup"><span data-stu-id="b9226-151">Updates entities membership to a collection.</span></span> | `POST /groups/{id}/members/$ref` |
| [<span data-ttu-id="b9226-152">$value</span><span class="sxs-lookup"><span data-stu-id="b9226-152">$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="b9226-153">Recupera ou atualiza o valor binário de um item.</span><span class="sxs-lookup"><span data-stu-id="b9226-153">Retrieves or updates the binary value of an item.</span></span> | `GET /me/photo/$value` |

## <a name="encoding-query-parameters"></a><span data-ttu-id="b9226-154">Codificação de parâmetros da consulta</span><span class="sxs-lookup"><span data-stu-id="b9226-154">Encoding query parameters</span></span>

<span data-ttu-id="b9226-155">Os valores dos parâmetros da consulta devem ser codificados por porcentagem.</span><span class="sxs-lookup"><span data-stu-id="b9226-155">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="b9226-156">Muitas ferramentas, navegadores e clientes HTTP (como o [Explorador do Graph][graph-explorer]) ajudarão você com isso.</span><span class="sxs-lookup"><span data-stu-id="b9226-156">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="b9226-157">Se uma consulta está falhando, uma causa possível é a falha na codificação adequada dos valores dos parâmetros da consulta.</span><span class="sxs-lookup"><span data-stu-id="b9226-157">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="b9226-158">Uma URL descodificada é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="b9226-158">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="b9226-159">Uma URL codificada adequadamente é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="b9226-159">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

### <a name="escaping-single-quotes"></a><span data-ttu-id="b9226-160">Escape de aspas simples</span><span class="sxs-lookup"><span data-stu-id="b9226-160">Escaping single quotes</span></span>

<span data-ttu-id="b9226-161">Para pedidos que usem aspas simples, se os valores de qualquer parâmetro também contém aspas, elas devem ter escape duplo. Caso contrário, a solicitação falhará devido a sintaxe inválida.</span><span class="sxs-lookup"><span data-stu-id="b9226-161">For requests that use single quotes, if any parameter values also contain single quotes, those must be double escaped; otherwise, the request will fail due to invalid syntax.</span></span> <span data-ttu-id="b9226-162">No exemplo, o valor de cadeia de caracteres `let''s meet for lunch?` tem o escape de aspas simples.</span><span class="sxs-lookup"><span data-stu-id="b9226-162">In the example, the string value `let''s meet for lunch?` has the single quote escaped.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a><span data-ttu-id="b9226-163">parâmetro count</span><span class="sxs-lookup"><span data-stu-id="b9226-163">count parameter</span></span>

<span data-ttu-id="b9226-164">Use o parâmetro de consulta `$count` para incluir uma contagem do número total de itens em um conjunto, juntamente com a página de valores de dados retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b9226-164">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="b9226-165">Por exemplo, a solicitação a seguir retornará tanto o conjunto **contato** do usuário atual quanto o número de itens no conjunto **contato** na propriedade `@odata.count`.</span><span class="sxs-lookup"><span data-stu-id="b9226-165">For example, the following request returns both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="b9226-166">Experimente o Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="b9226-166">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


<span data-ttu-id="b9226-167">O parâmetro de consulta `$count` é compatível com esses conjuntos de recursos e suas relações, derivadas do [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta):</span><span class="sxs-lookup"><span data-stu-id="b9226-167">The `$count` query parameter is supported for these collections of resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta):</span></span>
- [<span data-ttu-id="b9226-168">application</span><span class="sxs-lookup"><span data-stu-id="b9226-168">application</span></span>](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-beta)
- [<span data-ttu-id="b9226-169">orgContact</span><span class="sxs-lookup"><span data-stu-id="b9226-169">orgContact</span></span>](https://docs.microsoft.com/graph/api/resources/orgcontact?view=graph-rest-beta)
- [<span data-ttu-id="b9226-170">device</span><span class="sxs-lookup"><span data-stu-id="b9226-170">device</span></span>](https://docs.microsoft.com/graph/api/resources/device?view=graph-rest-beta)
- [<span data-ttu-id="b9226-171">group</span><span class="sxs-lookup"><span data-stu-id="b9226-171">group</span></span>](https://docs.microsoft.com/graph/api/resources/group?view=graph-rest-beta)
- [<span data-ttu-id="b9226-172">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="b9226-172">servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-beta)
- <span data-ttu-id="b9226-173">[users](https://docs.microsoft.com/graph/api/resources/user?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="b9226-173">[users](https://docs.microsoft.com/graph/api/resources/user?view=graph-rest-beta).</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="b9226-174">parâmetro expand</span><span class="sxs-lookup"><span data-stu-id="b9226-174">expand parameter</span></span>

<span data-ttu-id="b9226-175">Muitos recursos do Microsoft Graph expõem as propriedades declaradas do recurso, bem como as relações delas com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="b9226-175">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="b9226-176">Essas relações também são chamadas de propriedades de referência ou propriedades de navegação e podem fazer referência a um único recurso ou a um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="b9226-176">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="b9226-177">Por exemplo, as pastas de email, gerente e subordinados diretos de um usuário são todas expostas como relações.</span><span class="sxs-lookup"><span data-stu-id="b9226-177">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="b9226-p109">Normalmente, você pode consultar as propriedades de um recurso ou uma de suas relações em uma única solicitação, mas não ambas. Você pode usar o parâmetro de cadeia de caracteres de consulta `$expand` para incluir o recurso expandido ou o conjunto referenciado por uma única relação (propriedade de navegação) nos resultados.</span><span class="sxs-lookup"><span data-stu-id="b9226-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="b9226-180">O seguinte exemplo obtém informações de unidade raiz juntamente com os itens filho de nível superior em uma unidade:</span><span class="sxs-lookup"><span data-stu-id="b9226-180">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="b9226-181">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="b9226-181">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="b9226-p110">Com alguns conjuntos de recursos, você também pode especificar as propriedades a serem retornadas nos recursos expandidos adicionando um parâmetro `$select`. O exemplo a seguir executa a mesma consulta que o exemplo anterior, mas usa uma instrução [`$select`](#select-parameter) para limitar as propriedades retornadas para os itens filho expandidos para as propriedades **id** e **name**.</span><span class="sxs-lookup"><span data-stu-id="b9226-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="b9226-184">[Experimentar no Explorador do Graph][expand-example]</span><span class="sxs-lookup"><span data-stu-id="b9226-184">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="b9226-p111">**Observação:** nem todas as relações e recursos dão suporte ao parâmetro de consulta `$expand`. Por exemplo, você pode expandir as relações **directReports**, **manager** e **memberOf** em um usuário, mas não pode expandir suas relações **events**, **messages** ou **photo**. Nem todos os recursos ou relações dão suporte ao uso de `$select` em itens expandidos.</span><span class="sxs-lookup"><span data-stu-id="b9226-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="b9226-188">Com recursos do Azure AD derivados de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), como [user](/graph/api/resources/user?view=graph-rest-1.0) e [group](/graph/api/resources/group?view=graph-rest-1.0), `$expand` só há suporte para `beta`, e normalmente são retornados no máximo 20 itens para a relação expandida.</span><span class="sxs-lookup"><span data-stu-id="b9226-188">With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="b9226-189">parâmetro filter</span><span class="sxs-lookup"><span data-stu-id="b9226-189">filter parameter</span></span>

<span data-ttu-id="b9226-190">Use o parâmetro de consulta `$filter` para recuperar apenas um subconjunto de um conjunto.</span><span class="sxs-lookup"><span data-stu-id="b9226-190">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> <span data-ttu-id="b9226-191">O parâmetro de consulta `$filter` também pode ser usado para recuperar relações como members, memberOf, transitiveMembers e transitiveMemberOf.</span><span class="sxs-lookup"><span data-stu-id="b9226-191">The `$filter` query parameter can also be used to retrieve relationships like members, memberOf, transitiveMembers, and transitiveMemberOf.</span></span> <span data-ttu-id="b9226-192">Por exemplo, obter todos os grupos de segurança dos quais sou membro.</span><span class="sxs-lookup"><span data-stu-id="b9226-192">For example, get all the security groups I'm a member of.</span></span>

<span data-ttu-id="b9226-193">O exemplo a seguir pode ser usado para encontrar usuários cujo nome de exibição começa com a letra “J’: use `startswith`.</span><span class="sxs-lookup"><span data-stu-id="b9226-193">The following example can be used to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="b9226-194">[Experimentar no Explorador do Graph][filter-example]</span><span class="sxs-lookup"><span data-stu-id="b9226-194">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="b9226-195">O suporte para operadores `$filter` varia entre as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b9226-195">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="b9226-196">Os seguintes operadores lógicos geralmente são suportados:</span><span class="sxs-lookup"><span data-stu-id="b9226-196">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="b9226-197">igual a (`eq`)</span><span class="sxs-lookup"><span data-stu-id="b9226-197">equals (`eq`)</span></span>
- <span data-ttu-id="b9226-198">não é igual a (`ne`)</span><span class="sxs-lookup"><span data-stu-id="b9226-198">not equals (`ne`)</span></span>
- <span data-ttu-id="b9226-199">maior que (`gt`)</span><span class="sxs-lookup"><span data-stu-id="b9226-199">greater than (`gt`)</span></span>
- <span data-ttu-id="b9226-200">maior ou igual a (`ge`)</span><span class="sxs-lookup"><span data-stu-id="b9226-200">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="b9226-201">menor que (`lt`), menor ou igual a (`le`)</span><span class="sxs-lookup"><span data-stu-id="b9226-201">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="b9226-202">e (`and`)</span><span class="sxs-lookup"><span data-stu-id="b9226-202">and (`and`)</span></span>
- <span data-ttu-id="b9226-203">ou (`or`)</span><span class="sxs-lookup"><span data-stu-id="b9226-203">or (`or`)</span></span>
- <span data-ttu-id="b9226-204">não (`not`)</span><span class="sxs-lookup"><span data-stu-id="b9226-204">not (`not`)</span></span>
 
<span data-ttu-id="b9226-205">O operador de cadeia de caracteres `startswith` geralmente é suportado.</span><span class="sxs-lookup"><span data-stu-id="b9226-205">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="b9226-206">O operador lambda `any` tem suporte em algumas APIs.</span><span class="sxs-lookup"><span data-stu-id="b9226-206">The `any` lambda operator is supported for some APIs.</span></span> 

> <span data-ttu-id="b9226-207">**Observação:** é necessário [especificar propriedades em determinadas maneiras](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query) ao usar `$filter` e `$orderby` na mesma consulta para obter mensagens.</span><span class="sxs-lookup"><span data-stu-id="b9226-207">**Note:** You must [specify properties in certain ways](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query) when using both `$filter` and `$orderby` in the same query to get messages.</span></span>

<span data-ttu-id="b9226-208">Para ver alguns exemplos de uso, consulte a tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="b9226-208">For some usage examples, see the following table.</span></span> <span data-ttu-id="b9226-209">Para obter mais detalhes sobre a sintaxe `$filter`, confira o [protocolo OData][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="b9226-209">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="b9226-210">A tabela a seguir mostra alguns exemplos que usam o parâmetro de consulta `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b9226-210">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="b9226-211">**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="b9226-211">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="b9226-212">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9226-212">Description</span></span> | <span data-ttu-id="b9226-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9226-213">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="b9226-214">Pesquisar por usuários com o nome Clara entre várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="b9226-214">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| <span data-ttu-id="b9226-215">Obter todos os eventos do usuário conectado que começaram após 01/07/2017.</span><span class="sxs-lookup"><span data-stu-id="b9226-215">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| <span data-ttu-id="b9226-216">Obter todos os emails de um endereço específico recebidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b9226-216">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| <span data-ttu-id="b9226-217">Obter todos os emails recebidos pelo usuário conectado em abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="b9226-217">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| <span data-ttu-id="b9226-218">Obter todos os emails não lidos na caixa de entrada do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b9226-218">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| <span data-ttu-id="b9226-219">Listar todos os grupos do Microsoft 365 em uma organização.</span><span class="sxs-lookup"><span data-stu-id="b9226-219">List all Microsoft 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |
| <span data-ttu-id="b9226-220">Use a conversão OData para obter uma participação transitória em grupos com um nome de exibição que comece com “a”, incluindo o número de objetos retornados.</span><span class="sxs-lookup"><span data-stu-id="b9226-220">Use OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects.</span></span> | [`https://graph.microsoft.com/beta/me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`](https://developer.microsoft.com/graph/graph-explorer?request=me/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName,'a')&method=GET&version=v1.0) |

> <span data-ttu-id="b9226-p116">**Observação:** Os seguintes operadores `$filter` não têm suporte para recursos do Azure AD: `ne`, `gt`, `ge`, `lt`, `le` e `not`. O operador de cadeia de caracteres `contains` atualmente não tem suporte em nenhum recurso do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b9226-p116">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="b9226-223">parâmetro format</span><span class="sxs-lookup"><span data-stu-id="b9226-223">format parameter</span></span>

<span data-ttu-id="b9226-224">Use o parâmetro de consulta `$format` para especificar o formato de mídia dos itens retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b9226-224">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="b9226-225">Por exemplo, a seguinte solicitação retorna os usuários na organização no formato json:</span><span class="sxs-lookup"><span data-stu-id="b9226-225">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="b9226-226">[Experimentar no Explorador do Graph][format-example]</span><span class="sxs-lookup"><span data-stu-id="b9226-226">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="b9226-227">**Observação:** o parâmetro de consulta `$format` é compatível com vários formatos (por exemplo, atom, xml e json), mas os resultados podem não ser retornados em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="b9226-227">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="b9226-228">parâmetro orderby</span><span class="sxs-lookup"><span data-stu-id="b9226-228">orderby parameter</span></span>

<span data-ttu-id="b9226-229">Use o parâmetro de consulta `$orderby` para especificar a ordem de classificação dos itens retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b9226-229">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="b9226-230">Por exemplo, a solicitação a seguir retorna os usuários da organização ordenados por seu nome de exibição:</span><span class="sxs-lookup"><span data-stu-id="b9226-230">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="b9226-231">[Experimentar no Explorador do Graph][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="b9226-231">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="b9226-p117">Você também pode classificar por entidades de tipo complexo. A solicitação abaixo obtém mensagens e as classifica pelo campo **address** da propriedade **from**, que é do tipo complexo **emailAddress**:</span><span class="sxs-lookup"><span data-stu-id="b9226-p117">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="b9226-234">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="b9226-234">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="b9226-235">Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="b9226-235">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="b9226-236">Com algumas APIs, você pode ordenar os resultados em várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="b9226-236">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="b9226-237">Por exemplo, a solicitação a seguir ordena as mensagens na caixa de entrada do usuário primeiro pelo nome da pessoa que enviou, em ordem decrescente (Z – A) e, em seguida, por assunto, em ordem ascendente (padrão).</span><span class="sxs-lookup"><span data-stu-id="b9226-237">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="b9226-238">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="b9226-238">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

> <span data-ttu-id="b9226-239">**Observação:** quando você especifica $filter, o servidor deduz uma ordem de classificação para os resultados.</span><span class="sxs-lookup"><span data-stu-id="b9226-239">**Note:** When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="b9226-240">Se você usar `$orderby` e `$filter` juntos para receber mensagens, como o servidor sempre infere uma ordem de classificação para os resultados de `$filter`, você deve [especificar propriedades de determinadas maneiras](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query).</span><span class="sxs-lookup"><span data-stu-id="b9226-240">If you use both `$orderby` and `$filter` to get messages, because the server always infers a sort order for the results of a `$filter`, you must [specify properties in certain ways](/graph/api/user-list-messages?view=graph-rest-1.0#using-filter-and-orderby-in-the-same-query).</span></span>


<span data-ttu-id="b9226-241">O exemplo a seguir mostra uma consulta filtrada pelas propriedades **subject** e **priority** e classificadas pelas propriedades **subject**, **priority** e **receivedDateTime** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="b9226-241">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="b9226-242">Experimente o Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="b9226-242">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

> <span data-ttu-id="b9226-243">**Observação:** Combinar `$orderby` e parâmetros de consulta `$filter` é suportado no ponto de extremidade beta para os seguintes recursos do Microsoft Azure Active Directory e suas relações que derivam de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta):</span><span class="sxs-lookup"><span data-stu-id="b9226-243">**Note:** Combining `$orderby` and `$filter` query parameters is supported on the beta endpoint for the following AD resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta):</span></span>
>
>- [<span data-ttu-id="b9226-244">aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9226-244">application</span></span>](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-beta)
>- [<span data-ttu-id="b9226-245">orgContact</span><span class="sxs-lookup"><span data-stu-id="b9226-245">orgContact</span></span>](https://docs.microsoft.com/graph/api/resources/orgcontact?view=graph-rest-beta)
>- [<span data-ttu-id="b9226-246">device</span><span class="sxs-lookup"><span data-stu-id="b9226-246">device</span></span>](https://docs.microsoft.com/graph/api/resources/device?view=graph-rest-beta)
>- [<span data-ttu-id="b9226-247">group</span><span class="sxs-lookup"><span data-stu-id="b9226-247">group</span></span>](https://docs.microsoft.com/graph/api/resources/group?view=graph-rest-beta)
>- [<span data-ttu-id="b9226-248">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="b9226-248">servicePrincipal</span></span>](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-beta)
>- [<span data-ttu-id="b9226-249">user</span><span class="sxs-lookup"><span data-stu-id="b9226-249">user</span></span>](https://docs.microsoft.com/graph/api/resources/user?view=graph-rest-beta)
>
> <span data-ttu-id="b9226-250">Para usar o `$orderby` e o `$filter` em conjunto, você precisa:</span><span class="sxs-lookup"><span data-stu-id="b9226-250">To use `$orderby` and `$filter` together, you need to:</span></span>
>
> - <span data-ttu-id="b9226-251">Adicionar `$count=true` aos parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="b9226-251">Add `$count=true` to the query parameters</span></span>
> - <span data-ttu-id="b9226-252">Adicionar `ConsistencyLevel: eventual` ao cabeçalho de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9226-252">Add `ConsistencyLevel: eventual` request header</span></span>
>
> <span data-ttu-id="b9226-253">Confira [parâmetros opcionais de consulta de usuário](/graph/api/user-list?view=graph-rest-beta&tabs=http#optional-query-parameters) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="b9226-253">See [optional user query parameters](/graph/api/user-list?view=graph-rest-beta&tabs=http#optional-query-parameters) for more information.</span></span>

## <a name="search-parameter"></a><span data-ttu-id="b9226-254">parâmetro search</span><span class="sxs-lookup"><span data-stu-id="b9226-254">search parameter</span></span>

<span data-ttu-id="b9226-255">Use o parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="b9226-255">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="b9226-256">Usando $search em conjuntos de mensagens</span><span class="sxs-lookup"><span data-stu-id="b9226-256">Using $search on message collections</span></span>

<span data-ttu-id="b9226-257">Você pode pesquisar mensagens com base em um valor nas propriedades de mensagens específicas.</span><span class="sxs-lookup"><span data-stu-id="b9226-257">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="b9226-258">Os resultados da pesquisa são classificados pela data e hora em que a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="b9226-258">The results of the search are sorted by the date and time that the message was sent.</span></span> <span data-ttu-id="b9226-259">Uma solicitação de `$search` retorna até 250 resultados.</span><span class="sxs-lookup"><span data-stu-id="b9226-259">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="b9226-260">Se você realizar uma pesquisa em mensagens e especificar apenas um valor sem as propriedades de mensagens específicas, a pesquisa será realizada nas propriedades de pesquisa padrão **from**, **subject** e **body**.</span><span class="sxs-lookup"><span data-stu-id="b9226-260">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="b9226-261">O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:</span><span class="sxs-lookup"><span data-stu-id="b9226-261">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="b9226-262">[Experimentar no Explorador do Graph][search-example]</span><span class="sxs-lookup"><span data-stu-id="b9226-262">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="b9226-263">Como alternativa, você pode pesquisar mensagens especificando os nomes de propriedade da mensagem na tabela a seguir, que são reconhecidos pela sintaxe da Linguagem de Consulta de Palavra-chave (KQL).</span><span class="sxs-lookup"><span data-stu-id="b9226-263">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="b9226-264">Esses nomes de propriedades correspondem às propriedades definidas na entidade **mensagem** do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b9226-264">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="b9226-265">O Outlook e outros aplicativos do Microsoft 365 como o SharePoint são compatíveis com a sintaxe KQL, proporcionando a conveniência de um domínio de descoberta comum para seus repositórios de dados.</span><span class="sxs-lookup"><span data-stu-id="b9226-265">Outlook and other Microsoft 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="b9226-266">Propriedades de emails pesquisáveis</span><span class="sxs-lookup"><span data-stu-id="b9226-266">Searchable email property</span></span>                | <span data-ttu-id="b9226-267">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9226-267">Description</span></span> | <span data-ttu-id="b9226-268">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9226-268">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="b9226-269">**attachment**</span><span class="sxs-lookup"><span data-stu-id="b9226-269">**attachment**</span></span>           | <span data-ttu-id="b9226-270">Os nomes dos arquivos anexados a uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="b9226-270">The names of files attached to an email message.</span></span>|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| <span data-ttu-id="b9226-271">**bcc**</span><span class="sxs-lookup"><span data-stu-id="b9226-271">**bcc**</span></span>           | <span data-ttu-id="b9226-272">O campo **Cco** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="b9226-272">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| <span data-ttu-id="b9226-273">**body**</span><span class="sxs-lookup"><span data-stu-id="b9226-273">**body**</span></span>           | <span data-ttu-id="b9226-274">O corpo de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="b9226-274">The body of an email message.</span></span>|[`me/messages?$search="body:excitement"`][search-body-example]
| <span data-ttu-id="b9226-275">**cc**</span><span class="sxs-lookup"><span data-stu-id="b9226-275">**cc**</span></span>           | <span data-ttu-id="b9226-276">O campo **Cc** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="b9226-276">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| <span data-ttu-id="b9226-277">**from**</span><span class="sxs-lookup"><span data-stu-id="b9226-277">**from**</span></span>           | <span data-ttu-id="b9226-278">O remetente de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="b9226-278">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| <span data-ttu-id="b9226-279">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="b9226-279">**hasAttachment**</span></span> | <span data-ttu-id="b9226-280">Verdadeiro se uma mensagem de email contiver um anexo que não seja um anexo embutido, caso contrário, falso.</span><span class="sxs-lookup"><span data-stu-id="b9226-280">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> |[`me/messages?$search="hasAttachments:true"`][search-from-example]
| <span data-ttu-id="b9226-281">**importance**</span><span class="sxs-lookup"><span data-stu-id="b9226-281">**importance**</span></span>           | <span data-ttu-id="b9226-282">A prioridade de uma mensagem de email, que um remetente pode especificar ao enviar uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b9226-282">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="b9226-283">Os valores possíveis são `low`, `medium` ou `high`.</span><span class="sxs-lookup"><span data-stu-id="b9226-283">The possible values are `low`, `medium`, or `high`.</span></span>|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| <span data-ttu-id="b9226-284">**kind**</span><span class="sxs-lookup"><span data-stu-id="b9226-284">**kind**</span></span>           | <span data-ttu-id="b9226-285">O tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="b9226-285">The type of message.</span></span> <span data-ttu-id="b9226-286">Os valores possíveis são `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` ou `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="b9226-286">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| <span data-ttu-id="b9226-287">**participants**</span><span class="sxs-lookup"><span data-stu-id="b9226-287">**participants**</span></span>           | <span data-ttu-id="b9226-288">Os campos **de**, **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="b9226-288">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="participants:danas"`][search-part-example]
| <span data-ttu-id="b9226-289">**received**</span><span class="sxs-lookup"><span data-stu-id="b9226-289">**received**</span></span>           | <span data-ttu-id="b9226-290">A data em que uma mensagem de email foi recebida pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="b9226-290">The date that an email message was received by a recipient.</span></span>|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| <span data-ttu-id="b9226-291">**recipients**</span><span class="sxs-lookup"><span data-stu-id="b9226-291">**recipients**</span></span>           | <span data-ttu-id="b9226-292">Os campos **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="b9226-292">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| <span data-ttu-id="b9226-293">**sent**</span><span class="sxs-lookup"><span data-stu-id="b9226-293">**sent**</span></span>           | <span data-ttu-id="b9226-294">A data em que uma mensagem de email foi enviada pelo remetente.</span><span class="sxs-lookup"><span data-stu-id="b9226-294">The date that an email message was sent by the sender.</span></span>|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| <span data-ttu-id="b9226-295">**size**</span><span class="sxs-lookup"><span data-stu-id="b9226-295">**size**</span></span>           | <span data-ttu-id="b9226-296">O tamanho de um item em bytes.</span><span class="sxs-lookup"><span data-stu-id="b9226-296">The size of an item in bytes.</span></span>|[`me/messages?$search="size:1..500000"`][search-size-example]
| <span data-ttu-id="b9226-297">**subject**</span><span class="sxs-lookup"><span data-stu-id="b9226-297">**subject**</span></span>           | <span data-ttu-id="b9226-298">O texto na linha de assunto de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="b9226-298">The text in the subject line of an email message.</span></span> <span data-ttu-id="b9226-299">.</span><span class="sxs-lookup"><span data-stu-id="b9226-299">.</span></span>|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| <span data-ttu-id="b9226-300">**to**</span><span class="sxs-lookup"><span data-stu-id="b9226-300">**to**</span></span>           | <span data-ttu-id="b9226-301">O campo **para** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="b9226-301">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


<span data-ttu-id="b9226-302">Para saber mais sobre as propriedades de email pesquisáveis, KQL como a sintaxe, operadores com suporte e dicas de pesquisa, confira os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="b9226-302">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="b9226-303">[Propriedades pesquisáveis no Exchange](https://docs.microsoft.com/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span><span class="sxs-lookup"><span data-stu-id="b9226-303">[Searchable properties in Exchange](https://docs.microsoft.com/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- [<span data-ttu-id="b9226-304">Referência de sintaxe da Linguagem de Consulta de Palavra-chave (KQL)</span><span class="sxs-lookup"><span data-stu-id="b9226-304">Keyword Query Language (KQL) syntax reference</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- <span data-ttu-id="b9226-305">[Propriedades da mensagem e operadores de pesquisa para a Descoberta eletrônica In-loco no Exchange 2016](https://technet.microsoft.com/library/dn774955(v=exchg.160).aspx)</span><span class="sxs-lookup"><span data-stu-id="b9226-305">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="b9226-306">Usando $search em conjuntos de pessoas</span><span class="sxs-lookup"><span data-stu-id="b9226-306">Using $search on person collections</span></span>

<span data-ttu-id="b9226-307">Você pode usar a API de Pessoas do Microsoft Graph para recuperar as pessoas mais relevantes para um usuário.</span><span class="sxs-lookup"><span data-stu-id="b9226-307">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user.</span></span> <span data-ttu-id="b9226-308">A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="b9226-308">Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="b9226-309">A API de Pessoas é compatível com o parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="b9226-309">The People API supports the `$search` query parameter.</span></span> <span data-ttu-id="b9226-310">Uma solicitação de `$search` retorna até 250 resultados.</span><span class="sxs-lookup"><span data-stu-id="b9226-310">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="b9226-311">As pesquisas de pessoas ocorrem nas propriedades **displayName** e **emailAddress** do recurso [person](/graph/api/resources/person?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="b9226-311">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](/graph/api/resources/person?view=graph-rest-1.0) resource.</span></span>

<span data-ttu-id="b9226-312">A seguinte solicitação faz uma pesquisa por uma pessoa chamada "Clara Barbosa" nas propriedades **displayName** e **emailAddress** em todos os indivíduos no conjunto de **Pessoas** do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b9226-312">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="b9226-313">Como uma pessoa denominada "Clara Barbosa" é relevante para o usuário conectado, as informações para "Clara Barbosa" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="b9226-313">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="b9226-314">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9226-314">The following example shows the response.</span></span> 

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

<span data-ttu-id="b9226-315">Saiba mais sobre a API de Pessoas em [Obter informações sobre pessoas relevantes](./people-example.md#search-people).</span><span class="sxs-lookup"><span data-stu-id="b9226-315">To learn more about the People API, see [Get information about relevant people](./people-example.md#search-people).</span></span>  

### <a name="using-search-on-directory-object-collections"></a><span data-ttu-id="b9226-316">Como usar $search nos conjuntos de objetos do diretório</span><span class="sxs-lookup"><span data-stu-id="b9226-316">Using $search on directory object collections</span></span>

<span data-ttu-id="b9226-317">Você pode usar o parâmetro de consulta `$search` para restringir os resultados com base em um critério de pesquisa, como procurar palavras em strings de busca delimitadas por espaços, letras maiúsculas ou minúsculas e tipos de caracteres (números e caracteres especiais).</span><span class="sxs-lookup"><span data-stu-id="b9226-317">You can use the `$search` query parameter to restrict results based on a search criterion such as looking for words in strings delimited by spaces, casing, and character types (numbers and special characters).</span></span> <span data-ttu-id="b9226-318">O suporte tokenizado à pesquisa funciona apenas nos campos displayName e descrição.</span><span class="sxs-lookup"><span data-stu-id="b9226-318">The tokenized search support works only on the displayName and description fields.</span></span> <span data-ttu-id="b9226-319">Qualquer campo pode ser colocado no `$search`. Os padrão para os outros campos que não sejam **displayName** e **descrição** é o comportamento de `$filter` “startswith”.</span><span class="sxs-lookup"><span data-stu-id="b9226-319">Any field can be put in `$search`, fields other than **displayName** and **description** defaults to `$filter` startswith behavior.</span></span> <span data-ttu-id="b9226-320">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="b9226-320">For example:</span></span>

`https://graph.microsoft.com/beta/groups/?$search="displayName:OneVideo"`
 
<span data-ttu-id="b9226-321">procurar todos os grupos com nomes de exibição que se pareçam com "OneVideo".</span><span class="sxs-lookup"><span data-stu-id="b9226-321">This looks for all groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="b9226-322">O parâmetro `$search` também pode ser usado junto com o `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b9226-322">`$search` can be used together with `$filter` as well.</span></span> <span data-ttu-id="b9226-323">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="b9226-323">For example:</span></span> 
 
`https://graph.microsoft.com/beta/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"` 
 
<span data-ttu-id="b9226-324">procurar todos os grupos habilitados para email com nomes de exibição que se pareçam com "OneVideo".</span><span class="sxs-lookup"><span data-stu-id="b9226-324">This looks for all mail-enabled groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="b9226-325">Os resultados são restringidos com base em uma conjunção lógica (um “AND”) do parâmetro `$filter` e na consulta inteira no parâmetro `$search`.</span><span class="sxs-lookup"><span data-stu-id="b9226-325">The results are restricted based on a logical conjunction (an "AND") of the `$filter` and the entire query in the `$search`.</span></span> <span data-ttu-id="b9226-326">O texto da pesquisa é tokenizado com base nas letras maiúsculas ou minúsculas, mas as equiparações são executadas de maneira insensível ao fato de a letra ser maiúscula ou minúscula.</span><span class="sxs-lookup"><span data-stu-id="b9226-326">The search text is tokenized based on casing, but matches are performed in a case-insensitive manner.</span></span> <span data-ttu-id="b9226-327">Por exemplo, o termo “OneVideo” seria dividido em dois tokens de entrada, “one” e “video”, mas equiparado a propriedades insensíveis ao fato de a letra ser maiúscula ou minúscula.</span><span class="sxs-lookup"><span data-stu-id="b9226-327">For example, "OneVideo" would be split into two input tokens "one" and "video", but matches properties in insensitive to case.</span></span> 
 
 
<span data-ttu-id="b9226-328">A sintaxe da pesquisa segue as seguintes regras:</span><span class="sxs-lookup"><span data-stu-id="b9226-328">The syntax of search follows these rules:</span></span> 
 
- <span data-ttu-id="b9226-329">Formato genérico: $search="clause1" [AND | OR]  "[clauseX]".</span><span class="sxs-lookup"><span data-stu-id="b9226-329">Generic format: $search="clause1" [AND | OR]  "[clauseX]".</span></span> 
- <span data-ttu-id="b9226-330">O número de cláusulas (clause) não é limitado.</span><span class="sxs-lookup"><span data-stu-id="b9226-330">Any number of clauses is supported.</span></span> <span data-ttu-id="b9226-331">O uso de parênteses para a precedência também é suportado.</span><span class="sxs-lookup"><span data-stu-id="b9226-331">Parentheses for precedence is also supported.</span></span> 
- <span data-ttu-id="b9226-332">A sintaxe para cada cláusula é <property>:<text to search>.</span><span class="sxs-lookup"><span data-stu-id="b9226-332">The syntax for each clause is <property>:<text to search>.</span></span> 
- <span data-ttu-id="b9226-333">O nome da propriedade deve ser especificado na cláusula.</span><span class="sxs-lookup"><span data-stu-id="b9226-333">The property name must be specified in clause.</span></span> <span data-ttu-id="b9226-334">Qualquer propriedade que possa ser usada em `$filter` também pode ser usada dentro de `$search`.</span><span class="sxs-lookup"><span data-stu-id="b9226-334">Any property that can be used in `$filter` can also be used inside `$search`.</span></span> <span data-ttu-id="b9226-335">Dependendo da propriedade, o comportamento da pesquisa será "search" ou, se “search” não for suportado na propriedade, "startswith".</span><span class="sxs-lookup"><span data-stu-id="b9226-335">Depending on the property, the search behavior is either "search" or "startswith" if search is not supported on the property.</span></span> 
- <span data-ttu-id="b9226-336">Todas as partes de cláusula devem ser colocadas entre aspas duplas.</span><span class="sxs-lookup"><span data-stu-id="b9226-336">The whole clause part must be put inside double quotes.</span></span>  
- <span data-ttu-id="b9226-337">Os operadores lógicos “AND” e “OR” devem ser colocados fora das aspas duplas.</span><span class="sxs-lookup"><span data-stu-id="b9226-337">Logical operator 'AND' 'OR' must be put outside double quotes.</span></span> <span data-ttu-id="b9226-338">Devem sempre ser grafados em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="b9226-338">They must be in upper case.</span></span> 
- <span data-ttu-id="b9226-339">Considerando-se que todas as partes de cláusula precisam ser colocadas entre aspas duplas, se <text to search> contiver aspas duplas e barra invertida, as barras invertidas deverão ser usadas para escapar as aspas.</span><span class="sxs-lookup"><span data-stu-id="b9226-339">Given that the whole clause part needs to be put inside double quotes, if <text to search> contains double quote and backslash, it needs to be escaped by backslash.</span></span> <span data-ttu-id="b9226-340">Não é preciso escapar nenhum outro caractere.</span><span class="sxs-lookup"><span data-stu-id="b9226-340">No other characters need to be escaped.</span></span> 

<span data-ttu-id="b9226-341">A tabela abaixo mostra alguns exemplos.</span><span class="sxs-lookup"><span data-stu-id="b9226-341">The table below shows some examples.</span></span> 
 

| <span data-ttu-id="b9226-342">Classe de objeto</span><span class="sxs-lookup"><span data-stu-id="b9226-342">Object class</span></span> | <span data-ttu-id="b9226-343">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9226-343">Description</span></span> | <span data-ttu-id="b9226-344">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9226-344">Example</span></span> |
| ------------ | ----------- | ------- |
| <span data-ttu-id="b9226-345">Usuário</span><span class="sxs-lookup"><span data-stu-id="b9226-345">User</span></span> | <span data-ttu-id="b9226-346">O caderno de endereços exibe o nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="b9226-346">Address book display name of the user.</span></span> |  `https://graph.microsoft.com/beta/users?$search="displayName:Guthr"` |
| <span data-ttu-id="b9226-347">Usuário</span><span class="sxs-lookup"><span data-stu-id="b9226-347">User</span></span> | <span data-ttu-id="b9226-348">O caderno de endereços exibe o nome ou o email do usuário.</span><span class="sxs-lookup"><span data-stu-id="b9226-348">Address book display name or mail of the user.</span></span> | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"` |
| <span data-ttu-id="b9226-349">Grupo</span><span class="sxs-lookup"><span data-stu-id="b9226-349">Group</span></span> | <span data-ttu-id="b9226-350">O caderno de endereços exibe o nome ou a descrição de um grupo.</span><span class="sxs-lookup"><span data-stu-id="b9226-350">Address book display name or description of the group.</span></span> | `https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")` |
| <span data-ttu-id="b9226-351">Grupo</span><span class="sxs-lookup"><span data-stu-id="b9226-351">Group</span></span> | <span data-ttu-id="b9226-352">O caderno de endereços exibe o nome em um grupo habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="b9226-352">Address book display name on a mail enabled group.</span></span> | `https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"` |

<span data-ttu-id="b9226-353">Ambas as entradas de string fornecidas em `$search`, assim como as propriedades pesquisáveis indicadas acima, são divididas em partes por meio de espaços, da variação entre letras maiúsculas e minúsculas e de tipos de caracteres (números e caracteres especiais).</span><span class="sxs-lookup"><span data-stu-id="b9226-353">Both the string inputs you provide in `$search`, as well as the searchable properties indicated above, are split up into parts by spaces, different casing, and character types (numbers and special characters).</span></span>

## <a name="select-parameter"></a><span data-ttu-id="b9226-354">parâmetro select</span><span class="sxs-lookup"><span data-stu-id="b9226-354">select parameter</span></span>

<span data-ttu-id="b9226-355">Use o parâmetro de consulta `$select` para retornar um conjunto de propriedades diferente do padrão definido para um recurso individual ou um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="b9226-355">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="b9226-356">Com $select, você pode especificar um subconjunto ou um superconjunto das propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="b9226-356">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="b9226-357">Por exemplo, ao recuperar as mensagens do usuário conectado, você pode especificar que somente as propriedades **from** e **subject** sejam retornadas:</span><span class="sxs-lookup"><span data-stu-id="b9226-357">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="b9226-358">[Experimentar no Explorador do Graph][select-example]</span><span class="sxs-lookup"><span data-stu-id="b9226-358">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="b9226-359">**Importante:** Em geral, recomendamos que você use `$select` para limitar as propriedades retornadas por uma consulta àqueles exigidas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9226-359">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="b9226-360">Isso se aplica particularmente a consultas com o potencial de retornar um conjunto de resultados amplo.</span><span class="sxs-lookup"><span data-stu-id="b9226-360">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="b9226-361">Limitar as propriedades retornadas em cada linha reduzirá a carga de rede e ajudará a melhorar o desempenho do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9226-361">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="b9226-p136">No `v1.0`, alguns recursos do Azure AD que derivam de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), como [usuário](/graph/api/resources/user?view=graph-rest-1.0) e [grupo](/graph/api/resources/group?view=graph-rest-1.0), retornam um subconjunto limitado padrão de propriedades em leituras. Para esses recursos, você deve usar `$select` para retornar propriedades fora do conjunto padrão.</span><span class="sxs-lookup"><span data-stu-id="b9226-p136">In `v1.0`, some Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), like [user](/graph/api/resources/user?view=graph-rest-1.0) and [group](/graph/api/resources/group?view=graph-rest-1.0), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="b9226-364">parâmetro skip</span><span class="sxs-lookup"><span data-stu-id="b9226-364">skip parameter</span></span>

<span data-ttu-id="b9226-p137">Use o parâmetro de consulta `$skip` para definir o número de itens para ignorar no início de um conjunto. Por exemplo, a solicitação a seguir retorna eventos para o usuário classificadas por data de criação, começando com o evento 21 no conjunto:</span><span class="sxs-lookup"><span data-stu-id="b9226-p137">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="b9226-367">[Experimentar no Explorador do Graph][skip-example]</span><span class="sxs-lookup"><span data-stu-id="b9226-367">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="b9226-368">**Observação:** algumas APIs do Microsoft Graph, como Email e Calendário do Outlook (**message**, **event** e **calendar**), usam `$skip` para implementar a paginação.</span><span class="sxs-lookup"><span data-stu-id="b9226-368">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="b9226-369">Quando os resultados de uma consulta ocuparem várias páginas, essas APIs retornarão uma propriedade `@odata:nextLink` com uma URL que contém um parâmetro `$skip`.</span><span class="sxs-lookup"><span data-stu-id="b9226-369">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="b9226-370">Você pode usar essa URL para retornar a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="b9226-370">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="b9226-371">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="b9226-371">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="b9226-372">parâmetro skipToken</span><span class="sxs-lookup"><span data-stu-id="b9226-372">skipToken parameter</span></span>

<span data-ttu-id="b9226-p139">Algumas solicitações retornam várias páginas de dados devido à paginação do lado do servidor ou devido ao uso do parâmetro [`$top`](#top-parameter) para limitar o tamanho da página da resposta. Muitas APIs do Microsoft Graph usam o parâmetro de consulta `skipToken` para fazer referência a páginas subsequentes do resultado. O parâmetro `$skiptoken` contém um token opaco que faz referência à próxima página de resultados e é retornado na URL fornecida na propriedade `@odata.nextLink` na resposta. Para saber mais, confira [paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="b9226-p139">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="b9226-377">parâmetro top</span><span class="sxs-lookup"><span data-stu-id="b9226-377">top parameter</span></span>

<span data-ttu-id="b9226-378">Use o parâmetro de consulta `$top` para especificar o tamanho de página do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="b9226-378">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="b9226-379">Se restarem mais itens no conjunto de resultados, o corpo da resposta conterá um parâmetro `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="b9226-379">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="b9226-380">Esse parâmetro contém uma URL que você pode usar para obter a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="b9226-380">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="b9226-381">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="b9226-381">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="b9226-382">O $top aceita um valor mínimo de 1 e um valor máximo de 999 (inclusive).</span><span class="sxs-lookup"><span data-stu-id="b9226-382">$top accepts a minimum value of 1 and a maximum value of 999 (inclusive).</span></span>  

<span data-ttu-id="b9226-383">Por exemplo, a solicitação a seguir retorna as primeiras cinco mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="b9226-383">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="b9226-384">[Experimentar no Explorador do Graph][top-example]</span><span class="sxs-lookup"><span data-stu-id="b9226-384">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="b9226-385">Tratamento de erro para parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="b9226-385">Error handling for query parameters</span></span>

<span data-ttu-id="b9226-p141">Algumas solicitações retornarão uma mensagem de erro se não houver suporte para um parâmetro de consulta especificado. Por exemplo, você não pode usar `$expand` na relação `user/photo`.</span><span class="sxs-lookup"><span data-stu-id="b9226-p141">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="b9226-388">No entanto, é importante observar que os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente.</span><span class="sxs-lookup"><span data-stu-id="b9226-388">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="b9226-389">Isso pode ser verdadeiro para parâmetros de consulta sem suporte, bem como para combinações de parâmetros de consulta sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9226-389">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="b9226-390">Nesses casos, você deve examinar os dados retornados pela solicitação para determinar se os parâmetros de consulta que especificou tiveram o efeito desejado.</span><span class="sxs-lookup"><span data-stu-id="b9226-390">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

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



## <a name="see-also"></a><span data-ttu-id="b9226-391">Confira também</span><span class="sxs-lookup"><span data-stu-id="b9226-391">See also</span></span>

- [<span data-ttu-id="b9226-392">Limitações de parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="b9226-392">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)
