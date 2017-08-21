# <a name="create-conversation-thread"></a><span data-ttu-id="ec1da-101">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="ec1da-101">Create conversation thread</span></span>

<span data-ttu-id="ec1da-102">Inicie uma nova conversa em grupo criando primeiro um thread.</span><span class="sxs-lookup"><span data-stu-id="ec1da-102">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="ec1da-p101">Uma nova conversa, thread de conversas e posts são criados no grupo. Use [reply thread](conversationthread_reply.md) ou [reply post](post_reply.md) para postar mais naquele thread.</span><span class="sxs-lookup"><span data-stu-id="ec1da-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that thread.</span></span>

<span data-ttu-id="ec1da-105">Observação: também é possível [iniciar um novo thread em uma conversa existente](conversation_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="ec1da-105">Note: You can also [start a new thread in an existing conversation](conversation_post_threads.md).</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="ec1da-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec1da-106">Prerequisites</span></span>
<span data-ttu-id="ec1da-107">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="ec1da-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="ec1da-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec1da-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="ec1da-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec1da-109">Request headers</span></span>
| <span data-ttu-id="ec1da-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec1da-110">Header</span></span>       | <span data-ttu-id="ec1da-111">Valor</span><span class="sxs-lookup"><span data-stu-id="ec1da-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec1da-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec1da-112">Authorization</span></span>  | <span data-ttu-id="ec1da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec1da-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ec1da-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec1da-115">Content-Type</span></span>  | <span data-ttu-id="ec1da-116">application/json</span><span class="sxs-lookup"><span data-stu-id="ec1da-116">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec1da-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec1da-117">Request body</span></span>
<span data-ttu-id="ec1da-118">No corpo da solicitação, forneça uma representação JSON do objeto [conversationThread](../resources/conversationthread.md) que contém um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="ec1da-118">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="ec1da-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec1da-119">Response</span></span>

<span data-ttu-id="ec1da-120">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [conversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec1da-120">If successful, this method returns `201, Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec1da-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec1da-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec1da-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec1da-122">Request</span></span>
<span data-ttu-id="ec1da-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec1da-123">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ec1da-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec1da-124">Response</span></span>
<span data-ttu-id="ec1da-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec1da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
