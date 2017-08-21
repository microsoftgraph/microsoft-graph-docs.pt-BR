# <a name="conversationthread-reply"></a><span data-ttu-id="ceb90-101">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="ceb90-101">conversationThread: reply</span></span>

<span data-ttu-id="ceb90-p101">Responde a um thread em uma conversa de grupo e adicione uma nova postagem a ele. Você pode especificar a conversa pai na solicitação ou apenas o thread, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="ceb90-p101">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ceb90-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ceb90-104">Prerequisites</span></span>
<span data-ttu-id="ceb90-105">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="ceb90-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="ceb90-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceb90-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="ceb90-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb90-107">Request headers</span></span>
| <span data-ttu-id="ceb90-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ceb90-108">Header</span></span>       | <span data-ttu-id="ceb90-109">Valor</span><span class="sxs-lookup"><span data-stu-id="ceb90-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ceb90-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceb90-110">Authorization</span></span>  | <span data-ttu-id="ceb90-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceb90-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ceb90-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ceb90-113">Content-Type</span></span>  | <span data-ttu-id="ceb90-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceb90-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ceb90-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb90-116">Request body</span></span>
<span data-ttu-id="ceb90-117">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceb90-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ceb90-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ceb90-118">Parameter</span></span>    | <span data-ttu-id="ceb90-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ceb90-119">Type</span></span>   |<span data-ttu-id="ceb90-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceb90-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ceb90-121">post</span><span class="sxs-lookup"><span data-stu-id="ceb90-121">post</span></span>|[<span data-ttu-id="ceb90-122">post</span><span class="sxs-lookup"><span data-stu-id="ceb90-122">post</span></span>](../resources/post.md)|<span data-ttu-id="ceb90-123">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="ceb90-123">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="ceb90-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceb90-124">Response</span></span>

<span data-ttu-id="ceb90-p104">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceb90-p104">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceb90-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ceb90-127">Example</span></span>
<span data-ttu-id="ceb90-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ceb90-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ceb90-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceb90-129">Request</span></span>
<span data-ttu-id="ceb90-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceb90-130">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ceb90-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceb90-131">Response</span></span>
<span data-ttu-id="ceb90-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceb90-132">Here is an example of the response.</span></span>
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
