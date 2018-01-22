# <a name="create-conversation"></a><span data-ttu-id="64c41-101">Criar conversa</span><span class="sxs-lookup"><span data-stu-id="64c41-101">Create Conversation</span></span>
<span data-ttu-id="64c41-102">Crie uma nova [conversa](../resources/conversation.md) incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="64c41-102">Create a new conversation by including a thread and a post.</span></span> 

<span data-ttu-id="64c41-103">Use [reply thread](conversationthread_reply.md) ou [reply post](post_reply.md) para postar mais na conversa.</span><span class="sxs-lookup"><span data-stu-id="64c41-103">Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="64c41-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="64c41-104">Permissions</span></span>
<span data-ttu-id="64c41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="64c41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="64c41-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64c41-107">Permission type</span></span>      | <span data-ttu-id="64c41-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64c41-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64c41-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64c41-109">Delegated (work or school account)</span></span> | <span data-ttu-id="64c41-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c41-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="64c41-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64c41-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64c41-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64c41-112">Not supported.</span></span>    |
|<span data-ttu-id="64c41-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64c41-113">Application</span></span> | <span data-ttu-id="64c41-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64c41-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64c41-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64c41-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="64c41-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64c41-116">Request headers</span></span>
| <span data-ttu-id="64c41-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64c41-117">Header</span></span>       | <span data-ttu-id="64c41-118">Valor</span><span class="sxs-lookup"><span data-stu-id="64c41-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64c41-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="64c41-119">Authorization</span></span>  | <span data-ttu-id="64c41-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64c41-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="64c41-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64c41-122">Content-Type</span></span>  | <span data-ttu-id="64c41-123">application/json</span><span class="sxs-lookup"><span data-stu-id="64c41-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64c41-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64c41-124">Request body</span></span>
<span data-ttu-id="64c41-125">No corpo da solicitação, forneça uma representação JSON do objeto [conversation](../resources/conversation.md) que contém um [conversationThread](../resources/conversationThread.md) e um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="64c41-125">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationThread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="64c41-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="64c41-126">Response</span></span>
<span data-ttu-id="64c41-127">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64c41-127">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

<span data-ttu-id="64c41-128">A resposta inclui as IDs da nova conversa e do thread, que você pode usar na operação [listar postagens](conversationthread_list_posts.md) para obter a nova postagem também.</span><span class="sxs-lookup"><span data-stu-id="64c41-128">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread_list_posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="64c41-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64c41-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="64c41-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64c41-130">Request</span></span>
<span data-ttu-id="64c41-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64c41-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations
Content-type: application/json

{
    "topic":"New locations for this quarter",
    "threads":[
        {
            "posts":[
                {
                    "body":{
                        "contentType":"html",
                        "content":"What do we know so far?"
                    },
                    "newParticipants":[
                        {
                            "emailAddress":{
                                "name":"Adele Vance",
                                "address":"AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="64c41-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="64c41-132">Response</span></span>
<span data-ttu-id="64c41-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64c41-133">The following is an example of the response.</span></span>
><span data-ttu-id="64c41-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="64c41-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="64c41-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64c41-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
    "id":"AAQkADDVKtMlRp4Txc6k=",
    "threads@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADDVKtMlRp4Txc6k%3D')/threads",
    "threads":[
        {
            "id":"AAQkADQDarUNUq0yVGnhPFzqQ=="
        }
    ]
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