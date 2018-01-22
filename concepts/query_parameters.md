# <a name="use-query-parameters-to-customize-responses"></a><span data-ttu-id="ffbf3-101">Usar parâmetros de consulta para personalizar respostas</span><span class="sxs-lookup"><span data-stu-id="ffbf3-101">Use query parameters to customize responses</span></span>

<span data-ttu-id="ffbf3-p101">O Microsoft Graph fornece parâmetros de consulta opcional que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta. Há suporte para os parâmetros de consulta a seguir.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p101">Microsoft Graph provides optional query parameters that you can use to specify and control the amount of data returned in a response. The following query parameters are supported.</span></span>

><span data-ttu-id="ffbf3-104">**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="ffbf3-104">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="ffbf3-105">Name</span><span class="sxs-lookup"><span data-stu-id="ffbf3-105">Name</span></span>                     | <span data-ttu-id="ffbf3-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffbf3-106">Description</span></span> | <span data-ttu-id="ffbf3-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ffbf3-107">Example</span></span>
|:-------------------------|:------------|:---------|
| [<span data-ttu-id="ffbf3-108">$count</span><span class="sxs-lookup"><span data-stu-id="ffbf3-108">$count</span></span>](#count-parameter)         | <span data-ttu-id="ffbf3-109">Recupera a contagem total de recursos correspondentes.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-109">Retrieves the total count of matching resources.</span></span> | [`/me/messages?$top=2&$count=true`][count-example]
| [<span data-ttu-id="ffbf3-110">$expand</span><span class="sxs-lookup"><span data-stu-id="ffbf3-110">$expand</span></span>](#expand-parameter)       | <span data-ttu-id="ffbf3-111">Recupera os recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-111">Retrieves related resources.</span></span>|[`/groups?$expand=members`][expand-example]
| [<span data-ttu-id="ffbf3-112">$filter</span><span class="sxs-lookup"><span data-stu-id="ffbf3-112">$filter</span></span>](#filter-parameter)       | <span data-ttu-id="ffbf3-113">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="ffbf3-113">Filters results (rows).</span></span>|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [<span data-ttu-id="ffbf3-114">$format</span><span class="sxs-lookup"><span data-stu-id="ffbf3-114">$format</span></span>](#format-parameter)       | <span data-ttu-id="ffbf3-115">Retorna os resultados no formato de mídia especificado.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-115">Returns the results in the specified media format.</span></span>|[`/users?$format=json`][format-example]
| [<span data-ttu-id="ffbf3-116">$orderby</span><span class="sxs-lookup"><span data-stu-id="ffbf3-116">$orderby</span></span>](#orderby-parameter)     | <span data-ttu-id="ffbf3-117">Ordena os resultados.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-117">Orders results.</span></span>|[`/users?$orderby=displayName desc`][orderby-example]
| [<span data-ttu-id="ffbf3-118">$search</span><span class="sxs-lookup"><span data-stu-id="ffbf3-118">$search</span></span>](#search-parameter)       | <span data-ttu-id="ffbf3-p102">Retorna os resultados com base nos critérios de pesquisa. Atualmente, com suporte em conjuntos de **mensagens** e **pessoa**.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p102">Returns results based on search criteria. Currently supported on **** and **** collections.</span></span>|[`/me/messages?$search=pizza`][search-example]
| [<span data-ttu-id="ffbf3-121">$select</span><span class="sxs-lookup"><span data-stu-id="ffbf3-121">$select</span></span>](#select-parameter)       | <span data-ttu-id="ffbf3-122">Filtra as propriedades (colunas).</span><span class="sxs-lookup"><span data-stu-id="ffbf3-122">Filters properties (columns).</span></span>|[`/users?$select=givenName,surname`][select-example]
| [<span data-ttu-id="ffbf3-123">$skip</span><span class="sxs-lookup"><span data-stu-id="ffbf3-123">$skip</span></span>](#skip-parameter)           | <span data-ttu-id="ffbf3-p103">Índices em um conjunto de resultados. Também usado por algumas APIs para implementar a paginação e pode ser usado com `$top` para paginar resultados manualmente.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p103">Indexes into a result set. Also used by some APIs to implement paging and can be used together with `$top` to manually page results.</span></span> | [`/me/messages?$skip=11`][skip-example]
| [<span data-ttu-id="ffbf3-126">$skipToken</span><span class="sxs-lookup"><span data-stu-id="ffbf3-126">$skipToken</span></span>](#skiptoken-parameter) | <span data-ttu-id="ffbf3-p104">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas. (Algumas APIs usam `$skip` em vez disso.)</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p104">Retrieves the next page of results from result sets that span multiple pages. (Some APIs use `$skip` instead.)</span></span> | `/users?$skiptoken=X%274453707402000100000017...`|
| [<span data-ttu-id="ffbf3-129">$top</span><span class="sxs-lookup"><span data-stu-id="ffbf3-129">$top</span></span>](#top-parameter)             | <span data-ttu-id="ffbf3-130">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-130">Sets the page size of results.</span></span> |[`/users?$top=2`][top-example]



<span data-ttu-id="ffbf3-131">Esses parâmetros são compatíveis com a [linguagem de consulta OData V4][odata-query].</span><span class="sxs-lookup"><span data-stu-id="ffbf3-131">These parameters are compatible with the [OData V4 query language][odata-query].</span></span> <span data-ttu-id="ffbf3-132">Nem todos os parâmetros têm suporte em todas as APIs do Microsoft Graph, e o suporte pode diferir significativamente entre os pontos de extremidade `v1.0` e `beta`.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-132">Not all parameters are supported across all Microsoft Graph APIs, and support might differ significantly between the `v1.0` and `beta` endpoints.</span></span> 

> <span data-ttu-id="ffbf3-p106">**Observação:** No ponto de extremidade `beta`, o prefixo `$` é opcional. Por exemplo, em vez de `$filter`, você pode usar `filter`. Para obter mais detalhes e exemplos, confira [Suporte a parâmetros da consulta sem prefixos $ no Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p106">**Note:** On the `beta` endpoint, the `$` prefix is optional. For example, instead of `$filter`, you can use `filter`. For more details and examples, see [Supporting query parameters without $ prefixes in Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).</span></span>

## <a name="encoding-query-parameters"></a><span data-ttu-id="ffbf3-136">Codificação de parâmetros da consulta</span><span class="sxs-lookup"><span data-stu-id="ffbf3-136">Encoding query parameters</span></span>

<span data-ttu-id="ffbf3-137">Os valores dos parâmetros da consulta devem ser codificados por porcentagem.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-137">The values of query parameters should be percent-encoded.</span></span> <span data-ttu-id="ffbf3-138">Muitas ferramentas, navegadores e clientes HTTP (como o [Explorador do Graph][graph-explorer]) ajudarão você com isso.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-138">Many HTTP clients, browsers, and tools (such as the [Graph Explorer][graph-explorer]) will help you with this.</span></span> <span data-ttu-id="ffbf3-139">Se uma consulta está falhando, uma causa possível é a falha na codificação adequada dos valores dos parâmetros da consulta.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-139">If a query is failing, one possible cause is failure to encode the query parameter values appropriately.</span></span>

<span data-ttu-id="ffbf3-140">Uma URL descodificada é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-140">An unencoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

<span data-ttu-id="ffbf3-141">Uma URL codificada adequadamente é semelhante a esta:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-141">A properly encoded URL looks like this:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count-parameter"></a><span data-ttu-id="ffbf3-142">parâmetro count</span><span class="sxs-lookup"><span data-stu-id="ffbf3-142">count parameter</span></span>

<span data-ttu-id="ffbf3-143">Use o parâmetro de consulta `$count` para incluir uma contagem do número total de itens em um conjunto, juntamente com a página de valores de dados retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-143">Use the `$count` query parameter to include a count of the total number of items in a collection alongside the page of data values returned from Microsoft Graph.</span></span> 

<span data-ttu-id="ffbf3-144">Por exemplo, a solicitação a seguir retornará o conjunto **contato** do usuário atual e o número de itens no conjunto **contato** na propriedade `@odata.count`.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-144">For example, the following request will return both the **** collection of the current user, and the number of items in the **** collection in the `@odata.count` property.</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[<span data-ttu-id="ffbf3-145">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="ffbf3-145">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


><span data-ttu-id="ffbf3-146">**Observação:** `$count` não tem suporte para conjuntos de recursos derivados de [directoryObject](../api-reference/v1.0/resources/directoryobject.md), como conjuntos de [usuários](../api-reference/v1.0/resources/user.md) ou [grupos](../api-reference/v1.0/resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="ffbf3-146">Note:  is not supported for collections of resources that derive from    like collections of users or groups.</span></span>

## <a name="expand-parameter"></a><span data-ttu-id="ffbf3-147">parâmetro expand</span><span class="sxs-lookup"><span data-stu-id="ffbf3-147">expand parameter</span></span>

<span data-ttu-id="ffbf3-148">Muitos recursos do Microsoft Graph expõem as propriedades declaradas do recurso, bem como as relações delas com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-148">Many Microsoft Graph resources expose both declared properties of the resource as well as its relationships with other resources.</span></span> <span data-ttu-id="ffbf3-149">Essas relações também são chamadas de propriedades de referência ou propriedades de navegação e podem fazer referência a um único recurso ou a um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-149">These relationships are also called reference properties or navigation properties, and they can reference either a single resource or a collection of resources.</span></span> <span data-ttu-id="ffbf3-150">Por exemplo, as pastas de email, gerente e subordinados diretos de um usuário são todas expostas como relações.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-150">For example, the mail folders, manager, and direct reports of a user are all exposed as relationships.</span></span> 

<span data-ttu-id="ffbf3-p109">Normalmente, você pode consultar as propriedades de um recurso ou uma de suas relações em uma única solicitação, mas não ambas. Você pode usar o parâmetro de cadeia de caracteres de consulta `$expand` para incluir o recurso expandido ou o conjunto referenciado por uma única relação (propriedade de navegação) nos resultados.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p109">Normally, you can query either the properties of a resource or one of its relationships in a single request, but not both. You can use the `$expand` query string parameter to include the expanded resource or collection referenced by a single relationship (navigation property) in your results.</span></span>

<span data-ttu-id="ffbf3-153">O seguinte exemplo obtém informações de unidade raiz juntamente com os itens filho de nível superior em uma unidade:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-153">The following example gets root drive information along with the top-level child items in a drive:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[<span data-ttu-id="ffbf3-154">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="ffbf3-154">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

<span data-ttu-id="ffbf3-p110">Com alguns conjuntos de recursos, você também pode especificar as propriedades a serem retornadas nos recursos expandidos adicionando um parâmetro `$select`. O exemplo a seguir executa a mesma consulta que o exemplo anterior, mas usa uma instrução [`$select`](#select-parameter) para limitar as propriedades retornadas para os itens filho expandidos para as propriedades **id** e **name**.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p110">With some resource collections, you can also specify the properties to be returned in the expanded resources by adding a `$select` parameter. The following example performs the same query as the previous example but uses a [`$select`](#select-parameter) statement to limit the properties returned for the expanded child items to the **** and **** properties.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

<span data-ttu-id="ffbf3-157">[Experimentar no Explorador do Graph][expand-example]</span><span class="sxs-lookup"><span data-stu-id="ffbf3-157">[Try in Graph Explorer][expand-example]</span></span>

> <span data-ttu-id="ffbf3-p111">**Observação:** nem todas as relações e recursos dão suporte ao parâmetro de consulta `$expand`. Por exemplo, você pode expandir as relações **directReports**, **manager** e **memberOf** em um usuário, mas não pode expandir suas relações **events**, **messages** ou **photo**. Nem todos os recursos ou relações dão suporte ao uso de `$select` em itens expandidos.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p111">**Note:** Not all relationships and resources support the `$expand` query parameter. For example, you can expand the ****, ****, and **** relationships on a user, but you cannot expand its ****, ****, or **** relationships. Not all resources or relationships support using `$select` on expanded items.</span></span> 
> 
> <span data-ttu-id="ffbf3-161">Com recursos do Azure AD derivados de [directoryObject](../api-reference/v1.0/resources/directoryobject.md), como [user](../api-reference/v1.0/resources/user.md) e [group](../api-reference/v1.0/resources/group.md), `$expand` só há suporte para `beta`, e normalmente são retornados no máximo 20 itens para a relação expandida.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-161">With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), `$expand` is only supported for `beta` and  typically returns a maximum of 20 items for the expanded relationship.</span></span>

## <a name="filter-parameter"></a><span data-ttu-id="ffbf3-162">parâmetro filter</span><span class="sxs-lookup"><span data-stu-id="ffbf3-162">filter parameter</span></span>

<span data-ttu-id="ffbf3-163">Use o parâmetro de consulta `$filter` para recuperar apenas um subconjunto de um conjunto.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-163">Use the `$filter` query parameter to retrieve just a subset of a collection.</span></span> 

<span data-ttu-id="ffbf3-164">Por exemplo, para localizar os usuários cujo nome de exibição se inicia com a letra "J", use `startswith`.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-164">For example, to find users whose display name starts with the letter 'J', use `startswith`.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

<span data-ttu-id="ffbf3-165">[Experimentar no Explorador do Graph][filter-example]</span><span class="sxs-lookup"><span data-stu-id="ffbf3-165">[Try in Graph Explorer][filter-example]</span></span>

<span data-ttu-id="ffbf3-166">O suporte para operadores `$filter` varia entre as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-166">Support for `$filter` operators varies across Microsoft Graph APIs.</span></span> <span data-ttu-id="ffbf3-167">Os seguintes operadores lógicos geralmente são suportados:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-167">The following logical operators are generally supported:</span></span> 

- <span data-ttu-id="ffbf3-168">igual a (`eq`)</span><span class="sxs-lookup"><span data-stu-id="ffbf3-168">equals (`eq`)</span></span>
- <span data-ttu-id="ffbf3-169">não é igual a (`ne`)</span><span class="sxs-lookup"><span data-stu-id="ffbf3-169">not equals (`ne`)</span></span>
- <span data-ttu-id="ffbf3-170">maior que (`gt`)</span><span class="sxs-lookup"><span data-stu-id="ffbf3-170">greater than (`gt`)</span></span>
- <span data-ttu-id="ffbf3-171">maior ou igual a (`ge`)</span><span class="sxs-lookup"><span data-stu-id="ffbf3-171">greater than or equals (`ge`)</span></span>
- <span data-ttu-id="ffbf3-172">menor que (`lt`), menor ou igual a (`le`)</span><span class="sxs-lookup"><span data-stu-id="ffbf3-172">less than (`lt`), less than or equals (`le`)</span></span>
- <span data-ttu-id="ffbf3-173">e (`and`)</span><span class="sxs-lookup"><span data-stu-id="ffbf3-173">and (`and`)</span></span>
- <span data-ttu-id="ffbf3-174">ou (`or`)</span><span class="sxs-lookup"><span data-stu-id="ffbf3-174">or (`or`)</span></span>
- <span data-ttu-id="ffbf3-175">não (`not`)</span><span class="sxs-lookup"><span data-stu-id="ffbf3-175">not (`not`)</span></span>
 
<span data-ttu-id="ffbf3-176">O operador de cadeia de caracteres `startswith` geralmente é suportado.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-176">The `startswith` string operator is often supported.</span></span> <span data-ttu-id="ffbf3-177">O operador lambda `any` tem suporte em algumas APIs.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-177">The `any` lambda operator is supported for some APIs.</span></span> <span data-ttu-id="ffbf3-178">Para ver alguns exemplos de uso, confira a tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-178">For some  usage examples, see the following table.</span></span> <span data-ttu-id="ffbf3-179">Para obter mais detalhes sobre a sintaxe `$filter`, confira o [protocolo OData][odata-filter].</span><span class="sxs-lookup"><span data-stu-id="ffbf3-179">For more details about `$filter` syntax, see the [OData protocol][odata-filter].</span></span>  

<span data-ttu-id="ffbf3-180">A tabela a seguir mostra alguns exemplos que usam o parâmetro de consulta `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-180">The following table shows some examples that use the `$filter` query parameter.</span></span>

> <span data-ttu-id="ffbf3-181">**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].</span><span class="sxs-lookup"><span data-stu-id="ffbf3-181">**Note:** Click the examples to try them in [Graph Explorer][graph-explorer].</span></span>

| <span data-ttu-id="ffbf3-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffbf3-182">Description</span></span> | <span data-ttu-id="ffbf3-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ffbf3-183">Example</span></span>
|:------------|:--------|
| <span data-ttu-id="ffbf3-184">Pesquisar por usuários com o nome Clara entre várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-184">Search for users with the name Mary across multiple properties.</span></span> | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| <span data-ttu-id="ffbf3-185">Obter todos os eventos do usuário conectado que começaram após 01/07/2017.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-185">Get all the signed-in user's events that start after 7/1/2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| <span data-ttu-id="ffbf3-186">Obter todos os emails de um endereço específico recebidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-186">Get all emails from a specific address received by the signed-in user.</span></span> | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| <span data-ttu-id="ffbf3-187">Obter todos os emails recebidos pelo usuário conectado em abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-187">Get all emails received by the signed-in user in April 2017.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| <span data-ttu-id="ffbf3-188">Obter todos os emails não lidos na caixa de entrada do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-188">Get all unread mail in the signed-in user's Inbox.</span></span> | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| <span data-ttu-id="ffbf3-189">Listar todos os grupos do Office 365 em uma organização.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-189">List all Office 365 groups in an organization.</span></span> | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> <span data-ttu-id="ffbf3-p114">**Observação:** Os seguintes operadores `$filter` não têm suporte para recursos do Azure AD: `ne`, `gt`, `ge`, `lt`, `le` e `not`. O operador de cadeia de caracteres `contains` atualmente não tem suporte em nenhum recurso do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p114">**Note:** The following `$filter` operators are not supported for Azure AD resources:  `ne`, `gt`, `ge`, `lt`, `le`, and `not`. The `contains` string operator is currently not supported on any Microsoft Graph resources.</span></span>

## <a name="format-parameter"></a><span data-ttu-id="ffbf3-192">parâmetro format</span><span class="sxs-lookup"><span data-stu-id="ffbf3-192">format parameter</span></span>

<span data-ttu-id="ffbf3-193">Use o parâmetro de consulta `$format` para especificar o formato de mídia dos itens retornados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-193">Use the `$format` query parameter to specify the media format of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="ffbf3-194">Por exemplo, a seguinte solicitação retorna os usuários na organização no formato json:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-194">For example, the following request returns the users in the organization in the json format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

<span data-ttu-id="ffbf3-195">[Experimentar no Explorador do Graph][format-example]</span><span class="sxs-lookup"><span data-stu-id="ffbf3-195">[Try in Graph Explorer][format-example]</span></span>

> <span data-ttu-id="ffbf3-196">**Observação:** o parâmetro de consulta `$format` é compatível com vários formatos (por exemplo, atom, xml e json), mas os resultados podem não ser retornados em todos os formatos.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-196">**Note:** The `$format` query parameter supports a number of formats (for example, atom, xml, and json) but results may not be returned in all formats.</span></span>

## <a name="orderby-parameter"></a><span data-ttu-id="ffbf3-197">parâmetro orderby</span><span class="sxs-lookup"><span data-stu-id="ffbf3-197">orderby parameter</span></span>

<span data-ttu-id="ffbf3-198">Use o parâmetro de consulta `$orderby` para especificar a ordem de classificação dos itens retornados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-198">Use the `$orderby` query parameter to specify the sort order of the items returned from Microsoft Graph.</span></span>

<span data-ttu-id="ffbf3-199">Por exemplo, a solicitação a seguir retorna os usuários da organização ordenados por seu nome de exibição:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-199">For example, the following request returns the users in the organization ordered by their display name:</span></span>

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
<span data-ttu-id="ffbf3-200">[Experimentar no Explorador do Graph][orderby-example]</span><span class="sxs-lookup"><span data-stu-id="ffbf3-200">[Try in Graph Explorer][orderby-example]</span></span>

<span data-ttu-id="ffbf3-p115">Você também pode classificar por entidades de tipo complexo. A solicitação abaixo obtém mensagens e as classifica pelo campo **address** da propriedade **from**, que é do tipo complexo **emailAddress**:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p115">You can also sort by complex type entities. The following example gets messages and sorts them by the **address** field of the **from** property, which is of the complex type **emailAddress**:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[<span data-ttu-id="ffbf3-203">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="ffbf3-203">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

<span data-ttu-id="ffbf3-204">Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-204">To sort the results in ascending or descending order, append either `asc` or `desc` to the field name, separated by a space; for example, `?$orderby=name%20desc`.</span></span>

<span data-ttu-id="ffbf3-205">Com algumas APIs, você pode ordenar os resultados em várias propriedades.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-205">With some APIs, you can order results on multiple properties.</span></span> <span data-ttu-id="ffbf3-206">Por exemplo, a solicitação a seguir ordena as mensagens na caixa de entrada do usuário primeiro pelo nome da pessoa que enviou, em ordem decrescente (Z – A) e, em seguida, por assunto, em ordem ascendente (padrão).</span><span class="sxs-lookup"><span data-stu-id="ffbf3-206">For example, the following request orders the messages in the user's Inbox, first by the name of the person who sent it in descending order (Z to A), and then by subject in ascending order (default).</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[<span data-ttu-id="ffbf3-207">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="ffbf3-207">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

<span data-ttu-id="ffbf3-208">Quando você especifica $filter, servidor deduz uma ordem de classificação para os resultados.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-208">When you specify $filter the server will infer a sort order for the results.</span></span> <span data-ttu-id="ffbf3-209">Se você usar `$orderby` e `$filter`, como o servidor sempre deduz a ordem de classificação dos resultados de um `$filter`, as propriedades do `$filter` devem estar listadas primeiro no `$orderby` antes de outras propriedades e devem estar listadas na ordem que aparecem no parâmetro `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-209">If you use both `$orderby` and `$filter`, because the server always infers a sort order for the results of a `$filter`, the properties in the `$filter` must be listed first in the `$orderby` before any other properties, and they must be listed in the order that they appear in the `$filter` parameter.</span></span> 

<span data-ttu-id="ffbf3-210">O exemplo a seguir mostra uma consulta filtrada pelas propriedades **subject** e **priority** e classificadas pelas propriedades **subject**, **priority** e **receivedDateTime** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-210">The following example shows a query filtered by the **subject** and **importance** properties, and then sorted by the **subject**, **importance**, and **receivedDateTime** properties in descending order.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome to exchange unified messaging' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[<span data-ttu-id="ffbf3-211">Experimentar no Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="ffbf3-211">Try in Graph Explorer</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome to exchange unified messaging%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > <span data-ttu-id="ffbf3-212">**Observação:** Com os recursos do Azure AD derivados de [directoryObject](../api-reference/v1.0/resources/directoryobject.md), como [user](../api-reference/v1.0/resources/user.md) e [group](../api-reference/v1.0/resources/group.md), você não pode combinar `$orderby` a expressões `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-212">**Note:** With Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), you cannot combine `$orderby` with `$filter` expressions.</span></span> 

## <a name="search-parameter"></a><span data-ttu-id="ffbf3-213">parâmetro search</span><span class="sxs-lookup"><span data-stu-id="ffbf3-213">search parameter</span></span>

<span data-ttu-id="ffbf3-214">Use o parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-214">Use the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

> <span data-ttu-id="ffbf3-p118">**Observação:** Atualmente, é possível pesquisar **somente** coleções de [mensagens](../api-reference/v1.0/resources/message.md) e [pessoas](../api-reference/v1.0/resources/person.md). Uma solicitação de `$search` retorna até 250 resultados. Não é possível usar [`$filter`](#filter-parameter) ou [`$orderby`](#orderby-parameter) em uma solicitação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p118">**Note:** You can currently search **only** [message](../api-reference/v1.0/resources/message.md) and [person](../api-reference/v1.0/resources/person.md) collections. A `$search` request returns up to 250 results. You cannot use [`$filter`](#filter-parameter) or [`$orderby`](#orderby-parameter) in a search request.</span></span>

### <a name="using-search-on-message-collections"></a><span data-ttu-id="ffbf3-218">Usando $search em conjuntos de mensagens</span><span class="sxs-lookup"><span data-stu-id="ffbf3-218">Using $search on  collections</span></span>

<span data-ttu-id="ffbf3-219">Aplicativos do Office 365, como Outlook e SharePoint, oferecem suporte à sintaxe da Linguagem de Consulta de Palavra-Chave (KQL) para fazer pesquisas.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-219">Office 365 applications, such as Outlook and SharePoint, support the Keyword Query Language (KQL) syntax to do searches.</span></span> <span data-ttu-id="ffbf3-220">Isso oferece a comodidade de um domínio de descoberta comum para os repositórios de dados.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-220">This provides the convenience of a common discovery domain for their data stores.</span></span> 

<span data-ttu-id="ffbf3-221">Quando você pesquisa conjuntos de mensagens, os resultados são classificados pela data e hora em que a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-221">When you search message collections, the results are sorted by the date and time that the message was sent.</span></span> 

<span data-ttu-id="ffbf3-222">Você pode especificar as seguintes propriedades em uma **message** em um critério `$search`: </span><span class="sxs-lookup"><span data-stu-id="ffbf3-222">You can specify the following properties on a **** in a `$search` criterion:</span></span>

- <span data-ttu-id="ffbf3-223">**attachments**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-223">**attachments**</span></span>
- <span data-ttu-id="ffbf3-224">**bccRecipients**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-224">**bccRecipients**</span></span>
- <span data-ttu-id="ffbf3-225">**body**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-225">**body**</span></span>
- <span data-ttu-id="ffbf3-226">**category**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-226">**Category**</span></span>
- <span data-ttu-id="ffbf3-227">**ccRecipients**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-227">**ccRecipients**</span></span>
- <span data-ttu-id="ffbf3-228">**content**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-228">**content**</span></span>
- <span data-ttu-id="ffbf3-229">**from**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-229">**from**</span></span>
- <span data-ttu-id="ffbf3-230">**hasAttachments**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-230">**hasAttachments**</span></span>
- <span data-ttu-id="ffbf3-231">**participants**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-231">**participants**</span></span>
- <span data-ttu-id="ffbf3-232">**receivedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-232">**receivedDateTime**</span></span>
- <span data-ttu-id="ffbf3-233">**sender**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-233">**sender**</span></span>
- <span data-ttu-id="ffbf3-234">**subject**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-234">**subject**</span></span>
- <span data-ttu-id="ffbf3-235">**toRecipients**</span><span class="sxs-lookup"><span data-stu-id="ffbf3-235">**toRecipients**</span></span>

<span data-ttu-id="ffbf3-236">Se você realizar uma pesquisa em mensagens e especificar apenas um valor, a pesquisa será realizada nas propriedades de pesquisa padrão **from**, **subject** e **body**.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-236">If you do a search on messages and specify only a value, the search is carried out on the default search properties of **from**, **subject** and **body**.</span></span>

<span data-ttu-id="ffbf3-237">O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-237">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="ffbf3-238">[Experimentar no Explorador do Graph][search-example]</span><span class="sxs-lookup"><span data-stu-id="ffbf3-238">[Try in Graph Explorer][search-example]</span></span>

<span data-ttu-id="ffbf3-239">O próximo exemplo procura todas as mensagens na Caixa de Entrada do usuário que foram enviadas de um endereço de email específico:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-239">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```
<span data-ttu-id="ffbf3-240">Para saber mais sobre a KQL como a sintaxe, operadores com suporte e dicas de pesquisa, confira os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-240">For more information about KQL such as the syntax, supported operators, and tips on searching, see the following articles:</span></span>

- [<span data-ttu-id="ffbf3-241">Referência de sintaxe da Linguagem de Consulta de Palavra-chave (KQL)</span><span class="sxs-lookup"><span data-stu-id="ffbf3-241">Keyword Query Language (KQL) syntax reference</span></span>](https://docs.microsoft.com/pt-BR/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- <span data-ttu-id="ffbf3-242">
  [Propriedades da mensagem e operadores de pesquisa para a Descoberta eletrônica In-loco no Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span><span class="sxs-lookup"><span data-stu-id="ffbf3-242">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)</span></span>

### <a name="using-search-on-person-collections"></a><span data-ttu-id="ffbf3-243">Usando $search em conjuntos de pessoas</span><span class="sxs-lookup"><span data-stu-id="ffbf3-243">Using $search on  collections</span></span>

<span data-ttu-id="ffbf3-p120">Você pode usar a API de Pessoas do Microsoft Graph para recuperar as pessoas mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. A API de Pessoas dá suporte ao parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p120">You can use the Microsoft Graph People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. The People API supports the `$search` query parameter.</span></span>

<span data-ttu-id="ffbf3-247">As pesquisas de pessoas ocorrem nas propriedades **displayName** and **emailAddress** do recurso [person](../api-reference/v1.0/resources/person.md).</span><span class="sxs-lookup"><span data-stu-id="ffbf3-247">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](../api-reference/v1.0/resources/person.md) resource.</span></span> <span data-ttu-id="ffbf3-248">As pesquisas implementam um algoritmo de correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-248">Searches implement a fuzzy matching algorithm.</span></span> <span data-ttu-id="ffbf3-249">Retornarão resultados com base em uma correspondência exata e também em Inferências sobre a intenção da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-249">They will return results based on an exact match and also on inferences about the intent of the search.</span></span> <span data-ttu-id="ffbf3-250">Por exemplo, imagine que um usuário com o nome de exibição "Carlos Lima" e o endereço de email carloslim@example.com que esteja no conjunto **pessoas** do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-250">For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="ffbf3-251">Todas as pesquisas a seguintes retornarão resultados que contêm Carlos.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-251">All of the following searches will return results that contain Tyler.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

<span data-ttu-id="ffbf3-p122">Você também pode executar pesquisas de pessoas que estão interessadas em determinado tópico. As pesquisas são executadas com base nas inferências derivadas das conversas de email do usuário. Por exemplo, a pesquisa a seguir retornará um conjunto de pessoas relevantes para o usuário conectado que tenham expressado interesse por pizza nas comunicações com o usuário. Observe que a frase de pesquisa está entre aspas.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p122">You can also perform searches for people who are interested in a particular topic. Searches are performed based on inferences derived from the user's mail conversations. For example, the following search will return a collection of people relevant to the signed-in user who have expressed an interest in pizza in communications with that user. Note that the search phrase is enclosed in quotes.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

<span data-ttu-id="ffbf3-256">Finalmente, você pode combinar pesquisas de pessoas e pesquisas de tópicos na mesma solicitação combinando os dois tipos de expressão de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-256">Finally, you can combine both people searches and topic searches in the same request by combining the two types of search expression.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```

<span data-ttu-id="ffbf3-257">Essa solicitação realiza basicamente duas pesquisas: uma pesquisa difusa em relação às propriedades **displayName** e **emailAddress** de pessoas relevantes ao usuário conectado e uma pesquisa pontual por "pizza" em relação às pessoas relevantes ao usuário.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-257">This request essentially conducts two searches: a fuzzy search against **** and **** properties of the signed-in user's relevant people, and a topic search for "pizza" against the user's relevant people.</span></span> <span data-ttu-id="ffbf3-258">Os resultados são classificados, ordenados e retornados.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-258">The results are then ranked, ordered, and returned.</span></span> <span data-ttu-id="ffbf3-259">A pesquisa não é restritiva. Você pode obter resultados que contenham pessoas com correspondência difusa "car", que estejam interessadas em "pizza" ou ambos.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-259">Note that the search is not restrictive; you might get results that contain people that fuzzy match "tyl", or that are interested in "pizza", or both.</span></span>

<span data-ttu-id="ffbf3-260">Para saber mais sobre a API de Pessoas, confira [Obter informações sobre pessoas relevantes](./people_example.md).</span><span class="sxs-lookup"><span data-stu-id="ffbf3-260">To learn more about the People API, see [Get information about relevant people](./people_example.md).</span></span>  

## <a name="select-parameter"></a><span data-ttu-id="ffbf3-261">parâmetro select</span><span class="sxs-lookup"><span data-stu-id="ffbf3-261">select parameter</span></span>

<span data-ttu-id="ffbf3-262">Use o parâmetro de consulta `$select` para retornar um conjunto de propriedades diferente do padrão definido para um recurso individual ou um conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-262">Use the `$select` query parameter to return a set of properties that are different than the default set for an individual resource or a collection of resources.</span></span> <span data-ttu-id="ffbf3-263">Com $select, você pode especificar um subconjunto ou um superconjunto das propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-263">With $select, you can specify a subset or a superset of the default properties.</span></span>

<span data-ttu-id="ffbf3-264">Por exemplo, ao recuperar as mensagens do usuário conectado, você pode especificar que somente as propriedades **from** e **subject** sejam retornadas:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-264">For example, when retrieving the messages of the signed-in user, you can specify that only the **** and **** properties be returned:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<span data-ttu-id="ffbf3-265">[Experimentar no Explorador do Graph][select-example]</span><span class="sxs-lookup"><span data-stu-id="ffbf3-265">[Try in Graph Explorer][select-example]</span></span>

> <span data-ttu-id="ffbf3-266">**Importante:** Em geral, recomendamos que você use `$select` para limitar as propriedades retornadas por uma consulta àqueles exigidas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-266">**Important:** In general, we recommend that you use `$select` to limit the properties returned by a query to those needed by your app.</span></span> <span data-ttu-id="ffbf3-267">Isso se aplica particularmente a consultas com o potencial de retornar um conjunto de resultados amplo.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-267">This is especially true of queries that might potentially return a large result set.</span></span> <span data-ttu-id="ffbf3-268">Limitar as propriedades retornadas em cada linha reduzirá a carga de rede e ajudará a melhorar o desempenho do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-268">Limiting the properties returned in each row will reduce network load and help improve your app's performance.</span></span>
>
> <span data-ttu-id="ffbf3-p126">No `v1.0`, alguns recursos do Azure AD que derivam de [directoryObject](../api-reference/v1.0/resources/directoryobject.md), como [usuário](../api-reference/v1.0/resources/user.md) e [grupo](../api-reference/v1.0/resources/group.md), retornam um subconjunto limitado padrão de propriedades em leituras. Para esses recursos, você deve usar `$select` para retornar propriedades fora do conjunto padrão.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p126">In `v1.0`, some Azure AD resources that derive from [directoryObject](../api-reference/v1.0/resources/directoryobject.md), like [user](../api-reference/v1.0/resources/user.md) and [group](../api-reference/v1.0/resources/group.md), return a limited, default subset of properties on reads. For these resources, you must use `$select` to return properties outside of the default set.</span></span>  

## <a name="skip-parameter"></a><span data-ttu-id="ffbf3-271">parâmetro skip</span><span class="sxs-lookup"><span data-stu-id="ffbf3-271">skip parameter</span></span>

<span data-ttu-id="ffbf3-p127">Use o parâmetro de consulta `$skip` para definir o número de itens para ignorar no início de um conjunto. Por exemplo, a solicitação a seguir retorna eventos para o usuário classificadas por data de criação, começando com o evento 21 no conjunto:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p127">Use the `$skip` query parameter to set the number of items to skip at the start of a collection. For example, the following request returns events for the user sorted by date created, starting with the 21st event in the collection:</span></span>

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
<span data-ttu-id="ffbf3-274">[Experimentar no Explorador do Graph][skip-example]</span><span class="sxs-lookup"><span data-stu-id="ffbf3-274">[Try in Graph Explorer][skip-example]</span></span>

> <span data-ttu-id="ffbf3-275">**Observação:** algumas APIs do Microsoft Graph, como Email e Calendário do Outlook (**message**, **event** e **calendar**), usam `$skip` para implementar a paginação.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-275">**Note:** Some Microsoft Graph APIs, like Outlook Mail and Calendars (****, ****, and ****), use `$skip` to implement paging.</span></span> <span data-ttu-id="ffbf3-276">Quando os resultados de uma consulta ocuparem várias páginas, essas APIs retornarão uma propriedade `@odata:nextLink` com uma URL que contém um parâmetro `$skip`.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-276">When results of a query span multiple pages, these APIs will return an `@odata:nextLink` property with a URL that contains a `$skip` parameter.</span></span> <span data-ttu-id="ffbf3-277">Você pode usar essa URL para retornar a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-277">You can use this URL to return the next page of results.</span></span> <span data-ttu-id="ffbf3-278">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="ffbf3-278">To learn more, see [Paging](./paging.md).</span></span>

## <a name="skiptoken-parameter"></a><span data-ttu-id="ffbf3-279">parâmetro skipToken</span><span class="sxs-lookup"><span data-stu-id="ffbf3-279">skipToken parameter</span></span>

<span data-ttu-id="ffbf3-p129">Algumas solicitações retornam várias páginas de dados devido à paginação do lado do servidor ou devido ao uso do parâmetro [`$top`](#top-parameter) para limitar o tamanho da página da resposta. Muitas APIs do Microsoft Graph usam o parâmetro de consulta `skipToken` para fazer referência a páginas subsequentes do resultado. O parâmetro `$skiptoken` contém um token opaco que faz referência à próxima página de resultados e é retornado na URL fornecida na propriedade `@odata.nextLink` na resposta. Para saber mais, confira [paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p129">Some requests return multiple pages of data either due to server-side paging or due to the use of the [`$top`](#top-parameter) parameter to limit the page size of the response. Many Microsoft Graph APIs use the `skipToken` query parameter to reference subsequent pages of the result. The `$skiptoken` parameter contains an opaque token that references the next page of results and is returned in the URL provided in the `@odata.nextLink` property in the response. To learn more, see [Paging](./paging.md).</span></span>


## <a name="top-parameter"></a><span data-ttu-id="ffbf3-284">parâmetro top</span><span class="sxs-lookup"><span data-stu-id="ffbf3-284">top parameter</span></span>

<span data-ttu-id="ffbf3-285">Use o parâmetro de consulta `$top` para especificar o tamanho de página do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-285">Use the `$top` query parameter to specify the page size of the result set.</span></span> 

<span data-ttu-id="ffbf3-286">Se restarem mais itens no conjunto de resultados, o corpo da resposta conterá um parâmetro `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-286">If more items remain in the result set, the response body will contain an `@odata.nextLink` parameter.</span></span> <span data-ttu-id="ffbf3-287">Esse parâmetro contém uma URL que você pode usar para obter a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-287">This parameter contains a URL that you can use to get the next page of results.</span></span> <span data-ttu-id="ffbf3-288">Para saber mais, confira [Paginação](./paging.md).</span><span class="sxs-lookup"><span data-stu-id="ffbf3-288">To learn more, see [Paging](./paging.md).</span></span> 

<span data-ttu-id="ffbf3-289">Por exemplo, a solicitação a seguir retorna as primeiras cinco mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="ffbf3-289">For example, the following request returns the first five messages in the user's mailbox:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<span data-ttu-id="ffbf3-290">[Experimentar no Explorador do Graph][top-example]</span><span class="sxs-lookup"><span data-stu-id="ffbf3-290">[Try in Graph Explorer][top-example]</span></span>


## <a name="error-handling-for-query-parameters"></a><span data-ttu-id="ffbf3-291">Tratamento de erro para parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="ffbf3-291">Error handling for query parameters</span></span>

<span data-ttu-id="ffbf3-p131">Algumas solicitações retornarão uma mensagem de erro se não houver suporte para um parâmetro de consulta especificado. Por exemplo, você não pode usar `$expand` na relação `user/photo`.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-p131">Some requests will return an error message if a specified query parameter is not supported. For example, you cannot use `$expand` on the `user/photo` relationship.</span></span> 

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

<span data-ttu-id="ffbf3-294">No entanto, é importante observar que os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-294">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="ffbf3-295">Isso pode ser verdadeiro para parâmetros de consulta sem suporte, bem como para combinações de parâmetros de consulta sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-295">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="ffbf3-296">Nesses casos, você deve examinar os dados retornados pela solicitação para determinar se os parâmetros de consulta que especificou tiveram o efeito desejado.</span><span class="sxs-lookup"><span data-stu-id="ffbf3-296">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> 

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


