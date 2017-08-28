# <a name="conversationthread-reply"></a><span data-ttu-id="b56a0-101">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="b56a0-101">conversationThread: reply</span></span>

<span data-ttu-id="b56a0-p101">Responde a um thread em uma conversa de grupo e adicione uma nova postagem a ele. Você pode especificar a conversa pai na solicitação ou apenas o thread, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="b56a0-p101">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="b56a0-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="b56a0-104">Permissions</span></span>
<span data-ttu-id="b56a0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b56a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b56a0-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b56a0-107">Permission type</span></span>      | <span data-ttu-id="b56a0-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b56a0-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b56a0-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b56a0-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b56a0-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b56a0-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="b56a0-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b56a0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b56a0-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b56a0-112">Not supported.</span></span>    | 
|<span data-ttu-id="b56a0-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b56a0-113">Application</span></span> | <span data-ttu-id="b56a0-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b56a0-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b56a0-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b56a0-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="b56a0-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b56a0-116">Request headers</span></span>
| <span data-ttu-id="b56a0-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b56a0-117">Header</span></span>       | <span data-ttu-id="b56a0-118">Valor</span><span class="sxs-lookup"><span data-stu-id="b56a0-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b56a0-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b56a0-119">Authorization</span></span>  | <span data-ttu-id="b56a0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b56a0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b56a0-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b56a0-122">Content-Type</span></span>  | <span data-ttu-id="b56a0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b56a0-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b56a0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b56a0-125">Request body</span></span>
<span data-ttu-id="b56a0-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b56a0-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b56a0-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b56a0-127">Parameter</span></span>    | <span data-ttu-id="b56a0-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b56a0-128">Type</span></span>   |<span data-ttu-id="b56a0-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b56a0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b56a0-130">post</span><span class="sxs-lookup"><span data-stu-id="b56a0-130">post</span></span>|[<span data-ttu-id="b56a0-131">post</span><span class="sxs-lookup"><span data-stu-id="b56a0-131">post</span></span>](../resources/post.md)|<span data-ttu-id="b56a0-132">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="b56a0-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="b56a0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b56a0-133">Response</span></span>

<span data-ttu-id="b56a0-p105">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b56a0-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b56a0-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b56a0-136">Example</span></span>
<span data-ttu-id="b56a0-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b56a0-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b56a0-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b56a0-138">Request</span></span>
<span data-ttu-id="b56a0-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b56a0-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="b56a0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b56a0-140">Response</span></span>
<span data-ttu-id="b56a0-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b56a0-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
