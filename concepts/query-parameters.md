---
title: Usar parâmetros de consulta para personalizar respostas
description: O Microsoft Graph fornece parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta.
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 1bfa039dc133ccd215a3f43780ddb1523e8dafdc
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030254"
---
# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="5f931-103">Usar parâmetros de consulta para personalizar respostas</span><span class="sxs-lookup"><span data-stu-id="5f931-103">Use query parameters to customize responses</span></span>

<span data-ttu-id="5f931-104">O Microsoft Graph fornece suporte a parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="5f931-104">Microsoft Graph supports optional query parameters that you can use to specify and control the amount of data returned in a response.</span></span> <span data-ttu-id="5f931-105">O suporte para os parâmetros de consulta exatos variam de uma operação de API para outra e, dependendo da API, podem diferir entre os pontos de extremidade v1.0 e beta.</span><span class="sxs-lookup"><span data-stu-id="5f931-105">The support for the exact query parameters varies from one API operation to another, and depending on the API, can differ between the v1.0 and beta endpoints.</span></span>

> [!TIP] 
> <span data-ttu-id="5f931-106">No ponto de extremidade beta, o prefixo `$` é opcional.</span><span class="sxs-lookup"><span data-stu-id="5f931-106">On the beta endpoint, the `$` prefix is optional.</span></span> <span data-ttu-id="5f931-107">Por exemplo, em vez de `$filter`, você pode usar `filter`.</span><span class="sxs-lookup"><span data-stu-id="5f931-107">For example, instead of `$filter`, you can use `filter`.</span></span> <span data-ttu-id="5f931-108">No ponto de extremidade v1, o prefixo `$` é opcional apenas para um subconjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="5f931-108">On the v1 endpoint, the `$` prefix is optional for only a subset of APIs.</span></span> <span data-ttu-id="5f931-109">Para simplificar, inclua sempre `$` se estiver usando o ponto de extremidade v1.</span><span class="sxs-lookup"><span data-stu-id="5f931-109">For simplicity, always include `$` if using the v1 endpoint.</span></span>

<span data-ttu-id="5f931-110">Os parâmetros de consulta podem ser opções de consulta de sistema OData ou outros parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="5f931-110">Query parameters can be OData system query options or other query parameters.</span></span> 

> [!VIDEO https://www.youtube-nocookie.com/embed/7BuFv3yETi4]

## <a name="odata-system-query-options"></a><span data-ttu-id="5f931-111">Opções de consulta de sistema OData</span><span class="sxs-lookup"><span data-stu-id="5f931-111">OData system query options</span></span>
<span data-ttu-id="5f931-112">Uma operação de API do Microsoft Graph pode oferecer suporte a uma ou mais das seguintes opções de consulta de sistema OData.</span><span class="sxs-lookup"><span data-stu-id="5f931-112">A Microsoft Graph API operation might support one or more of the following OData system query options.</span></span> <span data-ttu-id="5f931-113">Essas opções de consulta são compatíveis com a [linguagem de consulta OData V4][odata-query].</span><span class="sxs-lookup"><span data-stu-id="5f931-113">These query options are compatible with the [OData V4 query language][odata-query].</span></span>

><span data-ttu-id="5f931-114">**Observação:** o OData 4.0 oferece suporte às opções de consulta do sistema apenas em operações GET.</span><span class="sxs-lookup"><span data-stu-id="5f931-114">**Note:** OData 4.0 supports system query options in only GET operations.</span></span>

<span data-ttu-id="5f931-115">Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="5f931-115">Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="5f931-116">Nome</span><span class="sxs-lookup"><span data-stu-id="5f931-116">Name</span></span>                     | <span data-ttu-id="5f931-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f931-117">Description</span></span> | <span data-ttu-id="5f931-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f931-118">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="5f931-119">$count</span><span class="sxs-lookup"><span data-stu-id="5f931-119">$count</span></span>](#count-parameter)         | <span data-ttu-id="5f931-120">Recupera a contagem total de recursos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="5f931-120">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="5f931-121">$expand</span><span class="sxs-lookup"><span data-stu-id="5f931-121">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="5f931-122">Recupera os recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="5f931-122">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="5f931-123">$filter</span><span class="sxs-lookup"><span data-stu-id="5f931-123">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="5f931-124">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="5f931-124">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="5f931-125">$format</span><span class="sxs-lookup"><span data-stu-id="5f931-125">$format</span></span>](#format-parameter)       | <span data-ttu-id="5f931-126">Retorna os resultados no formato de mídia especificado.</span><span class="sxs-lookup"><span data-stu-id="5f931-126">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="5f931-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="5f931-127">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="5f931-128">Ordena os resultados.</span><span class="sxs-lookup"><span data-stu-id="5f931-128">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="5f931-129">$search</span><span class="sxs-lookup"><span data-stu-id="5f931-129">$search</span></span>](#search-parameter)       | <span data-ttu-id="5f931-130">Retorna os resultados com base nos critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="5f931-130">Returns results based on search criteria.</span></span> |[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="5f931-131">$select</span><span class="sxs-lookup"><span data-stu-id="5f931-131">$select</span></span>](#select-parameter)       | <span data-ttu-id="5f931-132">Filtra as propriedades (colunas).</span><span class="sxs-lookup"><span data-stu-id="5f931-132">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="5f931-133">$skip</span><span class="sxs-lookup"><span data-stu-id="5f931-133">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="5f931-p104">Índices em um conjunto de resultados. Também usado por algumas APIs para implementar a paginação e pode ser usado com `$top` para paginar resultados manualmente.</span><span class="sxs-lookup"><span data-stu-id="5f931-p104">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="5f931-136">$top</span><span class="sxs-lookup"><span data-stu-id="5f931-136">$top</span></span>](#top-parameter)             | <span data-ttu-id="5f931-137">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="5f931-137">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a><span data-ttu-id="5f931-138">Outros parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="5f931-138">Other query parameters</span></span>

| <span data-ttu-id="5f931-139">Nome</span><span class="sxs-lookup"><span data-stu-id="5f931-139">Name</span></span>                     | <span data-ttu-id="5f931-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f931-140">Description</span></span> | <span data-ttu-id="5f931-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f931-141">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="5f931-142">$skipToken</span><span class="sxs-lookup"><span data-stu-id="5f931-142">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="5f931-p105">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas. (Algumas APIs usam `$skip` em vez disso.)</span><span class="sxs-lookup"><span data-stu-id="5f931-p105">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a><span data-ttu-id="5f931-145">Outros recursos de URL OData</span><span class="sxs-lookup"><span data-stu-id="5f931-145">Other OData URL capabilities</span></span>

<span data-ttu-id="5f931-146">Os seguintes recursos OData 4.0 são segmentos de URL, não parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="5f931-146">The following OData 4.0 capabilities are URL segments, not query parameters.</span></span>

| <span data-ttu-id="5f931-147">Nome</span><span class="sxs-lookup"><span data-stu-id="5f931-147">Name</span></span>                     | <span data-ttu-id="5f931-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f931-148">Description</span></span> | <span data-ttu-id="5f931-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f931-149">Example</span></span> 
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="5f931-150">$count</span><span class="sxs-lookup"><span data-stu-id="5f931-150">$count</span></span>](/graph/api/user-list#example-3-get-only-a-count-of-users)| <span data-ttu-id="5f931-151">Recupera o total inteiro da coleção.</span><span class="sxs-lookup"><span data-stu-id="5f931-151">Retrieves the integer total of the collection.</span></span> | `GET /users/$count` <br> `GET /groups/{id}/members/$count`|
| [<span data-ttu-id="5f931-152">$ref</span><span class="sxs-lookup"><span data-stu-id="5f931-152">$ref</span></span>](/graph/api/group-post-members) | <span data-ttu-id="5f931-153">Atualiza a associação de entidades a uma coleção.</span><span class="sxs-lookup"><span data-stu-id="5f931-153">Updates entities membership to a collection.</span></span> | `POST /groups/{id}/members/$ref` |
| [<span data-ttu-id="5f931-154">$value</span><span class="sxs-lookup"><span data-stu-id="5f931-154">$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="5f931-155">Recupera ou atualiza o valor binário de um item.</span><span class="sxs-lookup"><span data-stu-id="5f931-155">Retrieves or updates the binary value of an item.</span></span> | `GET /me/photo/$value` |

## <a name="encoding-query-parameters"></a><span data-ttu-id="5f931-156">Codificação de parâmetros da consulta</span><span class="sxs-lookup"><span data-stu-id="5f931-156">Encoding query parameters</span></span>

<span data-ttu-id="5f931-157">Os valores dos parâmetros da consulta devem ser codificados por porcentagem.</span><span class="sxs-lookup"><span data-stu-id="5f931-157">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="5f931-158">Muitas ferramentas, navegadores e clientes HTTP (como o [Explorador do Graph][graph-explorer]) ajudarão você com isso.</span><span class="sxs-lookup"><span data-stu-id="5f931-158">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="5f931-159">Se uma consulta está falhando, uma causa possível é a falha na codificação adequada dos valores dos parâmetros da consulta.</span><span class="sxs-lookup"><span data-stu-id="5f931-159">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="5f931-160">Uma URL descodificada é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="5f931-160">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="5f931-161">Uma URL codificada adequadamente é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="5f931-161">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

### <a name="escaping-single-quotes"></a><span data-ttu-id="5f931-162">Escape de aspas simples</span><span class="sxs-lookup"><span data-stu-id="5f931-162">Escaping single quotes</span></span>

<span data-ttu-id="5f931-163">Para pedidos que usem aspas simples, se os valores de qualquer parâmetro também contém aspas, elas devem ter escape duplo. Caso contrário, a solicitação falhará devido a sintaxe inválida.</span><span class="sxs-lookup"><span data-stu-id="5f931-163">For requests that use single quotes, if any parameter values also contain single quotes, those must be double escaped; otherwise, the request will fail due to invalid syntax.</span></span> <span data-ttu-id="5f931-164">No exemplo, o valor de cadeia de caracteres `let''s meet for lunch?` tem o escape de aspas simples.</span><span class="sxs-lookup"><span data-stu-id="5f931-164">In the example, the string value `let''s meet for lunch?` has the single quote escaped.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a><span data-ttu-id="5f931-165">parâmetro count</span><span class="sxs-lookup"><span data-stu-id="5f931-165">count parameter</span></span>

<span data-ttu-id="5f931-166">Use o parâmetro de consulta `$count` para incluir uma contagem do número total de itens em um conjunto, juntamente com a página de valores de dados retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5f931-166">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span>

> [!NOTE]
> <span data-ttu-id="5f931-167">`$count` também pode ser usado como um [segmento de URL](#other-odata-url-capabilities) para recuperar o total inteiro da coleção.</span><span class="sxs-lookup"><span data-stu-id="5f931-167">`$count` can also be used as a [URL segment](#other-odata-url-capabilities) to retrieve the integer total of the collection.</span></span> <span data-ttu-id="5f931-168">Em recursos que derivam de [directoryObject](/graph/api/resources/directoryobject), ele só tem suporte em uma [consulta avançada](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="5f931-168">On resources that derive from [directoryObject](/graph/api/resources/directoryobject), is it only supported in an [advanced query](/graph/aad-advanced-queries).</span></span> <span data-ttu-id="5f931-169">Consulte [Recursos avançados de consulta em objetos de diretório do Microsoft Azure Active Directory](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="5f931-169">See [Advanced query capabilities in Azure AD directory objects](/graph/aad-advanced-queries).</span></span>
>
> <span data-ttu-id="5f931-170">Não há suporte para o uso de `$count` em locatários do Microsoft Azure Active Directory B2C.</span><span class="sxs-lookup"><span data-stu-id="5f931-170">Use of `$count` is not supported in Azure AD B2C tenants.</span></span>

<span data-ttu-id="5f931-171">Por exemplo, a solicitação a seguir retornará tanto o conjunto **contato** do usuário atual quanto o número de itens no conjunto **contato** na propriedade `@odata.count`.</span><span class="sxs-lookup"><span data-stu-id="5f931-171">For example, the following request returns both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="5f931-172">Experimente o Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="5f931-172">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)

<span data-ttu-id="5f931-173">O parâmetro de consulta `$count` tem suporte para essas coleções de recursos e suas relações que derivam de [directoryObject](/graph/api/resources/directoryobject) e somente em [consultas avançadas](/graph/filter-directory-objects):</span><span class="sxs-lookup"><span data-stu-id="5f931-173">The `$count` query parameter is supported for these collections of resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject) and only in [advanced queries](/graph/filter-directory-objects):</span></span>
- [<span data-ttu-id="5f931-174">aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f931-174">application</span></span>](/graph/api/resources/application)
- [<span data-ttu-id="5f931-175">orgContact</span><span class="sxs-lookup"><span data-stu-id="5f931-175">orgContact</span></span>](/graph/api/resources/orgcontact)
- [<span data-ttu-id="5f931-176">device</span><span class="sxs-lookup"><span data-stu-id="5f931-176">device</span></span>](/graph/api/resources/device)
- [<span data-ttu-id="5f931-177">group</span><span class="sxs-lookup"><span data-stu-id="5f931-177">group</span></span>](/graph/api/resources/group)
- [<span data-ttu-id="5f931-178">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="5f931-178">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal)
- [<span data-ttu-id="5f931-179">usuários</span><span class="sxs-lookup"><span data-stu-id="5f931-179">users</span></span>](/graph/api/resources/user)

## <a name="expand-parameter"></a><span data-ttu-id="5f931-180">parâmetro expand</span><span class="sxs-lookup"><span data-stu-id="5f931-180">expand parameter</span></span>

<span data-ttu-id="5f931-181">Muitos recursos do Microsoft Graph expõem as propriedades declaradas do recurso, bem como as relações delas com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="5f931-181">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="5f931-182">Essas relações também são chamadas de propriedades de referência ou propriedades de navegação e podem fazer referência a um único recurso ou a um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="5f931-182">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="5f931-183">Por exemplo, as pastas de email, gerente e subordinados diretos de um usuário são todas expostas como relações.</span><span class="sxs-lookup"><span data-stu-id="5f931-183">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="5f931-p110">Normalmente, você pode consultar as propriedades de um recurso ou uma de suas relações em uma única solicitação, mas não ambas. Você pode usar o parâmetro de cadeia de caracteres de consulta `$expand` para incluir o recurso expandido ou o conjunto referenciado por uma única relação (propriedade de navegação) nos resultados.</span><span class="sxs-lookup"><span data-stu-id="5f931-p110">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="5f931-186">O seguinte exemplo obtém informações de unidade raiz juntamente com os itens filho de nível superior em uma unidade:</span><span class="sxs-lookup"><span data-stu-id="5f931-186">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="5f931-187">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="5f931-187">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="5f931-p111">Com alguns conjuntos de recursos, você também pode especificar as propriedades a serem retornadas nos recursos expandidos adicionando um parâmetro `$select`. O exemplo a seguir executa a mesma consulta que o exemplo anterior, mas usa uma instrução [`$select`](#select-parameter) para limitar as propriedades retornadas para os itens filho expandidos para as propriedades **id** e **name**.</span><span class="sxs-lookup"><span data-stu-id="5f931-p111">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="5f931-190">[Experimentar no Explorador do Graph][expand-example]</span><span class="sxs-lookup"><span data-stu-id="5f931-190">[Try in Graph Explorer][expand-example]</span></span>

> [!NOTE]
> <span data-ttu-id="5f931-191">Nem todas as relações e recursos dão suporte ao parâmetro de consulta `$expand`.</span><span class="sxs-lookup"><span data-stu-id="5f931-191">Not all relationships and resources support the `$expand` query parameter.</span></span> <span data-ttu-id="5f931-192">Por exemplo, você pode expandir as relações **directReports**, **manager** e **memberOf** em um usuário, mas não pode expandir seus relacionamentos de **eventos**, **mensagens** ou **foto**.</span><span class="sxs-lookup"><span data-stu-id="5f931-192">For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships.</span></span> <span data-ttu-id="5f931-193">Nem todos os recursos ou relações dão suporte ao uso de `$select` em itens expandidos.</span><span class="sxs-lookup"><span data-stu-id="5f931-193">Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="5f931-194">Com os recursos do Microsoft Azure Active Directory que derivam de [directoryObject](/graph/api/resources/directoryobject), como [usuário](/graph/api/resources/user) e [grupo](/graph/api/resources/group), o `$expand` normalmente retorna um máximo de 20 itens para a relação expandida e não tem [@odata.nextLink](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="5f931-194">With Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject), like [user](/graph/api/resources/user) and [group](/graph/api/resources/group), `$expand` typically returns a maximum of 20 items for the expanded relationship and has no [@odata.nextLink](./paging.md).</span></span> <span data-ttu-id="5f931-195">Veja mais [problemas conhecidos](known-issues.md#query-parameter-limitations).</span><span class="sxs-lookup"><span data-stu-id="5f931-195">See more [known issues](known-issues.md#query-parameter-limitations).</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="5f931-196">parâmetro filter</span><span class="sxs-lookup"><span data-stu-id="5f931-196">filter parameter</span></span>

<span data-ttu-id="5f931-197">Use o parâmetro de consulta `$filter` para recuperar apenas um subconjunto de um conjunto.</span><span class="sxs-lookup"><span data-stu-id="5f931-197">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> <span data-ttu-id="5f931-198">O parâmetro de consulta `$filter` também pode ser usado para recuperar relações como members, memberOf, transitiveMembers e transitiveMemberOf.</span><span class="sxs-lookup"><span data-stu-id="5f931-198">The `$filter` query parameter can also be used to retrieve relationships like members, memberOf, transitiveMembers, and transitiveMemberOf.</span></span> <span data-ttu-id="5f931-199">Por exemplo, obter todos os grupos de segurança dos quais sou membro.</span><span class="sxs-lookup"><span data-stu-id="5f931-199">For example, get all the security groups I'm a member of.</span></span>

<span data-ttu-id="5f931-200">O exemplo a seguir pode ser usado para encontrar usuários cujo nome de exibição começa com a letra “J’: use `startsWith`.</span><span class="sxs-lookup"><span data-stu-id="5f931-200">The following example can be used to find users whose display name starts with the letter 'J', use `startsWith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startsWith(displayName,'J')
```

<span data-ttu-id="5f931-201">[Experimentar no Explorador do Graph][filter-example]</span><span class="sxs-lookup"><span data-stu-id="5f931-201">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="5f931-202">O suporte para operadores `$filter` varia entre as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5f931-202">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="5f931-203">Os seguintes operadores lógicos geralmente são suportados:</span><span class="sxs-lookup"><span data-stu-id="5f931-203">The following logical operators are generally supported:</span></span>

- <span data-ttu-id="5f931-204">é igual a `eq` / não é igual a `ne`</span><span class="sxs-lookup"><span data-stu-id="5f931-204">equals `eq` / not equals `ne`</span></span>
- <span data-ttu-id="5f931-205">menor que `lt` / maior que `gt`</span><span class="sxs-lookup"><span data-stu-id="5f931-205">less than `lt` / greater than `gt`</span></span>
- <span data-ttu-id="5f931-206">menor que ou igual a `le` / maior que ou igual a `ge`</span><span class="sxs-lookup"><span data-stu-id="5f931-206">less than or equal to `le` / greater than or equal to `ge`</span></span>
- <span data-ttu-id="5f931-207">e `and` / ou `or`</span><span class="sxs-lookup"><span data-stu-id="5f931-207">and `and` / or `or`</span></span>
- <span data-ttu-id="5f931-208">em `in`</span><span class="sxs-lookup"><span data-stu-id="5f931-208">in `in`</span></span>
- <span data-ttu-id="5f931-209">Negação `not`</span><span class="sxs-lookup"><span data-stu-id="5f931-209">Negation `not`</span></span>
- <span data-ttu-id="5f931-210">operador lambda qualquer `any`</span><span class="sxs-lookup"><span data-stu-id="5f931-210">lambda operator any `any`</span></span>
- <span data-ttu-id="5f931-211">operador lambda todos `all`</span><span class="sxs-lookup"><span data-stu-id="5f931-211">lambda operator all `all`</span></span>
- <span data-ttu-id="5f931-212">Começa com`startsWith`</span><span class="sxs-lookup"><span data-stu-id="5f931-212">Starts with `startsWith`</span></span>
- <span data-ttu-id="5f931-213">Termina com `endsWith` (somente em [consultas avançadas](/graph/aad-advanced-queries))</span><span class="sxs-lookup"><span data-stu-id="5f931-213">Ends with `endsWith` (Only in [advanced queries](/graph/aad-advanced-queries))</span></span>
- <span data-ttu-id="5f931-214">Contém `contains`</span><span class="sxs-lookup"><span data-stu-id="5f931-214">Contains `contains`</span></span>

> <span data-ttu-id="5f931-215">**Observação:** Suporte para esses operadores varia de acordo com a entidade e algumas propriedades dão suporte a `$filter` somente em [consultas avançadas](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="5f931-215">**Note:** Support for these operators varies by entity and some properties support `$filter` only in [advanced queries](/graph/aad-advanced-queries).</span></span> <span data-ttu-id="5f931-216">Confira a documentação específica da entidade para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="5f931-216">See the specific entity documentation for details.</span></span>

### <a name="filter-using-lambda-operators"></a><span data-ttu-id="5f931-217">Filtrar usando operadores lambda</span><span class="sxs-lookup"><span data-stu-id="5f931-217">Filter using lambda operators</span></span>

<span data-ttu-id="5f931-218">OData define os operadores `any` e `all` para avaliar correspondências em propriedades com valores múltiplos, ou seja, uma coleção de valores primitivos, como tipos de **cadeia de caracteres** ou coleção de entidades.</span><span class="sxs-lookup"><span data-stu-id="5f931-218">OData defines the `any` and `all` operators to evaluate matches on multi-valued properties, that is, either collection of primitive values such as **String** types or collection of entities.</span></span>

<span data-ttu-id="5f931-219">O operador `any` aplica iterativamente uma expressão booliana a cada membro de uma coleção e retorna `true` se a expressão for `true` para *qualquer membro* da coleção, caso contrário, retornará `false`.</span><span class="sxs-lookup"><span data-stu-id="5f931-219">The `any` operator iteratively applies a Boolean expression to each member of a collection and returns `true` if the expression is `true` for *any member* of the collection, otherwise it returns `false`.</span></span> <span data-ttu-id="5f931-220">A seguir está a sintaxe do operador `any`:</span><span class="sxs-lookup"><span data-stu-id="5f931-220">The following is the syntax of the `any` operator:</span></span>

```http
$filter=param/any(var:var/subparam eq 'value-to-match')
```

<span data-ttu-id="5f931-221">Em que</span><span class="sxs-lookup"><span data-stu-id="5f931-221">Where</span></span>
+ <span data-ttu-id="5f931-222">*param* é a propriedade que contém uma coleção de valores ou uma coleção de entidades.</span><span class="sxs-lookup"><span data-stu-id="5f931-222">*param* is the property that contains a collection of values or a collection of entities.</span></span>
+ <span data-ttu-id="5f931-223">*var:var* é uma variável de intervalo que contém o elemento atual da coleção durante a iteração.</span><span class="sxs-lookup"><span data-stu-id="5f931-223">*var:var* is a range variable that holds the current element of the collection during iteration.</span></span> <span data-ttu-id="5f931-224">Essa variável pode ser nomeada praticamente qualquer coisa, por exemplo, *adele:adele* ou *x:x*.</span><span class="sxs-lookup"><span data-stu-id="5f931-224">This variable can be named almost anything, for example, *adele:adele* or *x:x*.</span></span>
+ <span data-ttu-id="5f931-225">*subparam* é necessário quando a consulta se aplica a uma coleção de entidades.</span><span class="sxs-lookup"><span data-stu-id="5f931-225">*subparam* is required when the query applies to a collection of entities.</span></span> <span data-ttu-id="5f931-226">Ele representa a propriedade do tipo complexo cujo valor estamos correspondendo.</span><span class="sxs-lookup"><span data-stu-id="5f931-226">It represents the property of the complex type whose value we are matching.</span></span>
+ <span data-ttu-id="5f931-227">*value-to-match* representa o membro da coleção com o qual estamos correspondendo.</span><span class="sxs-lookup"><span data-stu-id="5f931-227">*value-to-match* represents the member of the collection against which we are matching.</span></span>

<span data-ttu-id="5f931-228">Por exemplo, a propriedade **assignedLicenses** do recurso de usuários pode conter uma coleção de objetos **assignedLicense**, um tipo complexo com duas propriedades, **skuId** e **disabledPlans**.</span><span class="sxs-lookup"><span data-stu-id="5f931-228">For example the **assignedLicenses** property of the users resource can contain a collection of **assignedLicense** objects, a complex type with two properties, **skuId** and **disabledPlans**.</span></span> <span data-ttu-id="5f931-229">A consulta a seguir recupera apenas os usuários com uma licença atribuída identificada pelo **skuId** `184efa21-98c3-4e5d-95ab-d07053a96e67`.</span><span class="sxs-lookup"><span data-stu-id="5f931-229">The following query retrieves only users with an assigned license identified by the **skuId** `184efa21-98c3-4e5d-95ab-d07053a96e67`.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=assignedLicenses/any(s:s/skuId eq 184efa21-98c3-4e5d-95ab-d07053a96e67)
```

<span data-ttu-id="5f931-230">A propriedade **imAddresses** do recurso de usuários pode conter uma coleção de tipos primitivos de **cadeia de caracteres**.</span><span class="sxs-lookup"><span data-stu-id="5f931-230">The **imAddresses** property of the users resource can contain a collection of primitive type **string**.</span></span> <span data-ttu-id="5f931-231">A consulta a seguir recupera apenas os usuários com um imAddress de `admin@contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="5f931-231">The following query retrieves only users with an imAddress of `admin@contoso.com`.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=imAddresses/any(s:s eq 'admin@contoso.com')
```

<span data-ttu-id="5f931-232">Para negar o resultado da expressão dentro da cláusula `any`, use o operador `NOT`, não o operador `ne`.</span><span class="sxs-lookup"><span data-stu-id="5f931-232">To negate the result of the expression inside the `any` clause, use the `NOT` operator, not the `ne` operator.</span></span> <span data-ttu-id="5f931-233">Por exemplo, a consulta a seguir recupera apenas os usuários que não receberam o **imAddress** de `admin@contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="5f931-233">For example, the following query retrieves only users who are not assigned the **imAddress** of `admin@contoso.com`.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$filter=NOT imAddresses/any(s:s eq 'admin@m365x435773.onmicrosoft.com')&$count=true
```

<span data-ttu-id="5f931-234">O operador `all` aplica uma expressão booliana a cada membro de uma coleção e retorna `true` se a expressão for `true` para *todos os membros* da coleção, caso contrário, retornará `false`.</span><span class="sxs-lookup"><span data-stu-id="5f931-234">The `all` operator applies a Boolean expression to each member of a collection and returns `true` if the expression is `true` for *all members* of the collection, otherwise it returns `false`.</span></span> <span data-ttu-id="5f931-235">Não há suporte para ele em nenhuma propriedade.</span><span class="sxs-lookup"><span data-stu-id="5f931-235">It is not supported by any property.</span></span>

### <a name="examples-using-the-filter-query-operator"></a><span data-ttu-id="5f931-236">Exemplos usando o operador de consulta de filtro</span><span class="sxs-lookup"><span data-stu-id="5f931-236">Examples using the filter query operator</span></span>

<span data-ttu-id="5f931-237">A tabela a seguir mostra alguns exemplos que usam o parâmetro de consulta `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5f931-237">The following table shows some examples that use the `$filter` query parameter.</span></span> <span data-ttu-id="5f931-238">Para obter mais detalhes sobre a sintaxe `$filter`, confira o [protocolo OData][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="5f931-238">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>

> <span data-ttu-id="5f931-239">**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="5f931-239">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="5f931-240">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f931-240">Description</span></span> | <span data-ttu-id="5f931-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f931-241">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="5f931-242">Pesquisar por usuários com o nome Clara entre várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="5f931-242">Get all users with the name Mary across multiple properties.</span></span> | <span data-ttu-id="5f931-243">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) `../users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`</span><span class="sxs-lookup"><span data-stu-id="5f931-243">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) `../users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`</span></span> |
| <span data-ttu-id="5f931-244">Obter todos os usuários com o domínio de email igual a 'hotmail.com'</span><span class="sxs-lookup"><span data-stu-id="5f931-244">Get all users with mail domain equal to 'hotmail.com'</span></span> | <span data-ttu-id="5f931-245">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@hotmail.com')`.</span><span class="sxs-lookup"><span data-stu-id="5f931-245">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@hotmail.com')`.</span></span> <span data-ttu-id="5f931-246">Esta é uma [consulta avançada](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="5f931-246">This is an [advanced query](/graph/aad-advanced-queries).</span></span> |
| <span data-ttu-id="5f931-247">Obter todos os eventos do usuário conectado que começaram após 01/07/2017.</span><span class="sxs-lookup"><span data-stu-id="5f931-247">Get all the signed-in user's events that start after 7/1/2017.</span></span> | <span data-ttu-id="5f931-248">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) `../me/events?$filter=start/dateTime ge '2017-07-01T08:00'`</span><span class="sxs-lookup"><span data-stu-id="5f931-248">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) `../me/events?$filter=start/dateTime ge '2017-07-01T08:00'`</span></span> |
| <span data-ttu-id="5f931-249">Obter todos os emails de um endereço específico recebidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5f931-249">Get all emails from a specific address received by the signed-in user.</span></span> | <span data-ttu-id="5f931-250">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) `../me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`</span><span class="sxs-lookup"><span data-stu-id="5f931-250">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) `../me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`</span></span> |
| <span data-ttu-id="5f931-251">Obter todos os emails recebidos pelo usuário conectado em abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="5f931-251">Get all emails received by the signed-in user in April 2017.</span></span> | <span data-ttu-id="5f931-252">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`</span><span class="sxs-lookup"><span data-stu-id="5f931-252">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`</span></span> |
| <span data-ttu-id="5f931-253">Obter todos os emails não lidos na caixa de entrada do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5f931-253">Get all unread mail in the signed-in user's Inbox.</span></span> | <span data-ttu-id="5f931-254">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=isRead eq false`</span><span class="sxs-lookup"><span data-stu-id="5f931-254">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=isRead eq false`</span></span> |
| <span data-ttu-id="5f931-255">Obter todos os usuários nos departamentos de Varejo e Vendas.</span><span class="sxs-lookup"><span data-stu-id="5f931-255">Get all users in the Retail and Sales departments.</span></span> | <span data-ttu-id="5f931-256">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3Ddepartment%20in%20('Retail'%2C%20'Sales')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) `../users?$filter=department in ('Retail', 'Sales')`</span><span class="sxs-lookup"><span data-stu-id="5f931-256">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3Ddepartment%20in%20('Retail'%2C%20'Sales')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) `../users?$filter=department in ('Retail', 'Sales')`</span></span>| 
| <span data-ttu-id="5f931-257">Listar os usuários com um plano de serviço específico que está em um estado suspenso.</span><span class="sxs-lookup"><span data-stu-id="5f931-257">List users with a particular service plan that is in a suspended state.</span></span> | <span data-ttu-id="5f931-258">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedPlans%2Fany(a%3Aa%2FservicePlanId%20eq%202e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2%20and%20a%2FcapabilityStatus%20eq%20'Suspended')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=assignedPlans/any(a:a/servicePlanId eq 2e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2 and a/capabilityStatus eq 'Suspended')&$count=true`.</span><span class="sxs-lookup"><span data-stu-id="5f931-258">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedPlans%2Fany(a%3Aa%2FservicePlanId%20eq%202e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2%20and%20a%2FcapabilityStatus%20eq%20'Suspended')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=assignedPlans/any(a:a/servicePlanId eq 2e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2 and a/capabilityStatus eq 'Suspended')&$count=true`.</span></span> <span data-ttu-id="5f931-259">Esta é uma [consulta avançada](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="5f931-259">This is an [advanced query](/graph/aad-advanced-queries).</span></span> |
| <span data-ttu-id="5f931-260">Listar todos os grupos que não são do Microsoft 365 em uma organização.</span><span class="sxs-lookup"><span data-stu-id="5f931-260">List all non-Microsoft 365 groups in an organization.</span></span> | <span data-ttu-id="5f931-261">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DNOT%20groupTypes%2Fany(c%3Ac%20eq%20'Unified')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$filter=NOT groupTypes/any(c:c eq 'Unified')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="5f931-261">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DNOT%20groupTypes%2Fany(c%3Ac%20eq%20'Unified')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$filter=NOT groupTypes/any(c:c eq 'Unified')&$count=true`</span></span> |
| <span data-ttu-id="5f931-262">Listar todos os usuários cujo nome da empresa não é indefinido (ou seja, não é um valor `null`) ou Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5f931-262">List all users whose company name is not undefined (that is, not a `null` value) or Microsoft.</span></span> | <span data-ttu-id="5f931-263">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`.</span><span class="sxs-lookup"><span data-stu-id="5f931-263">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`.</span></span> <span data-ttu-id="5f931-264">Esta é uma [consulta avançada](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="5f931-264">This is an [advanced query](/graph/aad-advanced-queries).</span></span> |
| <span data-ttu-id="5f931-265">Listar todos os usuários cujo nome da empresa seja indefinido ou Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5f931-265">List all users whose company name is either undefined or Microsoft.</span></span> | <span data-ttu-id="5f931-266">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20in%20(null%2C%20'Microsoft')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName in (null, 'Microsoft')&$count=true`.</span><span class="sxs-lookup"><span data-stu-id="5f931-266">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20in%20(null%2C%20'Microsoft')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName in (null, 'Microsoft')&$count=true`.</span></span> <span data-ttu-id="5f931-267">Esta é uma [consulta avançada](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="5f931-267">This is an [advanced query](/graph/aad-advanced-queries).</span></span> |
| <span data-ttu-id="5f931-268">Use a conversão OData para obter uma participação transitória em grupos com um nome de exibição que comece com “a”, incluindo o número de objetos retornados.</span><span class="sxs-lookup"><span data-stu-id="5f931-268">Use OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects.</span></span> | <span data-ttu-id="5f931-269">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`.</span><span class="sxs-lookup"><span data-stu-id="5f931-269">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`.</span></span> <span data-ttu-id="5f931-270">Esta é uma [consulta avançada](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="5f931-270">This is an [advanced query](/graph/aad-advanced-queries).</span></span> |

## <a name="format-parameter"></a><span data-ttu-id="5f931-271">parâmetro format</span><span class="sxs-lookup"><span data-stu-id="5f931-271">format parameter</span></span>

<span data-ttu-id="5f931-272">Use o parâmetro de consulta `$format` para especificar o formato de mídia dos itens retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5f931-272">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="5f931-273">Por exemplo, a seguinte solicitação retorna os usuários na organização no formato json:</span><span class="sxs-lookup"><span data-stu-id="5f931-273">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="5f931-274">[Experimentar no Explorador do Graph][format-example]</span><span class="sxs-lookup"><span data-stu-id="5f931-274">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="5f931-275">**Observação:** o parâmetro de consulta `$format` é compatível com vários formatos (por exemplo, atom, xml e json), mas os resultados podem não ser retornados em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="5f931-275">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="5f931-276">parâmetro orderby</span><span class="sxs-lookup"><span data-stu-id="5f931-276">orderby parameter</span></span>

<span data-ttu-id="5f931-277">Use o parâmetro de consulta `$orderby` para especificar a ordem de classificação dos itens retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5f931-277">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span> <span data-ttu-id="5f931-278">A ordem padrão é ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="5f931-278">The default order is ascending order.</span></span>

<span data-ttu-id="5f931-279">Por exemplo, a solicitação a seguir retorna os usuários da organização ordenados por seu nome de exibição:</span><span class="sxs-lookup"><span data-stu-id="5f931-279">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="5f931-280">[Experimentar no Explorador do Graph][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="5f931-280">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="5f931-p131">Você também pode classificar por entidades de tipo complexo. A solicitação abaixo obtém mensagens e as classifica pelo campo **address** da propriedade **from**, que é do tipo complexo **emailAddress**:</span><span class="sxs-lookup"><span data-stu-id="5f931-p131">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="5f931-283">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="5f931-283">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="5f931-284">Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="5f931-284">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span> <span data-ttu-id="5f931-285">Se a ordem de classificação não for especificada, o padrão (ordem crescente) será inferido.</span><span class="sxs-lookup"><span data-stu-id="5f931-285">If the sort order is not specified, the default (ascending order) is inferred.</span></span>

<span data-ttu-id="5f931-p133">Com algumas APIs, você pode ordenar os resultados em várias propriedades. Por exemplo, a solicitação a seguir ordena as mensagens na caixa de entrada do usuário primeiro pelo nome da pessoa que enviou, em ordem decrescente (Z a A) e, em seguida, por assunto, em ordem crescente (padrão).</span><span class="sxs-lookup"><span data-stu-id="5f931-p133">With some APIs, you can order results on multiple properties. For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="5f931-288">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="5f931-288">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

> <span data-ttu-id="5f931-289">**Observação:** Quando você especificar `$filter` o servidor inferirá uma ordem de classificação para os resultados.</span><span class="sxs-lookup"><span data-stu-id="5f931-289">**Note:** When you specify `$filter` the server will infer a sort order for the results.</span></span> <span data-ttu-id="5f931-290">Se você usar `$orderby` e `$filter` juntos para receber mensagens, como o servidor sempre infere uma ordem de classificação para os resultados de `$filter`, você deve [especificar propriedades de determinadas maneiras](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query).</span><span class="sxs-lookup"><span data-stu-id="5f931-290">If you use both `$orderby` and `$filter` to get messages, because the server always infers a sort order for the results of a `$filter`, you must [specify properties in certain ways](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query).</span></span>


<span data-ttu-id="5f931-291">O exemplo a seguir mostra uma consulta filtrada pelas propriedades **subject** e **priority** e classificadas pelas propriedades **subject**, **priority** e **receivedDateTime** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="5f931-291">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="5f931-292">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="5f931-292">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

> [!NOTE] 
> <span data-ttu-id="5f931-293">A combinação dos parâmetros de consulta `$orderby` e `$filter` não tem suporte para objetos de diretório.</span><span class="sxs-lookup"><span data-stu-id="5f931-293">Combining `$orderby` and `$filter` query parameters is supported for directory objects.</span></span> <span data-ttu-id="5f931-294">Consulte [Recursos avançados de consulta em objetos de diretório do Microsoft Azure Active Directory](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="5f931-294">See [Advanced query capabilities in Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="search-parameter"></a><span data-ttu-id="5f931-295">parâmetro search</span><span class="sxs-lookup"><span data-stu-id="5f931-295">search parameter</span></span>

<span data-ttu-id="5f931-296">Use o parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="5f931-296">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span> <span data-ttu-id="5f931-297">Sua sintaxe e comportamento variam de uma operação de API para outra.</span><span class="sxs-lookup"><span data-stu-id="5f931-297">It's syntax and behavior varies from one API operation to another.</span></span> <span data-ttu-id="5f931-298">Para ver a sintaxe para `$search` em diferentes recursos, consulte [Usar o parâmetro de consulta $search para corresponder a um critério de pesquisa](/graph/search-query-parameter).</span><span class="sxs-lookup"><span data-stu-id="5f931-298">To see the syntax for `$search` across different resources, see [Use the $search query parameter to match a search criterion](/graph/search-query-parameter).</span></span>

## <a name="select-parameter"></a><span data-ttu-id="5f931-299">parâmetro select</span><span class="sxs-lookup"><span data-stu-id="5f931-299">select parameter</span></span>

<span data-ttu-id="5f931-300">Use o parâmetro de consulta `$select` para retornar um conjunto de propriedades diferente do padrão definido para um recurso individual ou um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="5f931-300">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="5f931-301">Com `$select`, você pode especificar um subconjunto ou um superconjunto das propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="5f931-301">With `$select`, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="5f931-302">Por exemplo, ao recuperar as mensagens do usuário conectado, você pode especificar que somente as propriedades **from** e **subject** sejam retornadas:</span><span class="sxs-lookup"><span data-stu-id="5f931-302">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="5f931-303">[Experimentar no Explorador do Graph][select-example]</span><span class="sxs-lookup"><span data-stu-id="5f931-303">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="5f931-304">**Importante:** Em geral, recomendamos que você use `$select` para limitar as propriedades retornadas por uma consulta àqueles exigidas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5f931-304">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="5f931-305">Isso se aplica particularmente a consultas com o potencial de retornar um conjunto de resultados amplo.</span><span class="sxs-lookup"><span data-stu-id="5f931-305">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="5f931-306">Limitar as propriedades retornadas em cada linha reduzirá a carga de rede e ajudará a melhorar o desempenho do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5f931-306">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="5f931-p139">No `v1.0`, alguns recursos do Azure AD que derivam de [directoryObject](/graph/api/resources/directoryobject), como [usuário](/graph/api/resources/user) e [grupo](/graph/api/resources/group), retornam um subconjunto limitado padrão de propriedades em leituras. Para esses recursos, você deve usar `$select` para retornar propriedades fora do conjunto padrão.</span><span class="sxs-lookup"><span data-stu-id="5f931-p139">In `v1.0`, some Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject), like [user](/graph/api/resources/user) and [group](/graph/api/resources/group), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="5f931-309">parâmetro skip</span><span class="sxs-lookup"><span data-stu-id="5f931-309">skip parameter</span></span>

<span data-ttu-id="5f931-p140">Use o parâmetro de consulta `$skip` para definir o número de itens para ignorar no início de um conjunto. Por exemplo, a solicitação a seguir retorna eventos para o usuário classificadas por data de criação, começando com o evento 21 no conjunto:</span><span class="sxs-lookup"><span data-stu-id="5f931-p140">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="5f931-312">[Experimentar no Explorador do Graph][skip-example]</span><span class="sxs-lookup"><span data-stu-id="5f931-312">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="5f931-313">**Observação:** algumas APIs do Microsoft Graph, como Email e Calendário do Outlook (**message**, **event** e **calendar**), usam `$skip` para implementar a paginação.</span><span class="sxs-lookup"><span data-stu-id="5f931-313">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="5f931-314">Quando os resultados de uma consulta ocuparem várias páginas, essas APIs retornarão uma propriedade `@odata:nextLink` com uma URL que contém um parâmetro `$skip`.</span><span class="sxs-lookup"><span data-stu-id="5f931-314">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="5f931-315">Você pode usar essa URL para retornar a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="5f931-315">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="5f931-316">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="5f931-316">To learn more, see [Paging](./paging.md).</span></span>
>
> <span data-ttu-id="5f931-317">O cabeçalho **consistencyLevel** necessário para consultas avançadas em objetos de diretório não está incluído por padrão em solicitações de página subsequentes.</span><span class="sxs-lookup"><span data-stu-id="5f931-317">The **ConsistencyLevel** header required for advanced queries against directory objects is not included by default in subsequent page requests.</span></span> <span data-ttu-id="5f931-318">Ele deve ser definido explicitamente nas páginas subsequentes.</span><span class="sxs-lookup"><span data-stu-id="5f931-318">It must be set explicitly in subsequent pages.</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="5f931-319">parâmetro skipToken</span><span class="sxs-lookup"><span data-stu-id="5f931-319">skipToken parameter</span></span>

<span data-ttu-id="5f931-320">Algumas solicitações retornam várias páginas de dados, devido à paginação do lado do servidor ou devido ao uso do parâmetro [`$top`](#top-parameter) para limitar o tamanho da página da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f931-320">Some requests return multiple pages of data, either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response.</span></span> <span data-ttu-id="5f931-321">Muitas APIs do Microsoft Graph usam o parâmetro de consulta `skipToken` para fazer referência a páginas subsequentes do resultado.</span><span class="sxs-lookup"><span data-stu-id="5f931-321">Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result.</span></span>  
<span data-ttu-id="5f931-322">O parâmetro `$skiptoken` contém um token opaco que faz referência à próxima página de resultados e é retornado na URL fornecida na propriedade `@odata.nextLink` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5f931-322">The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response.</span></span> <span data-ttu-id="5f931-323">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="5f931-323">To learn more, see [Paging](./paging.md).</span></span>
> <span data-ttu-id="5f931-324">**Observação:** Se você estiver usando a OData Count (adicionando `$count=true` na cadeia de caracteres de consulta) para consultas em objetos de diretório, a propriedade `@odata.count` estará presente apenas na primeira página.</span><span class="sxs-lookup"><span data-stu-id="5f931-324">**Note:** If you're using OData Count (adding `$count=true` in the query string) for queries against directory objects, the `@odata.count` property is present only in the first page.</span></span>
>
> <span data-ttu-id="5f931-325">O cabeçalho **consistencyLevel** necessário para consultas avançadas em objetos de diretório não está incluído por padrão em solicitações de página subsequentes.</span><span class="sxs-lookup"><span data-stu-id="5f931-325">The **ConsistencyLevel** header required for advanced queries against directory objects is not included by default in subsequent page requests.</span></span> <span data-ttu-id="5f931-326">Ele deve ser definido explicitamente nas páginas subsequentes.</span><span class="sxs-lookup"><span data-stu-id="5f931-326">It must be set explicitly in subsequent pages.</span></span>

## <a name="top-parameter"></a><span data-ttu-id="5f931-327">parâmetro top</span><span class="sxs-lookup"><span data-stu-id="5f931-327">top parameter</span></span>

<span data-ttu-id="5f931-328">Use o parâmetro de consulta `$top` para especificar o tamanho de página do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="5f931-328">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="5f931-329">Se restarem mais itens no conjunto de resultados, o corpo da resposta conterá um parâmetro `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="5f931-329">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="5f931-330">Esse parâmetro contém uma URL que você pode usar para obter a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="5f931-330">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="5f931-331">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="5f931-331">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="5f931-332">O valor mínimo de $top é 1 e o máximo depende da API correspondente.</span><span class="sxs-lookup"><span data-stu-id="5f931-332">The minimum value of $top is 1 and the maximum depends on the corresponding API.</span></span>  

<span data-ttu-id="5f931-333">Por exemplo, a seguinte solicitação de [lista de mensagens](/graph/api/user-list-messages) retorna as cinco primeiras mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="5f931-333">For example, the following [list messages](/graph/api/user-list-messages) request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="5f931-334">[Experimentar no Explorador do Graph][top-example]</span><span class="sxs-lookup"><span data-stu-id="5f931-334">[Try in Graph Explorer][top-example]</span></span>

> <span data-ttu-id="5f931-335">O cabeçalho **consistencyLevel** necessário para consultas avançadas em objetos de diretório não está incluído por padrão em solicitações de página subsequentes.</span><span class="sxs-lookup"><span data-stu-id="5f931-335">The **ConsistencyLevel** header required for advanced queries against directory objects is not included by default in subsequent page requests.</span></span> <span data-ttu-id="5f931-336">Ele deve ser definido explicitamente nas páginas subsequentes.</span><span class="sxs-lookup"><span data-stu-id="5f931-336">It must be set explicitly in subsequent pages.</span></span>

## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="5f931-337">Tratamento de erro para parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="5f931-337">Error handling for query parameters</span></span>

<span data-ttu-id="5f931-p148">Algumas solicitações retornarão uma mensagem de erro se não houver suporte para um parâmetro de consulta especificado. Por exemplo, você não pode usar `$expand` na relação `user/photo`.</span><span class="sxs-lookup"><span data-stu-id="5f931-p148">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="5f931-340">No entanto, é importante observar que os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente.</span><span class="sxs-lookup"><span data-stu-id="5f931-340">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="5f931-341">Isso pode ser verdadeiro para parâmetros de consulta sem suporte, bem como para combinações de parâmetros de consulta sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f931-341">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="5f931-342">Nesses casos, você deve examinar os dados retornados pela solicitação para determinar se os parâmetros de consulta que especificou tiveram o efeito desejado.</span><span class="sxs-lookup"><span data-stu-id="5f931-342">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

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



- [<span data-ttu-id="5f931-343">Recursos avançados de consulta em objetos de diretório do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="5f931-343">Advanced query capabilities on Azure AD directory objects</span></span>](/graph/aad-advanced-queries)
- [<span data-ttu-id="5f931-344">Limitações de parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="5f931-344">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)
- [<span data-ttu-id="5f931-345">Use o parâmetro de consulta $search para corresponder a um critério de pesquisa</span><span class="sxs-lookup"><span data-stu-id="5f931-345">Use the $search query parameter to match a search criterion</span></span>](/graph/search-query-parameter)