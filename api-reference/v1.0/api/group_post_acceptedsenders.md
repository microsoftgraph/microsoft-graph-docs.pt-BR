# <a name="create-acceptedsender"></a><span data-ttu-id="b545e-101">Criar acceptedSender</span><span class="sxs-lookup"><span data-stu-id="b545e-101">Create acceptedSender</span></span>

<span data-ttu-id="b545e-102">Adicione um novo usuário ou grupo à lista acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="b545e-102">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="b545e-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes aceitos podem postar em conversas do grupo. Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="b545e-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b545e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b545e-106">Prerequisites</span></span>
<span data-ttu-id="b545e-107">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="b545e-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="b545e-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b545e-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b545e-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b545e-109">Request headers</span></span>
| <span data-ttu-id="b545e-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b545e-110">Header</span></span>       | <span data-ttu-id="b545e-111">Valor</span><span class="sxs-lookup"><span data-stu-id="b545e-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b545e-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="b545e-112">Authorization</span></span>  | <span data-ttu-id="b545e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b545e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b545e-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b545e-115">Request body</span></span>
<span data-ttu-id="b545e-116">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="b545e-116">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="b545e-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="b545e-117">Response</span></span>

<span data-ttu-id="b545e-118">Este método retorna o código de resposta `204, No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b545e-118">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="b545e-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b545e-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b545e-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b545e-120">Request</span></span>
<span data-ttu-id="b545e-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b545e-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="b545e-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="b545e-122">Response</span></span>
<span data-ttu-id="b545e-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b545e-123">Here is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
