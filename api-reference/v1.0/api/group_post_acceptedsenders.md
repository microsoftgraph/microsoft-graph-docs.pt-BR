# <a name="create-acceptedsender"></a><span data-ttu-id="ba2e0-101">Criar acceptedSender</span><span class="sxs-lookup"><span data-stu-id="ba2e0-101">Create acceptedSender</span></span>

<span data-ttu-id="ba2e0-102">Adicione um novo usuário ou grupo à lista acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="ba2e0-102">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="ba2e0-p101">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes aceitos podem postar em conversas do grupo. Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="ba2e0-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba2e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba2e0-106">Permissions</span></span>
<span data-ttu-id="ba2e0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba2e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ba2e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba2e0-109">Permission type</span></span>      | <span data-ttu-id="ba2e0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba2e0-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="ba2e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba2e0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ba2e0-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba2e0-112">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="ba2e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba2e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba2e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba2e0-114">Not supported.</span></span>    | 
|<span data-ttu-id="ba2e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba2e0-115">Application</span></span> | <span data-ttu-id="ba2e0-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba2e0-116">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ba2e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba2e0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ba2e0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba2e0-118">Request headers</span></span>
| <span data-ttu-id="ba2e0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba2e0-119">Header</span></span>       | <span data-ttu-id="ba2e0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ba2e0-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba2e0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba2e0-121">Authorization</span></span>  | <span data-ttu-id="ba2e0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba2e0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba2e0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba2e0-124">Request body</span></span>
<span data-ttu-id="ba2e0-125">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="ba2e0-125">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="ba2e0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba2e0-126">Response</span></span>

<span data-ttu-id="ba2e0-127">Este método retorna o código de resposta `204, No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba2e0-127">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba2e0-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba2e0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba2e0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba2e0-129">Request</span></span>
<span data-ttu-id="ba2e0-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba2e0-130">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ba2e0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba2e0-131">Response</span></span>
<span data-ttu-id="ba2e0-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba2e0-132">Here is an example of the response.</span></span>
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
