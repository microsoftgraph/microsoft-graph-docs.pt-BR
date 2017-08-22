# <a name="create-conversation"></a><span data-ttu-id="3edf1-101">Criar conversa</span><span class="sxs-lookup"><span data-stu-id="3edf1-101">Create Conversation</span></span>

<span data-ttu-id="3edf1-102">Crie uma nova conversa incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="3edf1-102">Create a new conversation by including a thread and a post.</span></span> 

<span data-ttu-id="3edf1-103">Use [reply thread](conversationthread_reply.md) ou [reply post](post_reply.md) para postar mais na conversa.</span><span class="sxs-lookup"><span data-stu-id="3edf1-103">Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that conversation.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3edf1-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3edf1-104">Prerequisites</span></span>
<span data-ttu-id="3edf1-105">Um dos seguintes **escopos** é necessário para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="3edf1-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="3edf1-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3edf1-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```
## <a name="request-headers"></a><span data-ttu-id="3edf1-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3edf1-107">Request headers</span></span>
| <span data-ttu-id="3edf1-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3edf1-108">Header</span></span>       | <span data-ttu-id="3edf1-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3edf1-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3edf1-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="3edf1-110">Authorization</span></span>  | <span data-ttu-id="3edf1-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3edf1-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3edf1-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3edf1-113">Content-Type</span></span>  | <span data-ttu-id="3edf1-114">application/json</span><span class="sxs-lookup"><span data-stu-id="3edf1-114">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3edf1-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3edf1-115">Request body</span></span>
<span data-ttu-id="3edf1-116">No corpo da solicitação, forneça uma representação JSON do objeto [conversation](../resources/conversation.md) que contém um [conversationThread](../resources/conversationThread.md) e um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="3edf1-116">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationThread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="3edf1-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="3edf1-117">Response</span></span>

<span data-ttu-id="3edf1-118">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3edf1-118">If successful, this method returns `201, Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3edf1-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3edf1-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3edf1-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3edf1-120">Request</span></span>
<span data-ttu-id="3edf1-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3edf1-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations
Content-type: application/json

{
  "topic": "New Conversation Topic",
  "threads": [{
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
  }]
}
```
##### <a name="response"></a><span data-ttu-id="3edf1-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="3edf1-122">Response</span></span>
<span data-ttu-id="3edf1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3edf1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->