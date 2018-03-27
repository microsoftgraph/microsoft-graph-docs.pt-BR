# <a name="get-incremental-changes-for-groups"></a><span data-ttu-id="56126-101">Obter as alterações incrementais para grupos</span><span class="sxs-lookup"><span data-stu-id="56126-101">Get incremental changes for groups (preview)</span></span>

<span data-ttu-id="56126-p101">A [Consulta delta](./delta_query_overview.md) permite que você consulte adições, exclusões ou atualizações de grupos, por meio de uma série de chamadas de função [delta](../api-reference/v1.0/api/group_delta.md). A consulta Delta permite que você descubra alterações em grupos sem ter que buscar todo o conjunto de grupos do Microsoft Graph e comparar as alterações.</span><span class="sxs-lookup"><span data-stu-id="56126-p101">[Delta query](./delta_query_overview.md) lets you query for additions, deletions, or updates to groups, by way of a series of [delta](../api-reference/v1.0/api/group_delta.md) function calls. Delta query enables you discover changes to groups without having to fetch the entire set of groups from Microsoft Graph and compare changes.</span></span>

<span data-ttu-id="56126-p102">Clientes que sincronizam grupos com um repositório de perfil local, podem usar a Consulta Delta para a sincronização completa inicial juntamente com as sincronizações incrementais no futuro. Normalmente, um cliente faria uma sincronização completa inicial de todos os grupos em um locatário e, logo após, obteria alterações incrementais para esses grupos periodicamente.</span><span class="sxs-lookup"><span data-stu-id="56126-p102">Clients using synchronizing groups with a local profile store can use Delta Query for both their initial full synchronization along with incremental synchronizations in the future. Typically, a client would do an initial full synchronization of all the groups in a tenant, and subsequently, get incremental changes to groups periodically.</span></span> 

## <a name="tracking-group-changes"></a><span data-ttu-id="56126-106">Controle de alterações de grupo</span><span class="sxs-lookup"><span data-stu-id="56126-106">Tracking group changes</span></span>

<span data-ttu-id="56126-p103">O controle de alterações de grupo corresponde a uma série de uma ou mais solicitações GET com a função **delta**. Criar uma solicitação GET é muito parecido com a forma de [listar grupos](../api-reference/v1.0/api/group_list.md), exceto se você incluir o seguinte:</span><span class="sxs-lookup"><span data-stu-id="56126-p103">Tracking group changes is a round of one or more GET requests with the **delta** function. You make a GET request much like the way you [list groups](../api-reference/v1.0/api/group_list.md), except that you include the following:</span></span>

- <span data-ttu-id="56126-109">A função **delta**.</span><span class="sxs-lookup"><span data-stu-id="56126-109">The **delta** function.</span></span>
- <span data-ttu-id="56126-110">Um [token de estado](./delta_query_overview.md) (_deltaToken_ ou _skipToken_) da chamada de função GET **delta** anterior.</span><span class="sxs-lookup"><span data-stu-id="56126-110">A [state token](./delta_query_overview.md) (_deltaToken_ or _skipToken_) from the previous GET **delta** function call.</span></span>

## <a name="example"></a><span data-ttu-id="56126-111">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56126-111">Example</span></span>

<span data-ttu-id="56126-112">O exemplo a seguir mostra uma série de solicitações para rastrear as alterações nos grupos:</span><span class="sxs-lookup"><span data-stu-id="56126-112">The following example shows a series  requests to track changes to groups:</span></span>

1. <span data-ttu-id="56126-113">[Solicitação inicial](#initial-request) e [resposta](#initial-response)</span><span class="sxs-lookup"><span data-stu-id="56126-113">[Initial request](#initial-request) and [response](#initial-response)</span></span>
2. <span data-ttu-id="56126-114">[solicitação nextLink](#nextlink-request) e [resposta](#nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="56126-114">[nextLink request](#nextlink-request) and [response](#nextlink-response)</span></span>
3. <span data-ttu-id="56126-115">[Solicitação final nextLink](#final-nextlink-request) e [resposta](#final-nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="56126-115">[Final nextLink request](#final-nextlink-request) and [response](#final-nextlink-response)</span></span>
4. <span data-ttu-id="56126-116">[Solicitação deltaLink](#deltalink-request) e [resposta deltaLink](#deltalink-response)</span><span class="sxs-lookup"><span data-stu-id="56126-116">[deltaLink request](#deltalink-request) and [deltaLink response](#deltalink-response)</span></span>

## <a name="initial-request"></a><span data-ttu-id="56126-117">Solicitação inicial</span><span class="sxs-lookup"><span data-stu-id="56126-117">Initial request</span></span>

<span data-ttu-id="56126-118">Para iniciar o rastreamento de alterações no recurso de grupo, faça uma solicitação incluindo a função delta no recurso de grupo.</span><span class="sxs-lookup"><span data-stu-id="56126-118">To begin tracking changes in the group resource, you make a request including the delta function on the group resource.</span></span> 

<span data-ttu-id="56126-119">Observe o seguinte:</span><span class="sxs-lookup"><span data-stu-id="56126-119">Note the following:</span></span>

- <span data-ttu-id="56126-120">O parâmetro de consulta $select opcional está incluído na solicitação para demonstrar como os parâmetros de consulta são automaticamente incluídos nas futuras solicitações.</span><span class="sxs-lookup"><span data-stu-id="56126-120">The optional $select query parameter is included in the request to demonstrate how query parameters are automatically included in future requests.</span></span>
- <span data-ttu-id="56126-p104">A solicitação inicial não inclui um token de estado. Os tokens de estado serão usados nas solicitações subsequentes.</span><span class="sxs-lookup"><span data-stu-id="56126-p104">The initial request does not include a state token. State tokens will be used in subsequent requests.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description
```

## <a name="initial-response"></a><span data-ttu-id="56126-123">Resposta inicial</span><span class="sxs-lookup"><span data-stu-id="56126-123">Initial response</span></span>

<span data-ttu-id="56126-p105">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [group](../api-reference/v1.0/resources/group.md) no corpo da resposta. Pressupondo que todo o conjunto de grupos é muito grande, a resposta também incluirá um token de estado nextLink.</span><span class="sxs-lookup"><span data-stu-id="56126-p105">If successful, this method returns `200 OK` response code and [group](../api-reference/v1.0/resources/group.md) collection object in the response body. Assuming the entire set of groups is too large, the response will also include a nextLink state token.</span></span>

<span data-ttu-id="56126-p106">Neste exemplo, uma URL nextLink é retornada indicando que não há páginas adicionais de dados a serem recuperados na sessão. O parâmetro de consulta $select da solicitação inicial é codificado na URL nextLink.</span><span class="sxs-lookup"><span data-stu-id="56126-p106">In this example, a nextLink URL is returned indicating there are additional pages of data to be retrieved in the session. The $select query parameter from the initial request is encoded into the nextLink URL.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,description)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ",
  "value": [
    {
      "displayName":"TestGroup1",
      "description":"Employees in test group 1",
      "id":"c2f798fd-f95d-4623-8824-63aec21fffff"
    },
    {
      "displayName":"TestGroup2",
      "description":"Employees in test group 2",
      "id":"ec22655c-8eb2-432a-b4ea-8b8a254bffff"
    }
  ]
}
```

## <a name="nextlink-request"></a><span data-ttu-id="56126-128">solicitação nextLink</span><span class="sxs-lookup"><span data-stu-id="56126-128">nextLink request</span></span>

<span data-ttu-id="56126-p107">A segunda solicitação especifica o `skipToken` retornado da resposta anterior. Observe que o parâmetro `$select` não é obrigatório, pois o `skipToken` codifica e o inclui.</span><span class="sxs-lookup"><span data-stu-id="56126-p107">The second request specifies the `skipToken` returned from the previous response. Notice the `$select` parameter is not required, as the `skipToken` encodes and includes it.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ
```

## <a name="nextlink-response"></a><span data-ttu-id="56126-131">Resposta nextLink</span><span class="sxs-lookup"><span data-stu-id="56126-131">nextLink response</span></span>

<span data-ttu-id="56126-p108">A resposta contém um `nextLink` e outro `skipToken`, indicando que não há mais grupos disponíveis. Continue fazendo solicitações usando a URL nextLink até uma URL deltaLink ser retornada na resposta.</span><span class="sxs-lookup"><span data-stu-id="56126-p108">The response contains a `nextLink` and another `skipToken`, indicating there are more groups available. You continue making requests using the nextLink URL until a deltaLink URL is returned in the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"TestGroup3",
      "description":"Employees in test group 3",
      "id":"2e5807ce-58f3-4a94-9b37-ffff2e085957"
    },
    {
      "displayName":"TestGroup4",
      "description":"Employees in test group 4",
      "id":"421e797f-9406-4934-b778-4908421e3505"
    }
  ]
}
```

## <a name="final-nextlink-request"></a><span data-ttu-id="56126-134">Solicitação nextLink final</span><span class="sxs-lookup"><span data-stu-id="56126-134">Final nextLink request</span></span>

<span data-ttu-id="56126-135">A terceira solicitação continua a usar os últimos `skipToken` retornados da última solicitação de sincronização.</span><span class="sxs-lookup"><span data-stu-id="56126-135">The third request continues to use the latest `skipToken` returned from the last sync request.</span></span> 

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=ppqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a><span data-ttu-id="56126-136">Resposta nextLink final</span><span class="sxs-lookup"><span data-stu-id="56126-136">Final nextLink response</span></span>

<span data-ttu-id="56126-p109">Quando a URL deltaLink é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL deltaLink para se inteirar das alterações feitas no recurso. Salve o `deltaToken` e use-o na solicitação da URL para descobrir as alterações feitas nos grupos.</span><span class="sxs-lookup"><span data-stu-id="56126-p109">When the deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource. Save the `deltaToken` and use it in the request URL to discover changes to groups.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup5",
      "description":"Employees in test group 5",
      "id":"bed7f0d4-750e-4e7e-ffff-169002d06fc9"
    },
    {
      "displayName":"TestGroup6",
      "description":"Employees in test group 6",
      "id":"421e797f-9406-ffff-b778-4908421e3505"
    }
  ]
}
```

## <a name="deltalink-request"></a><span data-ttu-id="56126-140">Solicitação deltaLink</span><span class="sxs-lookup"><span data-stu-id="56126-140">deltaLink request</span></span>

<span data-ttu-id="56126-141">Usando o `deltaToken` da [última resposta](#final-nextlink-response), você poderá obter grupos alterados (ao ser adicionado, excluído ou atualizado) desde o último pedido.</span><span class="sxs-lookup"><span data-stu-id="56126-141">Using the `deltaToken` from the [last response](#final-nextlink-response), you will be able to get changed (by being added, deleted, or updated) groups since the last request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw
```

## <a name="deltalink-response"></a><span data-ttu-id="56126-142">Resposta deltaLink</span><span class="sxs-lookup"><span data-stu-id="56126-142">deltaLink response</span></span>

<span data-ttu-id="56126-143">Se não houve alterações, o mesmo `deltatoken` é retornado com nenhum resultado.</span><span class="sxs-lookup"><span data-stu-id="56126-143">If no changes have occurred, the same `deltatoken` is returned with no results.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": []
}
```

<span data-ttu-id="56126-144">Se houve, o mesmo `deltatoken` é retornado incluindo um conjunto de grupos alterados.</span><span class="sxs-lookup"><span data-stu-id="56126-144">If changes have occurred, the same `deltatoken` is returned including a collection of changed groups.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/groups/delta?$deltatoken=sZwAFZibx-LQOdZIo1hHhmmDhHzCY0Hs6snoIHJCSIfCHdqKdWNZ2VX3kErpyna9GygROwBk-rqWWMFxJC3pw",
  "value": [
    {
      "displayName":"TestGroup7",
      "description":"Employees in test group 7",
      "id":"f764235c-ffff-4843-a14a-1d8826967260"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="56126-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="56126-145">See also</span></span>
<span data-ttu-id="56126-146">Visão geral da [consulta delta do Microsoft Graph](../concepts/delta_query_overview.md).</span><span class="sxs-lookup"><span data-stu-id="56126-146">[Microsoft Graph delta query](../concepts/delta_query_overview.md) overview.</span></span>