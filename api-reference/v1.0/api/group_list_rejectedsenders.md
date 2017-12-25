# <a name="list-rejectedsenders"></a><span data-ttu-id="58cd9-101">Listar rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="58cd9-101">List rejectedSenders</span></span>
<span data-ttu-id="58cd9-102">Obter uma lista de usuários ou grupos que estão na lista rejectedSenders desse grupo.</span><span class="sxs-lookup"><span data-stu-id="58cd9-102">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="58cd9-p101">Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="58cd9-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="58cd9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="58cd9-105">Permissions</span></span>
<span data-ttu-id="58cd9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="58cd9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="58cd9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58cd9-108">Permission type</span></span>      | <span data-ttu-id="58cd9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58cd9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58cd9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58cd9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="58cd9-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58cd9-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="58cd9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58cd9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58cd9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58cd9-113">Not supported.</span></span>    |
|<span data-ttu-id="58cd9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58cd9-114">Application</span></span> | <span data-ttu-id="58cd9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58cd9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58cd9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58cd9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58cd9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58cd9-117">Optional query parameters</span></span>
<span data-ttu-id="58cd9-118">Este método dá suporte a [Parâmetros de consulta OData](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="58cd9-118">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58cd9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58cd9-119">Request headers</span></span>
| <span data-ttu-id="58cd9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58cd9-120">Header</span></span>       | <span data-ttu-id="58cd9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="58cd9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="58cd9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="58cd9-122">Authorization</span></span>  | <span data-ttu-id="58cd9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58cd9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="58cd9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58cd9-125">Request body</span></span>
<span data-ttu-id="58cd9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58cd9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58cd9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="58cd9-127">Response</span></span>
<span data-ttu-id="58cd9-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58cd9-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58cd9-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58cd9-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="58cd9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58cd9-130">Request</span></span>
<span data-ttu-id="58cd9-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58cd9-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="58cd9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="58cd9-132">Response</span></span>
<span data-ttu-id="58cd9-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="58cd9-133">The following is an example of the response.</span></span>
><span data-ttu-id="58cd9-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="58cd9-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="58cd9-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58cd9-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->