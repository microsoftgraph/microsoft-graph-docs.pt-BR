# <a name="group-delta"></a><span data-ttu-id="cc03c-101">group: delta</span><span class="sxs-lookup"><span data-stu-id="cc03c-101">group: delta</span></span>
<span data-ttu-id="cc03c-p101">A [consulta delta](../../../concepts/delta_query_overview.md) permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Para descobrir as alterações nos grupos, realize uma solicitação usando a função *delta*. Confira [Usando a Consulta Delta](../../../concepts/delta_query_overview.md) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="cc03c-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to groups, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc03c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc03c-105">Permissions</span></span>
<span data-ttu-id="cc03c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cc03c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cc03c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc03c-108">Permission type</span></span>      | <span data-ttu-id="cc03c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc03c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc03c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc03c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cc03c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc03c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc03c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc03c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc03c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc03c-113">Not supported.</span></span>    |
|<span data-ttu-id="cc03c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc03c-114">Application</span></span> | <span data-ttu-id="cc03c-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc03c-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc03c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc03c-116">HTTP request</span></span>
<span data-ttu-id="cc03c-117">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de grupos.</span><span class="sxs-lookup"><span data-stu-id="cc03c-117">To begin tracking changes, you make a request including the delta function on the groups resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/delta
```

## <a name="query-parameters"></a><span data-ttu-id="cc03c-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="cc03c-118">Query parameters</span></span>
<span data-ttu-id="cc03c-p103">Controlar alterações em grupos resulta em uma rodada de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e de `$skiptoken`), especifique na solicitação inicial **delta**. O Microsoft Graph codifica automaticamente os parâmetros especificados para a parte de token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="cc03c-p103">Tracking changes in groups incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span>

<span data-ttu-id="cc03c-122">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="cc03c-122">You only need to specify any desired query parameters once upfront.</span></span>

<span data-ttu-id="cc03c-123">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="cc03c-123">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="cc03c-124">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="cc03c-124">Query parameter</span></span>      | <span data-ttu-id="cc03c-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc03c-125">Type</span></span>   |<span data-ttu-id="cc03c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc03c-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cc03c-127">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="cc03c-127">$deltatoken</span></span> | <span data-ttu-id="cc03c-128">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc03c-128">string</span></span> | <span data-ttu-id="cc03c-p104">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de grupos indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="cc03c-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same group collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="cc03c-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="cc03c-131">$skiptoken</span></span> | <span data-ttu-id="cc03c-132">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc03c-132">string</span></span> | <span data-ttu-id="cc03c-133">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de grupos.</span><span class="sxs-lookup"><span data-stu-id="cc03c-133">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same group collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="cc03c-134">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="cc03c-134">OData query parameters</span></span>
<span data-ttu-id="cc03c-135">Este método dá suporte a parâmetros opcionais de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cc03c-135">This method supports the OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="cc03c-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="cc03c-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>
- <span data-ttu-id="cc03c-138">Suporte à consulta delta `$select`, `$top` e `$expand` para grupos.</span><span class="sxs-lookup"><span data-stu-id="cc03c-138">Delta query support `$select`, `$top`, and `$expand` for groups.</span></span>
- <span data-ttu-id="cc03c-139">Há suporte limitado para `$filter` e `$orderby`:</span><span class="sxs-lookup"><span data-stu-id="cc03c-139">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="cc03c-140">A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`.</span><span class="sxs-lookup"><span data-stu-id="cc03c-140">The only supported `$filter` expression is for tracking changes on a specific object: `$filter=id+eq+{value}`.</span></span> <span data-ttu-id="cc03c-141">É possível filtrar vários objetos.</span><span class="sxs-lookup"><span data-stu-id="cc03c-141">You can filter multiple objects.</span></span> <span data-ttu-id="cc03c-142">Por exemplo, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff`.</span><span class="sxs-lookup"><span data-stu-id="cc03c-142">For example, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff`.</span></span> <span data-ttu-id="cc03c-143">Há um limite de 50 objetos filtrados.</span><span class="sxs-lookup"><span data-stu-id="cc03c-143">There is a limit of 50 filtered objects.</span></span>
- <span data-ttu-id="cc03c-144">Não há suporte para `$search`.</span><span class="sxs-lookup"><span data-stu-id="cc03c-144">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc03c-145">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc03c-145">Request headers</span></span>
| <span data-ttu-id="cc03c-146">Nome</span><span class="sxs-lookup"><span data-stu-id="cc03c-146">Name</span></span>       | <span data-ttu-id="cc03c-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc03c-147">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cc03c-148">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc03c-148">Authorization</span></span>  | <span data-ttu-id="cc03c-149">Token&gt; de portador&gt;</span><span class="sxs-lookup"><span data-stu-id="cc03c-149">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="cc03c-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc03c-150">Content-Type</span></span>  | <span data-ttu-id="cc03c-151">application/json</span><span class="sxs-lookup"><span data-stu-id="cc03c-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc03c-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc03c-152">Request body</span></span>
<span data-ttu-id="cc03c-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc03c-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc03c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc03c-154">Response</span></span>
<span data-ttu-id="cc03c-p107">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta. A resposta também inclui um token de estado que é uma URL nextLink ou uma URL deltaLink.</span><span class="sxs-lookup"><span data-stu-id="cc03c-p107">If successful, this method returns `200 OK` response code and [group](../resources/group.md) collection object in the response body. The response also includes a state token which is either a nextLink URL or a deltaLink URL.</span></span>

- <span data-ttu-id="cc03c-p108">Se uma URL nextLink é retornada, existem páginas de dado adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL nextLink até uma URL deltaLink ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="cc03c-p108">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="cc03c-p109">Se uma URL deltaLink for retornada, não haverá mais dados sobre o estado existente do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL deltaLink para se inteirar das alterações feitas no recurso.</span><span class="sxs-lookup"><span data-stu-id="cc03c-p109">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="cc03c-161">Confira:</span><span class="sxs-lookup"><span data-stu-id="cc03c-161">See:</span></span></br>
- <span data-ttu-id="cc03c-162">[Usando a Consulta Delta](../../../concepts/delta_query_overview.md) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="cc03c-162">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="cc03c-163">[Obter alterações incrementais para grupos](../../../concepts/delta_query_groups.md) para uma explicação mais detalhada.</span><span class="sxs-lookup"><span data-stu-id="cc03c-163">[Get incremental changes for groups](../../../concepts/delta_query_groups.md) for a more detailed walkthrough.</span></span></br>

## <a name="example"></a><span data-ttu-id="cc03c-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc03c-164">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cc03c-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc03c-165">Request</span></span>
<span data-ttu-id="cc03c-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc03c-166">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response"></a><span data-ttu-id="cc03c-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc03c-167">Response</span></span>
<span data-ttu-id="cc03c-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc03c-168">The following is an example of the response.</span></span>
><span data-ttu-id="cc03c-p110">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para maior legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc03c-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
>
> <span data-ttu-id="cc03c-171">Observe a presença da propriedade *members@delta* que inclui as ids de objetos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="cc03c-171">Note the presence of the *members@delta* property which includes the ids of member objects in the group.</span></span>

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
      "mail": "mail-value",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="cc03c-172">Confira também</span><span class="sxs-lookup"><span data-stu-id="cc03c-172">See also</span></span>
- <span data-ttu-id="cc03c-173">[Usando a Consulta Delta](../../../concepts/delta_query_overview.md) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="cc03c-173">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span>
- <span data-ttu-id="cc03c-174">[Obter alterações incrementais para grupos](../../../concepts/delta_query_groups.md) para uma explicação mais detalhada.</span><span class="sxs-lookup"><span data-stu-id="cc03c-174">[Get incremental changes for groups](../../../concepts/delta_query_groups.md) for a more detailed walkthrough.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
