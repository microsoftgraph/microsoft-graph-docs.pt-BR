# <a name="post-reply"></a><span data-ttu-id="8f3cc-101">post: reply</span><span class="sxs-lookup"><span data-stu-id="8f3cc-101">post: reply</span></span>

<span data-ttu-id="8f3cc-p101">Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="8f3cc-p101">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f3cc-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f3cc-104">Prerequisites</span></span>
<span data-ttu-id="8f3cc-105">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="8f3cc-105">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="8f3cc-106">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="8f3cc-106">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="8f3cc-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f3cc-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="8f3cc-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f3cc-108">Request headers</span></span>
| <span data-ttu-id="8f3cc-109">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f3cc-109">Header</span></span>       | <span data-ttu-id="8f3cc-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8f3cc-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8f3cc-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f3cc-111">Authorization</span></span>  | <span data-ttu-id="8f3cc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f3cc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8f3cc-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f3cc-114">Request body</span></span>
<span data-ttu-id="8f3cc-115">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f3cc-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8f3cc-116">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8f3cc-116">Parameter</span></span>    | <span data-ttu-id="8f3cc-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f3cc-117">Type</span></span>   |<span data-ttu-id="8f3cc-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f3cc-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f3cc-119">post</span><span class="sxs-lookup"><span data-stu-id="8f3cc-119">post</span></span>|[<span data-ttu-id="8f3cc-120">post</span><span class="sxs-lookup"><span data-stu-id="8f3cc-120">post</span></span>](../resources/post.md)|<span data-ttu-id="8f3cc-121">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="8f3cc-121">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="8f3cc-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f3cc-122">Response</span></span>

<span data-ttu-id="8f3cc-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f3cc-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f3cc-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f3cc-125">Example</span></span>
<span data-ttu-id="8f3cc-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8f3cc-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8f3cc-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f3cc-127">Request</span></span>
<span data-ttu-id="8f3cc-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f3cc-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "datetime-value",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "datetime-value",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="8f3cc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f3cc-129">Response</span></span>
##### <a name="response"></a><span data-ttu-id="8f3cc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f3cc-130">Response</span></span>
<span data-ttu-id="8f3cc-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f3cc-131">Here is an example of the response.</span></span>
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
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
