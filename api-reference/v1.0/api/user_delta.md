# <a name="user-delta"></a><span data-ttu-id="674fd-101">user: delta</span><span class="sxs-lookup"><span data-stu-id="674fd-101">user: delta</span></span>

<span data-ttu-id="674fd-p101">A [consulta delta](../../../concepts/delta_query_overview.md) permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Para descobrir as alterações nos usuários, realize uma solicitação usando a função *delta*. Confira [Usando a Consulta Delta](../../../concepts/delta_query_overview.md) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="674fd-p101">[Delta query](../../../concepts/delta_query_overview.md) enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. To discover changes to users, perform a request using the *delta* function. See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="674fd-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="674fd-105">Prerequisites</span></span>

<span data-ttu-id="674fd-106">Um dos seguintes **escopos** é obrigatório para executar esta API: *User.Read; User.ReadWrite; User.ReadBasic.All; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="674fd-106">One of the following **scopes** is required to execute this API: *User.Read; User.ReadWrite; User.ReadBasic.All; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="674fd-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="674fd-107">HTTP request</span></span>

<span data-ttu-id="674fd-108">Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de usuários.</span><span class="sxs-lookup"><span data-stu-id="674fd-108">To begin tracking changes, you make a request including the delta function on the users resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

### <a name="query-parameters"></a><span data-ttu-id="674fd-109">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="674fd-109">Query parameters</span></span>

<span data-ttu-id="674fd-p102">O controle de alterações em usuários corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="674fd-p102">Tracking changes in users incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="674fd-115">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="674fd-115">Query parameter</span></span>      | <span data-ttu-id="674fd-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="674fd-116">Type</span></span>   |<span data-ttu-id="674fd-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="674fd-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="674fd-118">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="674fd-118">$deltatoken</span></span> | <span data-ttu-id="674fd-119">string</span><span class="sxs-lookup"><span data-stu-id="674fd-119">string</span></span> | <span data-ttu-id="674fd-p103">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de usuários indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="674fd-p103">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same user collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="674fd-122">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="674fd-122">$skiptoken</span></span> | <span data-ttu-id="674fd-123">string</span><span class="sxs-lookup"><span data-stu-id="674fd-123">string</span></span> | <span data-ttu-id="674fd-124">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="674fd-124">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same user collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="674fd-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="674fd-125">Optional query parameters</span></span>

<span data-ttu-id="674fd-126">Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="674fd-126">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="674fd-p104">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="674fd-p104">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="674fd-129">Suporte à consulta delta `$select`, `$top` e `$expand` para mensagens.</span><span class="sxs-lookup"><span data-stu-id="674fd-129">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="674fd-p105">Há suporte limitado para `$orderby`: A única expressão `$orderby` suportada é `$orderby=receivedDateTime+desc`. Se você não incluir uma expressão `$orderby`, a ordem de retorno não será garantida.</span><span class="sxs-lookup"><span data-stu-id="674fd-p105">There is limited support for `$orderby`: The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include  an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="674fd-132">Não há suporte DAV para `$search`.</span><span class="sxs-lookup"><span data-stu-id="674fd-132">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="674fd-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="674fd-133">Request headers</span></span>
| <span data-ttu-id="674fd-134">Nome</span><span class="sxs-lookup"><span data-stu-id="674fd-134">Name</span></span>       | <span data-ttu-id="674fd-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="674fd-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="674fd-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="674fd-136">Authorization</span></span>  | <span data-ttu-id="674fd-137">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="674fd-137">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="674fd-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="674fd-138">Content-Type</span></span>  | <span data-ttu-id="674fd-139">application/json</span><span class="sxs-lookup"><span data-stu-id="674fd-139">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="674fd-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="674fd-140">Request body</span></span>
<span data-ttu-id="674fd-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="674fd-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="674fd-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="674fd-142">Response</span></span>

<span data-ttu-id="674fd-p106">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto da coleção [user](../resources/user.md) no corpo da resposta. A resposta também inclui uma URL nextLink ou uma URL deltaLink.</span><span class="sxs-lookup"><span data-stu-id="674fd-p106">If successful, this method returns `200, OK` response code and [user](../resources/user.md) collection object in the response body. The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="674fd-p107">Se uma URL nextLink é retornada, existem páginas de dado adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL nextLink até uma URL deltaLink ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="674fd-p107">If a nextLink URL is returned, there are additional pages of data to be retrieved in the session. The application continues making requests using the nextLink URL until a deltaLink URL is included in the response.</span></span>

- <span data-ttu-id="674fd-p108">Se uma URL deltaLink for retornada, não haverá mais dados sobre o estado existente do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL deltaLink para se inteirar das alterações feitas no recurso.</span><span class="sxs-lookup"><span data-stu-id="674fd-p108">If a deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource.</span></span>

<span data-ttu-id="674fd-149">Confira:</span><span class="sxs-lookup"><span data-stu-id="674fd-149">See:</span></span></br>
- <span data-ttu-id="674fd-150">[Usando a Consulta Delta](../../../concepts/delta_query_overview.md) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="674fd-150">[Using Delta Query](../../../concepts/delta_query_overview.md) for more details</span></span></br>
- <span data-ttu-id="674fd-151">[Obter as alterações incrementais para usuários](../../../concepts/delta_query_users.md) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="674fd-151">[Get incremental changes for users](../../../concepts/delta_query_users.md) for an example requests.</span></span></br>

## <a name="example"></a><span data-ttu-id="674fd-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="674fd-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="674fd-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="674fd-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/delta
```

##### <a name="response"></a><span data-ttu-id="674fd-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="674fd-154">Response</span></span>
<span data-ttu-id="674fd-p109">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="674fd-p109">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->