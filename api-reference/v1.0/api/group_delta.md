# <a name="group-delta"></a><span data-ttu-id="01dd3-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="01dd3-101">group: delta</span></span>
<span data-ttu-id="01dd3-p101">A [consulta delta](../../../concepts/delta_query_overview.md) permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Para descobrir as alterações nos grupos, realize uma solicitação usando a função *delta*. Confira [Usando a Consulta Delta](../../../concepts/delta_query_overview.md) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="01dd3-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to groups, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="01dd3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="01dd3-105">Permissions</span></span>
<span data-ttu-id="01dd3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01dd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01dd3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01dd3-108">Permission type</span></span>      | <span data-ttu-id="01dd3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01dd3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01dd3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01dd3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="01dd3-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01dd3-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="01dd3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01dd3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01dd3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01dd3-113">Not supported.</span></span>    |
|<span data-ttu-id="01dd3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01dd3-114">Application</span></span> | <span data-ttu-id="01dd3-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01dd3-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01dd3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01dd3-116">HTTP request</span></span>
<span data-ttu-id="01dd3-117">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de grupos.</span><span class="sxs-lookup"><span data-stu-id="01dd3-117">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

### <a name="query-parameters"></a><span data-ttu-id="01dd3-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="01dd3-118">Query parameters</span></span>
<span data-ttu-id="01dd3-p103">Controlar alterações em grupos resulta em uma rodada de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e de `$skiptoken`), especifique na solicitação inicial **delta**. O Microsoft Graph codifica automaticamente os parâmetros especificados para a parte de token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="01dd3-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="01dd3-122">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="01dd3-122">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="01dd3-123">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="01dd3-123">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="01dd3-124">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="01dd3-124">Query parameter</span></span>      | <span data-ttu-id="01dd3-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="01dd3-125">Type</span></span>   |<span data-ttu-id="01dd3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="01dd3-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="01dd3-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="01dd3-127">$deltatoken</span></span> | <span data-ttu-id="01dd3-128">string</span><span class="sxs-lookup"><span data-stu-id="01dd3-128">string</span></span> | <span data-ttu-id="01dd3-p104">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de grupos indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="01dd3-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="01dd3-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="01dd3-131">$skiptoken</span></span> | <span data-ttu-id="01dd3-132">string</span><span class="sxs-lookup"><span data-stu-id="01dd3-132">string</span></span> | <span data-ttu-id="01dd3-133">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de grupos.</span><span class="sxs-lookup"><span data-stu-id="01dd3-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="01dd3-134">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="01dd3-134">Optional query parameters</span></span>
<span data-ttu-id="01dd3-135">Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="01dd3-135">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="01dd3-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="01dd3-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="01dd3-138">Suporte à consulta delta `$select`, `$top` e `$expand` para grupos.</span><span class="sxs-lookup"><span data-stu-id="01dd3-138">Delta query support `$select`, `$top`, and `$expand` for groups.</span></span> 
- <span data-ttu-id="01dd3-139">Há suporte limitado para `$filter` e `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="01dd3-139">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="01dd3-140">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="01dd3-140">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="01dd3-141">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="01dd3-141">You can filter multiple objects.</span></span> <span data-ttu-id="01dd3-142">Por exemplo, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff`.</span><span class="sxs-lookup"><span data-stu-id="01dd3-142">For example: `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff`.</span></span> <span data-ttu-id="01dd3-143">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="01dd3-143">There is a limit of 50 filtered objects.</span></span>
- <span data-ttu-id="01dd3-144">Não há suporte para `$search`.</span><span class="sxs-lookup"><span data-stu-id="01dd3-144">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01dd3-145">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01dd3-145">Request headers</span></span>
| <span data-ttu-id="01dd3-146">Nome</span><span class="sxs-lookup"><span data-stu-id="01dd3-146">Name</span></span>       | <span data-ttu-id="01dd3-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="01dd3-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="01dd3-148">Autorização</span><span class="sxs-lookup"><span data-stu-id="01dd3-148">Authorization</span></span>  | <span data-ttu-id="01dd3-149">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="01dd3-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="01dd3-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01dd3-150">Content-Type</span></span>  | <span data-ttu-id="01dd3-151">application/json</span><span class="sxs-lookup"><span data-stu-id="01dd3-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="01dd3-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01dd3-152">Request body</span></span>
<span data-ttu-id="01dd3-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01dd3-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01dd3-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="01dd3-154">Response</span></span>
<span data-ttu-id="01dd3-p107">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta. A resposta também inclui um token de estado que é uma URL nextLink ou uma URL deltaLink.</span><span class="sxs-lookup"><span data-stu-id="01dd3-p107">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body. The response also includes a state token which is either a nextLink URL or a deltaLink URL.</span></span>

- <span data-ttu-id="01dd3-p108">Se uma URL nextLink é retornada, existem páginas de dado adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL nextLink até uma URL deltaLink ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="01dd3-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="01dd3-p109">Se uma URL deltaLink for retornada, não haverá mais dados sobre o estado existente do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL deltaLink para se inteirar das alterações feitas no recurso.</span><span class="sxs-lookup"><span data-stu-id="01dd3-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="01dd3-161">Confira:</span><span class="sxs-lookup"><span data-stu-id="01dd3-161">See:</span></span></br>
- <span data-ttu-id="01dd3-162">[Usando a Consulta Delta](../../../concepts/delta_query_overview.md) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="01dd3-162">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="01dd3-163">[Obter as alterações incrementais para grupos](../../../concepts/delta_query_groups.md) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="01dd3-163">[Get incremental changes for groups](../../../concepts/delta_query_groups.md) for an example requests.</span></span></br>
    
## <a name="example"></a><span data-ttu-id="01dd3-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01dd3-164">Example</span></span>
#### <a name="request"></a><span data-ttu-id="01dd3-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01dd3-165">Request</span></span>
<span data-ttu-id="01dd3-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01dd3-166">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response"></a><span data-ttu-id="01dd3-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="01dd3-167">Response</span></span>
<span data-ttu-id="01dd3-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01dd3-168">The following is an example of the response.</span></span>
><span data-ttu-id="01dd3-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01dd3-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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