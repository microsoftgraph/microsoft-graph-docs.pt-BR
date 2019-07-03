---
title: Criar conversa
description: 'Crie uma nova conversa incluindo um thread e uma postagem. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f5234a380644c9b1d0ea59a7dec53cf74f56283a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456411"
---
# <a name="create-conversation"></a><span data-ttu-id="d5bb6-103">Criar conversa</span><span class="sxs-lookup"><span data-stu-id="d5bb6-103">Create conversation</span></span>
<span data-ttu-id="d5bb6-104">Crie uma nova [conversa](../resources/conversation.md) incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="d5bb6-104">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="d5bb6-105">Use [reply thread](conversationthread-reply.md) ou [reply post](post-reply.md) para postar mais na conversa.</span><span class="sxs-lookup"><span data-stu-id="d5bb6-105">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5bb6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5bb6-106">Permissions</span></span>
<span data-ttu-id="d5bb6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5bb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5bb6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5bb6-109">Permission type</span></span>      | <span data-ttu-id="d5bb6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5bb6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5bb6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5bb6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d5bb6-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5bb6-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d5bb6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5bb6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5bb6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5bb6-114">Not supported.</span></span>    |
|<span data-ttu-id="d5bb6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5bb6-115">Application</span></span> | <span data-ttu-id="d5bb6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5bb6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5bb6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5bb6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="d5bb6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bb6-118">Request headers</span></span>
| <span data-ttu-id="d5bb6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5bb6-119">Header</span></span>       | <span data-ttu-id="d5bb6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d5bb6-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d5bb6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5bb6-121">Authorization</span></span>  | <span data-ttu-id="d5bb6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5bb6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d5bb6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5bb6-124">Content-Type</span></span>  | <span data-ttu-id="d5bb6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5bb6-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d5bb6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bb6-126">Request body</span></span>
<span data-ttu-id="d5bb6-127">No corpo da solicitação, forneça uma representação JSON do objeto [conversation](../resources/conversation.md) que contém um [conversationThread](../resources/conversationthread.md) e um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="d5bb6-127">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="d5bb6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5bb6-128">Response</span></span>
<span data-ttu-id="d5bb6-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5bb6-129">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

<span data-ttu-id="d5bb6-130">A resposta inclui as IDs da nova conversa e do thread, que você pode usar na operação [listar postagens](conversationthread-list-posts.md) para obter a nova postagem também.</span><span class="sxs-lookup"><span data-stu-id="d5bb6-130">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="d5bb6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5bb6-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d5bb6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5bb6-132">Request</span></span>
<span data-ttu-id="d5bb6-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5bb6-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d5bb6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5bb6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["29981b6a-0e57-42dc-94c9-cd24f5306196"],
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5bb6-135">C#</span><span class="sxs-lookup"><span data-stu-id="d5bb6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5bb6-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="d5bb6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5bb6-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d5bb6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d5bb6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5bb6-138">Response</span></span>
<span data-ttu-id="d5bb6-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d5bb6-139">The following is an example of the response.</span></span>
><span data-ttu-id="d5bb6-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5bb6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
