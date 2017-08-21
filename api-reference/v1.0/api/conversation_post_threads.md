# <a name="create-thread"></a><span data-ttu-id="bc0f7-101">Criar thread</span><span class="sxs-lookup"><span data-stu-id="bc0f7-101">Create thread</span></span>

<span data-ttu-id="bc0f7-102">Crie um novo thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="bc0f7-102">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="bc0f7-p101">Um thread e uma postagem são criados conforme especificado. Use [responder ao thread](conversationthread_reply.md) para incluir postagens adicionais no thread. Ou, se receber a ID de postagem, você também poderá [responder](post_reply.md) a essa postagem no thread.</span><span class="sxs-lookup"><span data-stu-id="bc0f7-p101">A thread and post are created as specified. Use [reply thread](conversationthread_reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post_reply.md) to that post in that thread.</span></span>

<span data-ttu-id="bc0f7-106">Observação: Você também pode [Iniciar uma nova conversa criando primeiro um thread](group_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="bc0f7-106">Note: You can also [start a new conversation by first creating a thread](group_post_threads.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc0f7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc0f7-107">Prerequisites</span></span>
<span data-ttu-id="bc0f7-108">Os seguintes **escopos** são necessários para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="bc0f7-108">The following **scopes** are required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="bc0f7-109">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc0f7-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="bc0f7-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc0f7-110">Request headers</span></span>
| <span data-ttu-id="bc0f7-111">Nome</span><span class="sxs-lookup"><span data-stu-id="bc0f7-111">Name</span></span>       | <span data-ttu-id="bc0f7-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc0f7-112">Type</span></span> | <span data-ttu-id="bc0f7-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc0f7-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bc0f7-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc0f7-114">Authorization</span></span>  | <span data-ttu-id="bc0f7-115">string</span><span class="sxs-lookup"><span data-stu-id="bc0f7-115">string</span></span>  | <span data-ttu-id="bc0f7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc0f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc0f7-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc0f7-118">Request body</span></span>
<span data-ttu-id="bc0f7-119">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="bc0f7-119">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bc0f7-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc0f7-120">Response</span></span>

<span data-ttu-id="bc0f7-121">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc0f7-121">If successful, this method returns `201, Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc0f7-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc0f7-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc0f7-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc0f7-123">Request</span></span>
<span data-ttu-id="bc0f7-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc0f7-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
<span data-ttu-id="bc0f7-125">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="bc0f7-125">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bc0f7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc0f7-126">Response</span></span>

<span data-ttu-id="bc0f7-p103">Se for bem-sucedido, este método retornará um código de resposta `201, Created` e o `id` do novo thread no corpo da resposta. Este é um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc0f7-p103">If successful, this method returns `201, Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
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
