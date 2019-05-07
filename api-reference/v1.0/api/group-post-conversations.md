---
title: Criar conversa
description: 'Crie uma nova conversa incluindo um thread e uma postagem. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a81ae51a7fbccebd60354cf9eb659697b8e7f474
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613919"
---
# <a name="create-conversation"></a><span data-ttu-id="cab6d-103">Criar conversa</span><span class="sxs-lookup"><span data-stu-id="cab6d-103">Create conversation</span></span>
<span data-ttu-id="cab6d-104">Crie uma nova [conversa](../resources/conversation.md) incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="cab6d-104">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="cab6d-105">Use [reply thread](conversationthread-reply.md) ou [reply post](post-reply.md) para postar mais na conversa.</span><span class="sxs-lookup"><span data-stu-id="cab6d-105">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="cab6d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cab6d-106">Permissions</span></span>
<span data-ttu-id="cab6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cab6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cab6d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cab6d-109">Permission type</span></span>      | <span data-ttu-id="cab6d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cab6d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cab6d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cab6d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cab6d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cab6d-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cab6d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cab6d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cab6d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cab6d-114">Not supported.</span></span>    |
|<span data-ttu-id="cab6d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cab6d-115">Application</span></span> | <span data-ttu-id="cab6d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cab6d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cab6d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cab6d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="cab6d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cab6d-118">Request headers</span></span>
| <span data-ttu-id="cab6d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cab6d-119">Header</span></span>       | <span data-ttu-id="cab6d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cab6d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cab6d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cab6d-121">Authorization</span></span>  | <span data-ttu-id="cab6d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cab6d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cab6d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cab6d-124">Content-Type</span></span>  | <span data-ttu-id="cab6d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cab6d-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cab6d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cab6d-126">Request body</span></span>
<span data-ttu-id="cab6d-127">No corpo da solicitação, forneça uma representação JSON do objeto [conversation](../resources/conversation.md) que contém um [conversationThread](../resources/conversationthread.md) e um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="cab6d-127">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="cab6d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab6d-128">Response</span></span>
<span data-ttu-id="cab6d-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cab6d-129">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

<span data-ttu-id="cab6d-130">A resposta inclui as IDs da nova conversa e do thread, que você pode usar na operação [listar postagens](conversationthread-list-posts.md) para obter a nova postagem também.</span><span class="sxs-lookup"><span data-stu-id="cab6d-130">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="cab6d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cab6d-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cab6d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cab6d-132">Request</span></span>
<span data-ttu-id="cab6d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cab6d-133">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="cab6d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab6d-134">Response</span></span>
<span data-ttu-id="cab6d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cab6d-135">The following is an example of the response.</span></span>
><span data-ttu-id="cab6d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cab6d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cab6d-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="cab6d-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cab6d-139">Basic</span><span class="sxs-lookup"><span data-stu-id="cab6d-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_conversation_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cab6d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cab6d-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_conversation_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-conversations.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-conversations.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
