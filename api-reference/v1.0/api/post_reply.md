# <a name="post-reply"></a><span data-ttu-id="78ccf-101">post: reply</span><span class="sxs-lookup"><span data-stu-id="78ccf-101">post: reply</span></span>

<span data-ttu-id="78ccf-p101">Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="78ccf-p101">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="78ccf-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="78ccf-104">Permissions</span></span>
<span data-ttu-id="78ccf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="78ccf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="78ccf-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78ccf-107">Permission type</span></span>      | <span data-ttu-id="78ccf-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78ccf-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="78ccf-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78ccf-109">Delegated (work or school account)</span></span> | <span data-ttu-id="78ccf-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78ccf-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="78ccf-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78ccf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78ccf-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78ccf-112">Not supported.</span></span>    | 
|<span data-ttu-id="78ccf-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78ccf-113">Application</span></span> | <span data-ttu-id="78ccf-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78ccf-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="78ccf-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78ccf-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="78ccf-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78ccf-116">Request headers</span></span>
| <span data-ttu-id="78ccf-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78ccf-117">Header</span></span>       | <span data-ttu-id="78ccf-118">Valor</span><span class="sxs-lookup"><span data-stu-id="78ccf-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="78ccf-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="78ccf-119">Authorization</span></span>  | <span data-ttu-id="78ccf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78ccf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="78ccf-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78ccf-122">Request body</span></span>
<span data-ttu-id="78ccf-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78ccf-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="78ccf-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="78ccf-124">Parameter</span></span>    | <span data-ttu-id="78ccf-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="78ccf-125">Type</span></span>   |<span data-ttu-id="78ccf-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="78ccf-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78ccf-127">post</span><span class="sxs-lookup"><span data-stu-id="78ccf-127">post</span></span>|[<span data-ttu-id="78ccf-128">post</span><span class="sxs-lookup"><span data-stu-id="78ccf-128">post</span></span>](../resources/post.md)|<span data-ttu-id="78ccf-129">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="78ccf-129">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="78ccf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="78ccf-130">Response</span></span>

<span data-ttu-id="78ccf-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78ccf-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78ccf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78ccf-133">Example</span></span>
<span data-ttu-id="78ccf-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="78ccf-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="78ccf-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78ccf-135">Request</span></span>
<span data-ttu-id="78ccf-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78ccf-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="78ccf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="78ccf-137">Response</span></span>
##### <a name="response"></a><span data-ttu-id="78ccf-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="78ccf-138">Response</span></span>
<span data-ttu-id="78ccf-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78ccf-139">Here is an example of the response.</span></span>
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
