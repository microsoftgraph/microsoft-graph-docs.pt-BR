# <a name="list-rejectedsenders"></a><span data-ttu-id="182b5-101">Listar rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="182b5-101">List rejectedSenders</span></span>

<span data-ttu-id="182b5-102">Obter uma lista de usuários ou grupos que estão na lista rejectedSenders desse grupo.</span><span class="sxs-lookup"><span data-stu-id="182b5-102">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="182b5-p101">Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="182b5-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="permissions"></a><span data-ttu-id="182b5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="182b5-105">Permissions</span></span>
<span data-ttu-id="182b5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="182b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="182b5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="182b5-108">Permission type</span></span>      | <span data-ttu-id="182b5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="182b5-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="182b5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="182b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="182b5-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="182b5-111">Group.Read.All, Group.Readwrite.All</span></span>    | 
|<span data-ttu-id="182b5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="182b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="182b5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="182b5-113">Not supported.</span></span>    | 
|<span data-ttu-id="182b5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="182b5-114">Application</span></span> | <span data-ttu-id="182b5-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="182b5-115">Group.Read.All, Group.Readwrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="182b5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="182b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="182b5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="182b5-117">Optional query parameters</span></span>
<span data-ttu-id="182b5-118">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="182b5-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="182b5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="182b5-119">Request headers</span></span>
| <span data-ttu-id="182b5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="182b5-120">Header</span></span>       | <span data-ttu-id="182b5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="182b5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="182b5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="182b5-122">Authorization</span></span>  | <span data-ttu-id="182b5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="182b5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="182b5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="182b5-125">Request body</span></span>
<span data-ttu-id="182b5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="182b5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="182b5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="182b5-127">Response</span></span>

<span data-ttu-id="182b5-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="182b5-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="182b5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="182b5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="182b5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="182b5-130">Request</span></span>
<span data-ttu-id="182b5-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="182b5-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```
##### <a name="response"></a><span data-ttu-id="182b5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="182b5-132">Response</span></span>
<span data-ttu-id="182b5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="182b5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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