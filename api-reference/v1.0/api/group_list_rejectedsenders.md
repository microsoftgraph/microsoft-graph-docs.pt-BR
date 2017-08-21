# <a name="list-rejectedsenders"></a><span data-ttu-id="68b86-101">Listar rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="68b86-101">List rejectedSenders</span></span>

<span data-ttu-id="68b86-102">Obter uma lista de usuários ou grupos que estão na lista rejectedSenders desse grupo.</span><span class="sxs-lookup"><span data-stu-id="68b86-102">Get a list of users or groups that are in the rejectedSenders list for this group.</span></span> 

<span data-ttu-id="68b86-p101">Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação GET). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="68b86-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68b86-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68b86-105">Prerequisites</span></span>
<span data-ttu-id="68b86-106">Um dos seguintes **escopos** é obrigatório para executar esta API:  *Group.Read.All* ou *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="68b86-106">One of the following **scopes** is required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="68b86-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68b86-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="68b86-108">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="68b86-108">Optional query parameters</span></span>
<span data-ttu-id="68b86-109">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="68b86-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="68b86-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68b86-110">Request headers</span></span>
| <span data-ttu-id="68b86-111">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68b86-111">Header</span></span>       | <span data-ttu-id="68b86-112">Valor</span><span class="sxs-lookup"><span data-stu-id="68b86-112">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68b86-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="68b86-113">Authorization</span></span>  | <span data-ttu-id="68b86-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68b86-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68b86-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68b86-116">Request body</span></span>
<span data-ttu-id="68b86-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="68b86-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68b86-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="68b86-118">Response</span></span>

<span data-ttu-id="68b86-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68b86-119">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="68b86-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68b86-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68b86-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68b86-121">Request</span></span>
<span data-ttu-id="68b86-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68b86-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```
##### <a name="response"></a><span data-ttu-id="68b86-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="68b86-123">Response</span></span>
<span data-ttu-id="68b86-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68b86-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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