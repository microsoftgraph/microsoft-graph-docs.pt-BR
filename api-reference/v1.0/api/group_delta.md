# <a name="group-delta"></a><span data-ttu-id="f66d4-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="f66d4-101">group: delta</span></span>

<span data-ttu-id="f66d4-p101">A [consulta delta](../../../concepts/delta_query_overview.md) permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Para descobrir as alterações nos grupos, realize uma solicitação usando a função *delta*. Confira [Usando a Consulta Delta](../../../concepts/delta_query_overview.md) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="f66d4-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to groups, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f66d4-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f66d4-105">Prerequisites</span></span>

<span data-ttu-id="f66d4-106">Um dos seguintes **escopos** é obrigatório para executar esta API: *Group.Read.All* ou *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="f66d4-106">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="f66d4-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f66d4-107">HTTP request</span></span>

<span data-ttu-id="f66d4-108">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de grupos.</span><span class="sxs-lookup"><span data-stu-id="f66d4-108">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

### <a name="query-parameters"></a><span data-ttu-id="f66d4-109">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="f66d4-109">Query parameters</span></span>

<span data-ttu-id="f66d4-p102">O controle de alterações em grupos corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="f66d4-p102">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="f66d4-115">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="f66d4-115">Query parameter</span></span>      | <span data-ttu-id="f66d4-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="f66d4-116">Type</span></span>   |<span data-ttu-id="f66d4-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f66d4-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f66d4-118">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="f66d4-118">$deltatoken</span></span> | <span data-ttu-id="f66d4-119">string</span><span class="sxs-lookup"><span data-stu-id="f66d4-119">string</span></span> | <span data-ttu-id="f66d4-p103">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de grupos indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="f66d4-p103">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="f66d4-122">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="f66d4-122">$skiptoken</span></span> | <span data-ttu-id="f66d4-123">string</span><span class="sxs-lookup"><span data-stu-id="f66d4-123">string</span></span> | <span data-ttu-id="f66d4-124">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de grupos.</span><span class="sxs-lookup"><span data-stu-id="f66d4-124">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="f66d4-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f66d4-125">Optional query parameters</span></span>

<span data-ttu-id="f66d4-126">Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f66d4-126">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="f66d4-p104">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="f66d4-p104">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="f66d4-129">Suporte à consulta delta `$select`, `$top` e `$expand` para grupos.</span><span class="sxs-lookup"><span data-stu-id="f66d4-129">Delta query support `$select`, `$top`, and `$expand` for groups.</span></span> 
- <span data-ttu-id="f66d4-p105">Há suporte limitado para `$orderby`: A única expressão `$orderby` suportada é `$orderby=receivedDateTime+desc`. Se você não incluir uma expressão `$orderby`, a ordem de retorno não será garantida.</span><span class="sxs-lookup"><span data-stu-id="f66d4-p105">There is limited support for `$orderby`: The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="f66d4-132">Não há suporte DAV para `$search`.</span><span class="sxs-lookup"><span data-stu-id="f66d4-132">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f66d4-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f66d4-133">Request headers</span></span>
| <span data-ttu-id="f66d4-134">Nome</span><span class="sxs-lookup"><span data-stu-id="f66d4-134">Name</span></span>       | <span data-ttu-id="f66d4-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="f66d4-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f66d4-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="f66d4-136">Authorization</span></span>  | <span data-ttu-id="f66d4-137">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="f66d4-137">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="f66d4-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f66d4-138">Content-Type</span></span>  | <span data-ttu-id="f66d4-139">application/json</span><span class="sxs-lookup"><span data-stu-id="f66d4-139">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f66d4-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f66d4-140">Request body</span></span>
<span data-ttu-id="f66d4-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f66d4-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f66d4-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f66d4-142">Response</span></span>

<span data-ttu-id="f66d4-p106">Se bem-sucedido, este método retorna o código de resposta `200, OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta. A resposta também inclui um token de estado que é uma URL nextLink ou uma URL deltaLink.</span><span class="sxs-lookup"><span data-stu-id="f66d4-p106">If successful, this method returns `200, OK` response code and [group](../resources/group.md) collection object in the response body. The response also includes a state token which is either a nextLink URL or a deltaLink URL.</span></span>

- <span data-ttu-id="f66d4-p107">Se uma URL nextLink é retornada, existem páginas de dado adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL nextLink até uma URL deltaLink ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="f66d4-p107">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="f66d4-p108">Se uma URL deltaLink for retornada, não haverá mais dados sobre o estado existente do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL deltaLink para se inteirar das alterações feitas no recurso.</span><span class="sxs-lookup"><span data-stu-id="f66d4-p108">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="f66d4-149">Confira:</span><span class="sxs-lookup"><span data-stu-id="f66d4-149">See:</span></span></br>
- <span data-ttu-id="f66d4-150">[Usando a Consulta Delta](../../../concepts/delta_query_overview.md) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="f66d4-150">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="f66d4-151">[Obter as alterações incrementais para grupos](../../../concepts/delta_query_groups.md) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="f66d4-151">[Get incremental changes for groups](../../../concepts/delta_query_groups.md) for an example requests.</span></span></br>
    
## <a name="example"></a><span data-ttu-id="f66d4-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f66d4-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f66d4-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f66d4-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

##### <a name="response"></a><span data-ttu-id="f66d4-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f66d4-154">Response</span></span>
<span data-ttu-id="f66d4-p109">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f66d4-p109">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->