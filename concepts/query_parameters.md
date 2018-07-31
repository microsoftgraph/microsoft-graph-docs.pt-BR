# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="f15ab-101">Usar parâmetros de consulta para personalizar respostas</span><span class="sxs-lookup"><span data-stu-id="f15ab-101">Use query parameters to customize responses</span></span>

<span data-ttu-id="f15ab-p101">O Microsoft Graph fornece parâmetros de consulta opcional que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta. Há suporte para os parâmetros de consulta a seguir.</span><span class="sxs-lookup"><span data-stu-id="f15ab-p101">Microsoft Graph provides optional query parameters that you can use to specify and control the amount of data returned in a response. The following query parameters are supported.</span></span>

><span data-ttu-id="f15ab-104">**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="f15ab-104">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="f15ab-105">Nome</span><span class="sxs-lookup"><span data-stu-id="f15ab-105">Name</span></span>                     | <span data-ttu-id="f15ab-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="f15ab-106">Description</span></span> | <span data-ttu-id="f15ab-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f15ab-107">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="f15ab-108">$count</span><span class="sxs-lookup"><span data-stu-id="f15ab-108">$count</span></span>](#count-parameter)         | <span data-ttu-id="f15ab-109">Recupera a contagem total de recursos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="f15ab-109">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="f15ab-110">$expand</span><span class="sxs-lookup"><span data-stu-id="f15ab-110">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="f15ab-111">Recupera os recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="f15ab-111">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="f15ab-112">$filter</span><span class="sxs-lookup"><span data-stu-id="f15ab-112">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="f15ab-113">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="f15ab-113">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="f15ab-114">$format</span><span class="sxs-lookup"><span data-stu-id="f15ab-114">$format</span></span>](#format-parameter)       | <span data-ttu-id="f15ab-115">Retorna os resultados no formato de mídia especificado.</span><span class="sxs-lookup"><span data-stu-id="f15ab-115">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="f15ab-116">$orderby</span><span class="sxs-lookup"><span data-stu-id="f15ab-116">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="f15ab-117">Ordena os resultados.</span><span class="sxs-lookup"><span data-stu-id="f15ab-117">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="f15ab-118">$search</span><span class="sxs-lookup"><span data-stu-id="f15ab-118">$search</span></span>](#search-parameter)       | <span data-ttu-id="f15ab-p102">Retorna os resultados com base nos critérios de pesquisa. Atualmente, com suporte em conjuntos de **mensagens** e **pessoa**.</span><span class="sxs-lookup"><span data-stu-id="f15ab-p102">Returns results based on search criteria. Currently supported on **messages** and **person** collections.</span></span>|[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="f15ab-121">$select</span><span class="sxs-lookup"><span data-stu-id="f15ab-121">$select</span></span>](#select-parameter)       | <span data-ttu-id="f15ab-122">Filtra as propriedades (colunas).</span><span class="sxs-lookup"><span data-stu-id="f15ab-122">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="f15ab-123">$skip</span><span class="sxs-lookup"><span data-stu-id="f15ab-123">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="f15ab-p103">Índices em um conjunto de resultados. Também usado por algumas APIs para implementar a paginação e pode ser usado com `$top` para paginar resultados manualmente.</span><span class="sxs-lookup"><span data-stu-id="f15ab-p103">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="f15ab-126">$skipToken</span><span class="sxs-lookup"><span data-stu-id="f15ab-126">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="f15ab-p104">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas. (Algumas APIs usam `$skip` em vez disso.)</span><span class="sxs-lookup"><span data-stu-id="f15ab-p104">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|
| [<span data-ttu-id="f15ab-129">$top</span><span class="sxs-lookup"><span data-stu-id="f15ab-129">$top</span></span>](#top-parameter)             | <span data-ttu-id="f15ab-130">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="f15ab-130">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]



<span data-ttu-id="f15ab-131">Esses parâmetros são compatíveis com a [linguagem de consulta OData V4][odata-query].</span><span class="sxs-lookup"><span data-stu-id="f15ab-131">These parameters are compatible with the [OData V4 query language][odata-query].</span></span> <span data-ttu-id="f15ab-132">Nem todos os parâmetros têm suporte em todas as APIs do Microsoft Graph, e o suporte pode diferir significativamente entre os pontos de extremidade `v1.0` e `beta`.</span><span class="sxs-lookup"><span data-stu-id="f15ab-132">Not all parameters are supported across all Microsoft Graph APIs, and support might differ significantly between the `v1.0` and `beta` endpoints.</span></span> 

> <span data-ttu-id="f15ab-p106">**Observação:** No ponto de extremidade `beta`, o prefixo `$` é opcional. Por exemplo, em vez de `$filter`, você pode usar `filter`. Para obter mais detalhes e exemplos, confira [Suporte a parâmetros da consulta sem prefixos $ no Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span><span class="sxs-lookup"><span data-stu-id="f15ab-p106">**Note:** On the `beta` endpoint, the `$` prefix is optional. For example, instead of `$filter`, you can use `filter`. For more details and examples, see [Supporting query parameters without $ prefixes in Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span></span>

## <a name="encoding-query-parameters"></a><span data-ttu-id="f15ab-136">Codificação de parâmetros da consulta</span><span class="sxs-lookup"><span data-stu-id="f15ab-136">Encoding query parameters</span></span>

<span data-ttu-id="f15ab-137">Os valores dos parâmetros da consulta devem ser codificados por porcentagem.</span><span class="sxs-lookup"><span data-stu-id="f15ab-137">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="f15ab-138">Muitas ferramentas, navegadores e clientes HTTP (como o [Explorador do Graph][graph-explorer]) ajudarão você com isso.</span><span class="sxs-lookup"><span data-stu-id="f15ab-138">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="f15ab-139">Se uma consulta está falhando, uma causa possível é a falha na codificação adequada dos valores dos parâmetros da consulta.</span><span class="sxs-lookup"><span data-stu-id="f15ab-139">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="f15ab-140">Uma URL descodificada é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="f15ab-140">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="f15ab-141">Uma URL codificada adequadamente é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="f15ab-141">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count-parameter"></a><span data-ttu-id="f15ab-142">parâmetro count</span><span class="sxs-lookup"><span data-stu-id="f15ab-142">count parameter</span></span>

<span data-ttu-id="f15ab-143">Use o parâmetro de consulta `$count` para incluir uma contagem do número total de itens em um conjunto, juntamente com a página de valores de dados retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f15ab-143">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="f15ab-144">Por exemplo, a solicitação a seguir retornará o conjunto **contato** do usuário atual e o número de itens no conjunto **contato** na propriedade `@odata.count`.</span><span class="sxs-lookup"><span data-stu-id="f15ab-144">For example, the following request will return both the **contact** collection of the current user, and the number of items in the **contact** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="f15ab-145">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="f15ab-145">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="f15ab-146">**Observação:** `$count` não tem suporte para conjuntos de recursos derivados de [directoryObject](../api-reference/v1.0/resources/directoryobject.md), como conjuntos de [usuários](../api-reference/v1.0/resources/user.md) ou [grupos](../api-reference/v1.0/resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="f15ab-146">**Note:** `$count` is not supported for collections of resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md) like collections of [users](../api-reference/v1.0/resources/user.md) or [groups](../api-reference/v1.0/resources/group.md).</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="f15ab-147">parâmetro expand</span><span class="sxs-lookup"><span data-stu-id="f15ab-147">expand parameter</span></span>

<span data-ttu-id="f15ab-148">Muitos recursos do Microsoft Graph expõem as propriedades declaradas do recurso, bem como as relações delas com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="f15ab-148">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="f15ab-149">Essas relações também são chamadas de propriedades de referência ou propriedades de navegação e podem fazer referência a um único recurso ou a um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="f15ab-149">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="f15ab-150">Por exemplo, as pastas de email, gerente e subordinados diretos de um usuário são todas expostas como relações.</span><span class="sxs-lookup"><span data-stu-id="f15ab-150">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="f15ab-p109">Normalmente, você pode consultar as propriedades de um recurso ou uma de suas relações em uma única solicitação, mas não ambas. Você pode usar o parâmetro de cadeia de caracteres de consulta `$expand` para incluir o recurso expandido ou o conjunto referenciado por uma única relação (propriedade de navegação) nos resultados.</span><span class="sxs-lookup"><span data-stu-id="f15ab-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="f15ab-153">O seguinte exemplo obtém informações de unidade raiz juntamente com os itens filho de nível superior em uma unidade:</span><span class="sxs-lookup"><span data-stu-id="f15ab-153">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="f15ab-154">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="f15ab-154">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="f15ab-p110">Com alguns conjuntos de recursos, você também pode especificar as propriedades a serem retornadas nos recursos expandidos adicionando um parâmetro `$select`. O exemplo a seguir executa a mesma consulta que o exemplo anterior, mas usa uma instrução [`$select`](#select-parameter) para limitar as propriedades retornadas para os itens filho expandidos para as propriedades **id** e **name**.</span><span class="sxs-lookup"><span data-stu-id="f15ab-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **id** and **name** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="f15ab-157">[Experimentar no Explorador do Graph][expand-example]</span><span class="sxs-lookup"><span data-stu-id="f15ab-157">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="f15ab-p111">**Observação:** nem todas as relações e recursos dão suporte ao parâmetro de consulta `$expand`. Por exemplo, você pode expandir as relações **directReports**, **manager** e **memberOf** em um usuário, mas não pode expandir suas relações **events**, **messages** ou **photo**. Nem todos os recursos ou relações dão suporte ao uso de `$select` em itens expandidos.</span><span class="sxs-lookup"><span data-stu-id="f15ab-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the **directReports**, **manager**, and **memberOf** relationships on a user, but you cannot expand its **events**, **messages**, or **photo** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="f15ab-161">Com recursos do Azure AD derivados de [directoryObject](../api-reference/v1.0/resources/directoryobject.md), como [user](../api-reference/v1.0/resources/user.md) e [group](../api-reference/v1.0/resources/group.md), `$expand` só há suporte para `beta`, e normalmente são retornados no máximo 20 itens para a relação expandida.</span><span class="sxs-lookup"><span data-stu-id="f15ab-161">With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="f15ab-162">parâmetro filter</span><span class="sxs-lookup"><span data-stu-id="f15ab-162">filter parameter</span></span>

<span data-ttu-id="f15ab-163">Use o parâmetro de consulta `$filter` para recuperar apenas um subconjunto de um conjunto.</span><span class="sxs-lookup"><span data-stu-id="f15ab-163">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="f15ab-164">Por exemplo, para localizar os usuários cujo nome de exibição se inicia com a letra "J", use `startswith`.</span><span class="sxs-lookup"><span data-stu-id="f15ab-164">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="f15ab-165">[Experimentar no Explorador do Graph][filter-example]</span><span class="sxs-lookup"><span data-stu-id="f15ab-165">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="f15ab-166">O suporte para operadores `$filter` varia entre as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f15ab-166">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="f15ab-167">Os seguintes operadores lógicos geralmente são suportados:</span><span class="sxs-lookup"><span data-stu-id="f15ab-167">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="f15ab-168">igual a (`eq`)</span><span class="sxs-lookup"><span data-stu-id="f15ab-168">equals (`eq`)</span></span>
- <span data-ttu-id="f15ab-169">não é igual a (`ne`)</span><span class="sxs-lookup"><span data-stu-id="f15ab-169">not equals (`ne`)</span></span>
- <span data-ttu-id="f15ab-170">maior que (`gt`)</span><span class="sxs-lookup"><span data-stu-id="f15ab-170">greater than (`gt`)</span></span>
- <span data-ttu-id="f15ab-171">maior ou igual a (`ge`)</span><span class="sxs-lookup"><span data-stu-id="f15ab-171">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="f15ab-172">menor que (`lt`), menor ou igual a (`le`)</span><span class="sxs-lookup"><span data-stu-id="f15ab-172">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="f15ab-173">e (`and`)</span><span class="sxs-lookup"><span data-stu-id="f15ab-173">and (`and`)</span></span>
- <span data-ttu-id="f15ab-174">ou (`or`)</span><span class="sxs-lookup"><span data-stu-id="f15ab-174">or (`or`)</span></span>
- <span data-ttu-id="f15ab-175">não (`not`)</span><span class="sxs-lookup"><span data-stu-id="f15ab-175">not (`not`)</span></span>
 
<span data-ttu-id="f15ab-176">O operador de cadeia de caracteres `startswith` geralmente é suportado.</span><span class="sxs-lookup"><span data-stu-id="f15ab-176">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="f15ab-177">O operador lambda `any` tem suporte em algumas APIs.</span><span class="sxs-lookup"><span data-stu-id="f15ab-177">The `any` lambda operator is supported for some APIs.</span></span> <span data-ttu-id="f15ab-178">Para ver alguns exemplos de uso, confira a tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f15ab-178">For some  usage examples, see the following table.</span></span> <span data-ttu-id="f15ab-179">Para obter mais detalhes sobre a sintaxe `$filter`, confira o [protocolo OData][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="f15ab-179">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="f15ab-180">A tabela a seguir mostra alguns exemplos que usam o parâmetro de consulta `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f15ab-180">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="f15ab-181">**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="f15ab-181">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="f15ab-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="f15ab-182">Description</span></span> | <span data-ttu-id="f15ab-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f15ab-183">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="f15ab-184">Pesquisar por usuários com o nome Clara entre várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="f15ab-184">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| <span data-ttu-id="f15ab-185">Obter todos os eventos do usuário conectado que começaram após 01/07/2017.</span><span class="sxs-lookup"><span data-stu-id="f15ab-185">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| <span data-ttu-id="f15ab-186">Obter todos os emails de um endereço específico recebidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="f15ab-186">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| <span data-ttu-id="f15ab-187">Obter todos os emails recebidos pelo usuário conectado em abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="f15ab-187">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| <span data-ttu-id="f15ab-188">Obter todos os emails não lidos na caixa de entrada do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="f15ab-188">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| <span data-ttu-id="f15ab-189">Listar todos os grupos do Office 365 em uma organização.</span><span class="sxs-lookup"><span data-stu-id="f15ab-189">List all Office 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> <span data-ttu-id="f15ab-p114">**Observação:** Os seguintes operadores `$filter` não têm suporte para recursos do Azure AD: `ne`, `gt`, `ge`, `lt`, `le` e `not`. O operador de cadeia de caracteres `contains` atualmente não tem suporte em nenhum recurso do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f15ab-p114">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="f15ab-192">parâmetro format</span><span class="sxs-lookup"><span data-stu-id="f15ab-192">format parameter</span></span>

<span data-ttu-id="f15ab-193">Use o parâmetro de consulta `$format` para especificar o formato de mídia dos itens retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f15ab-193">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="f15ab-194">Por exemplo, a seguinte solicitação retorna os usuários na organização no formato json:</span><span class="sxs-lookup"><span data-stu-id="f15ab-194">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="f15ab-195">[Experimentar no Explorador do Graph][format-example]</span><span class="sxs-lookup"><span data-stu-id="f15ab-195">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="f15ab-196">**Observação:** o parâmetro de consulta `$format` é compatível com vários formatos (por exemplo, atom, xml e json), mas os resultados podem não ser retornados em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="f15ab-196">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="f15ab-197">parâmetro orderby</span><span class="sxs-lookup"><span data-stu-id="f15ab-197">orderby parameter</span></span>

<span data-ttu-id="f15ab-198">Use o parâmetro de consulta `$orderby` para especificar a ordem de classificação dos itens retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f15ab-198">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="f15ab-199">Por exemplo, a solicitação a seguir retorna os usuários da organização ordenados por seu nome de exibição:</span><span class="sxs-lookup"><span data-stu-id="f15ab-199">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="f15ab-200">[Experimentar no Explorador do Graph][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="f15ab-200">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="f15ab-p115">Você também pode classificar por entidades de tipo complexo. A solicitação abaixo obtém mensagens e as classifica pelo campo **address** da propriedade **from**, que é do tipo complexo **emailAddress**:</span><span class="sxs-lookup"><span data-stu-id="f15ab-p115">You can also sort by complex type entities. The following request gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="f15ab-203">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="f15ab-203">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="f15ab-204">Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="f15ab-204">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="f15ab-205">Com algumas APIs, você pode ordenar os resultados em várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="f15ab-205">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="f15ab-206">Por exemplo, a solicitação a seguir ordena as mensagens na caixa de entrada do usuário primeiro pelo nome da pessoa que enviou, em ordem decrescente (Z – A) e, em seguida, por assunto, em ordem ascendente (padrão).</span><span class="sxs-lookup"><span data-stu-id="f15ab-206">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="f15ab-207">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="f15ab-207">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

<span data-ttu-id="f15ab-208">Quando você especifica $filter, servidor deduz uma ordem de classificação para os resultados.</span><span class="sxs-lookup"><span data-stu-id="f15ab-208">When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="f15ab-209">Se você usar `$orderby` e `$filter`, como o servidor sempre deduz a ordem de classificação dos resultados de um `$filter`, as propriedades do `$filter` devem estar listadas primeiro no `$orderby` antes de outras propriedades e devem estar listadas na ordem que aparecem no parâmetro `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f15ab-209">If you use both `$orderby` and `$filter`, because the server always infers a sort order for the results of a `$filter`, the properties in the `$filter` must be listed first in the `$orderby` before any other properties, and they must be listed in the order that they appear in the `$filter` parameter.</span></span> 

<span data-ttu-id="f15ab-210">O exemplo a seguir mostra uma consulta filtrada pelas propriedades **subject** e **priority** e classificadas pelas propriedades **subject**, **priority** e **receivedDateTime** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="f15ab-210">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="f15ab-211">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="f15ab-211">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > <span data-ttu-id="f15ab-212">**Observação:** Com os recursos do Azure AD derivados de [directoryObject](../api-reference/v1.0/resources/directoryobject.md), como [user](../api-reference/v1.0/resources/user.md) e [group](../api-reference/v1.0/resources/group.md), você não pode combinar `$orderby` a expressões `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f15ab-212">**Note:** With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search-parameter"></a><span data-ttu-id="f15ab-213">parâmetro search</span><span class="sxs-lookup"><span data-stu-id="f15ab-213">search parameter</span></span>

<span data-ttu-id="f15ab-214">Use o parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f15ab-214">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="f15ab-p118">**Observação:** Atualmente, é possível pesquisar **somente** coleções de [mensagens](../api-reference/v1.0/resources/message.md) e [pessoas](../api-reference/v1.0/resources/person.md). Uma solicitação de `$search` retorna até 250 resultados. Não é possível usar [`$filter`](#filter-parameter) ou [`$orderby`](#orderby-parameter) em uma solicitação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f15ab-p118">**Note:** You can currently search **only** [message](../api-reference/v1.0/resources/message.md) and [person](../api-reference/v1.0/resources/person.md) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter-parameter) or [`$orderby`](#orderby-parameter) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="f15ab-218">Usando $search em conjuntos de mensagens</span><span class="sxs-lookup"><span data-stu-id="f15ab-218">Using $search on message collections</span></span>

<span data-ttu-id="f15ab-219">Aplicativos do Office 365, como Outlook e SharePoint, oferecem suporte à sintaxe da Linguagem de Consulta de Palavra-Chave (KQL) para fazer pesquisas.</span><span class="sxs-lookup"><span data-stu-id="f15ab-219">Office 365 applications, such as Outlook and SharePoint, support the Keyword Query Language (KQL) syntax to do searches.</span></span> <span data-ttu-id="f15ab-220">Isso oferece a comodidade de um domínio de descoberta comum para os repositórios de dados.</span><span class="sxs-lookup"><span data-stu-id="f15ab-220">This provides the convenience of a common discovery domain for their data stores.</span></span> 

<span data-ttu-id="f15ab-221">Você pode especificar os seguintes nomes de propriedade reconhecidos pelo KQL em uma cadeia de consulta $search.</span><span class="sxs-lookup"><span data-stu-id="f15ab-221">You can specify the following property names that KQL recognizes in a $search query string.</span></span> <span data-ttu-id="f15ab-222">Esses nomes de propriedade não são definidos em propriedades na entidade **message**, mas são internamente mapeados para propriedades na entidade **message**.</span><span class="sxs-lookup"><span data-stu-id="f15ab-222">These property names are not properties defined in the **message** entity, but are internally mapped to properties in the **message** entity.</span></span> <span data-ttu-id="f15ab-223">Confira [propriedades pesquisáveis no Exchange](https://docs.microsoft.com/pt-BR/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange) para obter exemplos e saber mais.</span><span class="sxs-lookup"><span data-stu-id="f15ab-223">See [searchable properties in Exchange](https://docs.microsoft.com/pt-BR/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange) for more information and examples.</span></span>

- <span data-ttu-id="f15ab-224">**attachment**</span><span class="sxs-lookup"><span data-stu-id="f15ab-224">**attachment**</span></span>
- <span data-ttu-id="f15ab-225">**bcc**</span><span class="sxs-lookup"><span data-stu-id="f15ab-225">**bcc**</span></span>
- <span data-ttu-id="f15ab-226">**body**</span><span class="sxs-lookup"><span data-stu-id="f15ab-226">**body**</span></span>
- <span data-ttu-id="f15ab-227">**category**</span><span class="sxs-lookup"><span data-stu-id="f15ab-227">**category**</span></span>
- <span data-ttu-id="f15ab-228">**cc**</span><span class="sxs-lookup"><span data-stu-id="f15ab-228">**cc**</span></span>
- <span data-ttu-id="f15ab-229">**content**</span><span class="sxs-lookup"><span data-stu-id="f15ab-229">**content**</span></span>
- <span data-ttu-id="f15ab-230">**from**</span><span class="sxs-lookup"><span data-stu-id="f15ab-230">**from**</span></span>
- <span data-ttu-id="f15ab-231">**has**</span><span class="sxs-lookup"><span data-stu-id="f15ab-231">**has**</span></span>
- <span data-ttu-id="f15ab-232">**importance**</span><span class="sxs-lookup"><span data-stu-id="f15ab-232">**Importance**</span></span>
- <span data-ttu-id="f15ab-233">**participants**</span><span class="sxs-lookup"><span data-stu-id="f15ab-233">**participants**</span></span>
- <span data-ttu-id="f15ab-234">**received**</span><span class="sxs-lookup"><span data-stu-id="f15ab-234">**Received**</span></span>
- <span data-ttu-id="f15ab-235">**sender**</span><span class="sxs-lookup"><span data-stu-id="f15ab-235">**sender**</span></span>
- <span data-ttu-id="f15ab-236">**subject**</span><span class="sxs-lookup"><span data-stu-id="f15ab-236">**subject**</span></span>
- <span data-ttu-id="f15ab-237">**to**</span><span class="sxs-lookup"><span data-stu-id="f15ab-237">**to**</span></span>

<span data-ttu-id="f15ab-238">Se você realizar uma pesquisa em mensagens e especificar apenas um valor, a pesquisa será realizada nas propriedades de pesquisa padrão **from**, **subject** e **body**.</span><span class="sxs-lookup"><span data-stu-id="f15ab-238">If you do a search on messages and specify only a value, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="f15ab-239">Os resultados de uma pesquisa em um conjunto de mensagens são classificados pela data e hora em que a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="f15ab-239">The results of a search on a message collection are sorted by the date and time that the message was sent.</span></span>

<span data-ttu-id="f15ab-240">O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:</span><span class="sxs-lookup"><span data-stu-id="f15ab-240">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="f15ab-241">[Experimentar no Explorador do Graph][search-example]</span><span class="sxs-lookup"><span data-stu-id="f15ab-241">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="f15ab-242">O próximo exemplo procura todas as mensagens na Caixa de Entrada do usuário que foram enviadas de um endereço de email específico:</span><span class="sxs-lookup"><span data-stu-id="f15ab-242">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```
<span data-ttu-id="f15ab-243">Para saber mais sobre a KQL como a sintaxe, operadores com suporte e dicas de pesquisa, confira os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="f15ab-243">For more information about KQL such as the syntax, supported operators, and tips on searching, see the following articles:</span></span>

- [<span data-ttu-id="f15ab-244">Referência de sintaxe da Linguagem de Consulta de Palavra-chave (KQL)</span><span class="sxs-lookup"><span data-stu-id="f15ab-244">Keyword Query Language (KQL) syntax reference</span></span>](https://docs.microsoft.com/pt-BR/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- <span data-ttu-id="f15ab-245">
  [Propriedades da mensagem e operadores de pesquisa para a Descoberta eletrônica In-loco no Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span><span class="sxs-lookup"><span data-stu-id="f15ab-245">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="f15ab-246">Usando $search em conjuntos de pessoas</span><span class="sxs-lookup"><span data-stu-id="f15ab-246">Using $search on person collections</span></span>

<span data-ttu-id="f15ab-p121">Você pode usar a API de Pessoas do Microsoft Graph para recuperar as pessoas mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. A API de Pessoas dá suporte ao parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="f15ab-p121">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="f15ab-250">As pesquisas de pessoas ocorrem nas propriedades **displayName** e **emailAddress** do recurso [person](../api-reference/v1.0/resources/person.md).</span><span class="sxs-lookup"><span data-stu-id="f15ab-250">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](../api-reference/v1.0/resources/person.md) resource.</span></span>

<span data-ttu-id="f15ab-251">A seguinte solicitação faz uma pesquisa por uma pessoa chamada "Clara Barbosa" nas propriedades **displayName** e **emailAddress** em todos os indivíduos no conjunto de **Pessoas** do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="f15ab-251">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="f15ab-252">Como uma pessoa denominada "Clara Barbosa" é relevante para o usuário conectado, as informações para "Clara Barbosa" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="f15ab-252">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="f15ab-253">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="f15ab-253">The following example shows the response.</span></span> 

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

<span data-ttu-id="f15ab-254">Saiba mais sobre a API de Pessoas em [Obter informações sobre pessoas relevantes](./people_example.md#search-people).</span><span class="sxs-lookup"><span data-stu-id="f15ab-254">To learn more about the People API, see [Get information about relevant people](./people_example.md#search-people).</span></span>  

## <a name="select-parameter"></a><span data-ttu-id="f15ab-255">parâmetro select</span><span class="sxs-lookup"><span data-stu-id="f15ab-255">select parameter</span></span>

<span data-ttu-id="f15ab-256">Use o parâmetro de consulta `$select` para retornar um conjunto de propriedades diferente do padrão definido para um recurso individual ou um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="f15ab-256">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="f15ab-257">Com $select, você pode especificar um subconjunto ou um superconjunto das propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="f15ab-257">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="f15ab-258">Por exemplo, ao recuperar as mensagens do usuário conectado, você pode especificar que somente as propriedades **from** e **subject** sejam retornadas:</span><span class="sxs-lookup"><span data-stu-id="f15ab-258">For example, when retrieving the messages of the signed-in user, you can specify that only the **from** and **subject** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="f15ab-259">[Experimentar no Explorador do Graph][select-example]</span><span class="sxs-lookup"><span data-stu-id="f15ab-259">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="f15ab-260">**Importante:** Em geral, recomendamos que você use `$select` para limitar as propriedades retornadas por uma consulta àqueles exigidas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f15ab-260">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="f15ab-261">Isso se aplica particularmente a consultas com o potencial de retornar um conjunto de resultados amplo.</span><span class="sxs-lookup"><span data-stu-id="f15ab-261">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="f15ab-262">Limitar as propriedades retornadas em cada linha reduzirá a carga de rede e ajudará a melhorar o desempenho do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f15ab-262">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="f15ab-p125">No `v1.0`, alguns recursos do Azure AD que derivam de [directoryObject](../api-reference/v1.0/resources/directoryobject.md), como [usuário](../api-reference/v1.0/resources/user.md) e [grupo](../api-reference/v1.0/resources/group.md), retornam um subconjunto limitado padrão de propriedades em leituras. Para esses recursos, você deve usar `$select` para retornar propriedades fora do conjunto padrão.</span><span class="sxs-lookup"><span data-stu-id="f15ab-p125">In `v1.0`, some Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="f15ab-265">parâmetro skip</span><span class="sxs-lookup"><span data-stu-id="f15ab-265">skip parameter</span></span>

<span data-ttu-id="f15ab-p126">Use o parâmetro de consulta `$skip` para definir o número de itens para ignorar no início de um conjunto. Por exemplo, a solicitação a seguir retorna eventos para o usuário classificadas por data de criação, começando com o evento 21 no conjunto:</span><span class="sxs-lookup"><span data-stu-id="f15ab-p126">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="f15ab-268">[Experimentar no Explorador do Graph][skip-example]</span><span class="sxs-lookup"><span data-stu-id="f15ab-268">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="f15ab-269">**Observação:** algumas APIs do Microsoft Graph, como Email e Calendário do Outlook (**message**, **event** e **calendar**), usam `$skip` para implementar a paginação.</span><span class="sxs-lookup"><span data-stu-id="f15ab-269">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (**message**, **event**, and **calendar**), use `$skip` to implement paging.</span></span> <span data-ttu-id="f15ab-270">Quando os resultados de uma consulta ocuparem várias páginas, essas APIs retornarão uma propriedade `@odata:nextLink` com uma URL que contém um parâmetro `$skip`.</span><span class="sxs-lookup"><span data-stu-id="f15ab-270">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="f15ab-271">Você pode usar essa URL para retornar a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="f15ab-271">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="f15ab-272">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="f15ab-272">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="f15ab-273">parâmetro skipToken</span><span class="sxs-lookup"><span data-stu-id="f15ab-273">skipToken parameter</span></span>

<span data-ttu-id="f15ab-p128">Algumas solicitações retornam várias páginas de dados devido à paginação do lado do servidor ou devido ao uso do parâmetro [`$top`](#top-parameter) para limitar o tamanho da página da resposta. Muitas APIs do Microsoft Graph usam o parâmetro de consulta `skipToken` para fazer referência a páginas subsequentes do resultado. O parâmetro `$skiptoken` contém um token opaco que faz referência à próxima página de resultados e é retornado na URL fornecida na propriedade `@odata.nextLink` na resposta. Para saber mais, confira [paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="f15ab-p128">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="f15ab-278">parâmetro top</span><span class="sxs-lookup"><span data-stu-id="f15ab-278">top parameter</span></span>

<span data-ttu-id="f15ab-279">Use o parâmetro de consulta `$top` para especificar o tamanho de página do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="f15ab-279">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="f15ab-280">Se restarem mais itens no conjunto de resultados, o corpo da resposta conterá um parâmetro `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="f15ab-280">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="f15ab-281">Esse parâmetro contém uma URL que você pode usar para obter a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="f15ab-281">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="f15ab-282">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="f15ab-282">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="f15ab-283">Por exemplo, a solicitação a seguir retorna as primeiras cinco mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="f15ab-283">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="f15ab-284">[Experimentar no Explorador do Graph][top-example]</span><span class="sxs-lookup"><span data-stu-id="f15ab-284">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="f15ab-285">Tratamento de erro para parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="f15ab-285">Error handling for query parameters</span></span>

<span data-ttu-id="f15ab-p130">Algumas solicitações retornarão uma mensagem de erro se não houver suporte para um parâmetro de consulta especificado. Por exemplo, você não pode usar `$expand` na relação `user/photo`.</span><span class="sxs-lookup"><span data-stu-id="f15ab-p130">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="f15ab-288">No entanto, é importante observar que os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente.</span><span class="sxs-lookup"><span data-stu-id="f15ab-288">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="f15ab-289">Isso pode ser verdadeiro para parâmetros de consulta sem suporte, bem como para combinações de parâmetros de consulta sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f15ab-289">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="f15ab-290">Nesses casos, você deve examinar os dados retornados pela solicitação para determinar se os parâmetros de consulta que especificou tiveram o efeito desejado.</span><span class="sxs-lookup"><span data-stu-id="f15ab-290">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0


