# <a name="create-conversation-thread"></a><span data-ttu-id="bd7e4-101">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="bd7e4-101">Create conversation thread</span></span>
<span data-ttu-id="bd7e4-102">Inicie uma nova conversa em grupo criando primeiro um thread.</span><span class="sxs-lookup"><span data-stu-id="bd7e4-102">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="bd7e4-p101">Uma nova conversa, thread de conversas e posts são criados no grupo. Use [reply thread](conversationthread_reply.md) ou [reply post](post_reply.md) para postar mais naquele thread.</span><span class="sxs-lookup"><span data-stu-id="bd7e4-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that thread.</span></span>

<span data-ttu-id="bd7e4-105">Observação: também é possível [iniciar um novo thread em uma conversa existente](conversation_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="bd7e4-105">Note: You can also [start a new thread in an existing conversation](conversation_post_threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="bd7e4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd7e4-106">Permissions</span></span>
<span data-ttu-id="bd7e4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd7e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bd7e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd7e4-109">Permission type</span></span>      | <span data-ttu-id="bd7e4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd7e4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd7e4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd7e4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bd7e4-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd7e4-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bd7e4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd7e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd7e4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd7e4-114">Not supported.</span></span>    |
|<span data-ttu-id="bd7e4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd7e4-115">Application</span></span> | <span data-ttu-id="bd7e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd7e4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd7e4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd7e4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="bd7e4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd7e4-118">Request headers</span></span>
| <span data-ttu-id="bd7e4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd7e4-119">Header</span></span>       | <span data-ttu-id="bd7e4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="bd7e4-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd7e4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd7e4-121">Authorization</span></span>  | <span data-ttu-id="bd7e4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd7e4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bd7e4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd7e4-124">Content-Type</span></span>  | <span data-ttu-id="bd7e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd7e4-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bd7e4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd7e4-126">Request body</span></span>
<span data-ttu-id="bd7e4-127">No corpo da solicitação, forneça uma representação JSON do objeto [conversationThread](../resources/conversationthread.md) que contém um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="bd7e4-127">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="bd7e4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd7e4-128">Response</span></span>
<span data-ttu-id="bd7e4-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd7e4-129">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd7e4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd7e4-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bd7e4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd7e4-131">Request</span></span>
<span data-ttu-id="bd7e4-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd7e4-132">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```
#### <a name="response"></a><span data-ttu-id="bd7e4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd7e4-133">Response</span></span>
<span data-ttu-id="bd7e4-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd7e4-134">Here is an example of the response.</span></span>
><span data-ttu-id="bd7e4-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bd7e4-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bd7e4-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd7e4-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
