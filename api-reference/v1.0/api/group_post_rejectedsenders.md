# <a name="create-rejectedsender"></a><span data-ttu-id="d0024-101">Criar rejectedSender</span><span class="sxs-lookup"><span data-stu-id="d0024-101">Create rejectedSender</span></span>

<span data-ttu-id="d0024-102">Adiciona um novo usuário ou grupo à lista rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="d0024-102">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="d0024-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação POST). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="d0024-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0024-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0024-106">Prerequisites</span></span>
<span data-ttu-id="d0024-107">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="d0024-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="d0024-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0024-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d0024-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0024-109">Request headers</span></span>
| <span data-ttu-id="d0024-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0024-110">Header</span></span>       | <span data-ttu-id="d0024-111">Valor</span><span class="sxs-lookup"><span data-stu-id="d0024-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0024-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0024-112">Authorization</span></span>  | <span data-ttu-id="d0024-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0024-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0024-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0024-115">Request body</span></span>
<span data-ttu-id="d0024-116">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="d0024-116">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="d0024-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0024-117">Response</span></span>

<span data-ttu-id="d0024-118">Este método retorna o código de resposta `204, No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0024-118">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0024-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0024-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0024-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0024-120">Request</span></span>
<span data-ttu-id="d0024-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0024-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="d0024-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0024-122">Response</span></span>
<span data-ttu-id="d0024-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0024-123">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
