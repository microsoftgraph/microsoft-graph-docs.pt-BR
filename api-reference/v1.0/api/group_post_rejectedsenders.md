# <a name="create-rejectedsender"></a><span data-ttu-id="a319c-101">Criar rejectedSender</span><span class="sxs-lookup"><span data-stu-id="a319c-101">Create rejectedSender</span></span>

<span data-ttu-id="a319c-102">Adiciona um novo usuário ou grupo à lista rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="a319c-102">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="a319c-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação POST). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="a319c-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="permissions"></a><span data-ttu-id="a319c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a319c-106">Permissions</span></span>
<span data-ttu-id="a319c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a319c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a319c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a319c-109">Permission type</span></span>      | <span data-ttu-id="a319c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a319c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a319c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a319c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a319c-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a319c-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a319c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a319c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a319c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a319c-114">Not supported.</span></span>    |
|<span data-ttu-id="a319c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a319c-115">Application</span></span> | <span data-ttu-id="a319c-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a319c-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a319c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a319c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a319c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a319c-118">Request headers</span></span>
| <span data-ttu-id="a319c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a319c-119">Header</span></span>       | <span data-ttu-id="a319c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a319c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a319c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a319c-121">Authorization</span></span>  | <span data-ttu-id="a319c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a319c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a319c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a319c-124">Request body</span></span>
<span data-ttu-id="a319c-125">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="a319c-125">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="a319c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a319c-126">Response</span></span>

<span data-ttu-id="a319c-127">Este método retorna o código de resposta `204, No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a319c-127">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="a319c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a319c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a319c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a319c-129">Request</span></span>
<span data-ttu-id="a319c-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a319c-130">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="a319c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a319c-131">Response</span></span>
<span data-ttu-id="a319c-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a319c-132">Here is an example of the response.</span></span>
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
