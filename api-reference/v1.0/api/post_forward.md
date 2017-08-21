# <a name="post-forward"></a><span data-ttu-id="fab07-101">post: forward</span><span class="sxs-lookup"><span data-stu-id="fab07-101">post: forward</span></span>

<span data-ttu-id="fab07-p101">Encaminhe uma postagem para um destinatário. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="fab07-p101">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="fab07-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fab07-104">Prerequisites</span></span>
<span data-ttu-id="fab07-105">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="fab07-105">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="fab07-106">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="fab07-106">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="fab07-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fab07-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="fab07-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fab07-108">Request headers</span></span>
| <span data-ttu-id="fab07-109">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fab07-109">Header</span></span>       | <span data-ttu-id="fab07-110">Valor</span><span class="sxs-lookup"><span data-stu-id="fab07-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fab07-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="fab07-111">Authorization</span></span>  | <span data-ttu-id="fab07-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fab07-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fab07-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fab07-114">Request body</span></span>
<span data-ttu-id="fab07-115">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fab07-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fab07-116">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fab07-116">Parameter</span></span>    | <span data-ttu-id="fab07-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="fab07-117">Type</span></span>   |<span data-ttu-id="fab07-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="fab07-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fab07-119">comment</span><span class="sxs-lookup"><span data-stu-id="fab07-119">comment</span></span>|<span data-ttu-id="fab07-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fab07-120">String</span></span>|<span data-ttu-id="fab07-121">Comentário opcional que é encaminhado com a postagem.</span><span class="sxs-lookup"><span data-stu-id="fab07-121">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="fab07-122">toRecipients</span><span class="sxs-lookup"><span data-stu-id="fab07-122">toRecipients</span></span>|<span data-ttu-id="fab07-123">Coleção [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="fab07-123">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="fab07-124">Os destinatários aos quais os threads são encaminhados.</span><span class="sxs-lookup"><span data-stu-id="fab07-124">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="fab07-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="fab07-125">Response</span></span>

<span data-ttu-id="fab07-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fab07-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fab07-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fab07-128">Example</span></span>
<span data-ttu-id="fab07-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fab07-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fab07-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fab07-130">Request</span></span>
<span data-ttu-id="fab07-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fab07-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="fab07-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fab07-132">Response</span></span>
<span data-ttu-id="fab07-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fab07-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
