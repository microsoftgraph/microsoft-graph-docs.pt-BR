# <a name="create-thread"></a><span data-ttu-id="97e9c-101">Criar thread</span><span class="sxs-lookup"><span data-stu-id="97e9c-101">Create thread</span></span>

<span data-ttu-id="97e9c-102">Crie um novo thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="97e9c-102">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="97e9c-p101">Um thread e uma postagem são criados conforme especificado. Use [responder ao thread](conversationthread_reply.md) para incluir postagens adicionais no thread. Ou, se receber a ID de postagem, você também poderá [responder](post_reply.md) a essa postagem no thread.</span><span class="sxs-lookup"><span data-stu-id="97e9c-p101">A thread and post are created as specified. Use [reply thread](conversationthread_reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post_reply.md) to that post in that thread.</span></span>

<span data-ttu-id="97e9c-106">Observação: Você também pode [Iniciar uma nova conversa criando primeiro um thread](group_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="97e9c-106">Note: You can also [start a new conversation by first creating a thread](group_post_threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="97e9c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="97e9c-107">Permissions</span></span>
<span data-ttu-id="97e9c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97e9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97e9c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97e9c-110">Permission type</span></span>      | <span data-ttu-id="97e9c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97e9c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97e9c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97e9c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="97e9c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97e9c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="97e9c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97e9c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97e9c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97e9c-115">Not supported.</span></span>    |
|<span data-ttu-id="97e9c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97e9c-116">Application</span></span> | <span data-ttu-id="97e9c-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97e9c-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97e9c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97e9c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="97e9c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97e9c-119">Request headers</span></span>
| <span data-ttu-id="97e9c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="97e9c-120">Name</span></span>       | <span data-ttu-id="97e9c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="97e9c-121">Type</span></span> | <span data-ttu-id="97e9c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="97e9c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="97e9c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97e9c-123">Authorization</span></span>  | <span data-ttu-id="97e9c-124">string</span><span class="sxs-lookup"><span data-stu-id="97e9c-124">string</span></span>  | <span data-ttu-id="97e9c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97e9c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97e9c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97e9c-127">Request body</span></span>
<span data-ttu-id="97e9c-128">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="97e9c-128">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="97e9c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="97e9c-129">Response</span></span>

<span data-ttu-id="97e9c-130">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [ConversationThread](../resources/conversationthread.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97e9c-130">If successful, this method returns `201, Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97e9c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97e9c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97e9c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97e9c-132">Request</span></span>
<span data-ttu-id="97e9c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97e9c-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="97e9c-134">No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="97e9c-134">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="97e9c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="97e9c-135">Response</span></span>

<span data-ttu-id="97e9c-p104">Se for bem-sucedido, este método retornará um código de resposta `201, Created` e o `id` do novo thread no corpo da resposta. Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97e9c-p104">If successful, this method returns `201, Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
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
