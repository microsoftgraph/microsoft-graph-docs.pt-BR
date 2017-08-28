# <a name="create-conversation"></a><span data-ttu-id="6210e-101">Criar conversa</span><span class="sxs-lookup"><span data-stu-id="6210e-101">Create Conversation</span></span>

<span data-ttu-id="6210e-102">Crie uma nova conversa incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="6210e-102">Create a new conversation by including a thread and a post.</span></span> 

<span data-ttu-id="6210e-103">Use [reply thread](conversationthread_reply.md) ou [reply post](post_reply.md) para postar mais na conversa.</span><span class="sxs-lookup"><span data-stu-id="6210e-103">Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="6210e-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="6210e-104">Permissions</span></span>
<span data-ttu-id="6210e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6210e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6210e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6210e-107">Permission type</span></span>      | <span data-ttu-id="6210e-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6210e-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="6210e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6210e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6210e-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6210e-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="6210e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6210e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6210e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6210e-112">Not supported.</span></span>    | 
|<span data-ttu-id="6210e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6210e-113">Application</span></span> | <span data-ttu-id="6210e-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6210e-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6210e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6210e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```
## <a name="request-headers"></a><span data-ttu-id="6210e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6210e-116">Request headers</span></span>
| <span data-ttu-id="6210e-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6210e-117">Header</span></span>       | <span data-ttu-id="6210e-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6210e-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6210e-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6210e-119">Authorization</span></span>  | <span data-ttu-id="6210e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6210e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6210e-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6210e-122">Content-Type</span></span>  | <span data-ttu-id="6210e-123">application/json</span><span class="sxs-lookup"><span data-stu-id="6210e-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6210e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6210e-124">Request body</span></span>
<span data-ttu-id="6210e-125">No corpo da solicitação, forneça uma representação JSON do objeto [conversation](../resources/conversation.md) que contém um [conversationThread](../resources/conversationThread.md) e um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="6210e-125">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationThread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="6210e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6210e-126">Response</span></span>

<span data-ttu-id="6210e-127">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6210e-127">If successful, this method returns `201, Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6210e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6210e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6210e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6210e-129">Request</span></span>
<span data-ttu-id="6210e-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6210e-130">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6210e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6210e-131">Response</span></span>
<span data-ttu-id="6210e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6210e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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