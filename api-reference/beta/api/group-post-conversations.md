---
title: Criar conversa
description: 'Crie uma nova conversa incluindo um thread e uma postagem. '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c69414b1580aff3e909c02510fbdf6cc81e22d61
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470978"
---
# <a name="create-conversation"></a><span data-ttu-id="6e570-103">Criar conversa</span><span class="sxs-lookup"><span data-stu-id="6e570-103">Create conversation</span></span>

<span data-ttu-id="6e570-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e570-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e570-105">Crie uma nova [conversa](../resources/conversation.md) incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="6e570-105">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="6e570-106">Use [reply thread](conversationthread-reply.md) ou [reply post](post-reply.md) para postar mais na conversa.</span><span class="sxs-lookup"><span data-stu-id="6e570-106">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e570-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e570-107">Permissions</span></span>
<span data-ttu-id="6e570-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e570-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e570-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e570-110">Permission type</span></span>      | <span data-ttu-id="6e570-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e570-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e570-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e570-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6e570-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e570-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e570-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e570-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e570-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e570-115">Not supported.</span></span>    |
|<span data-ttu-id="6e570-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e570-116">Application</span></span> | <span data-ttu-id="6e570-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e570-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e570-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e570-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="6e570-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e570-119">Request headers</span></span>
| <span data-ttu-id="6e570-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e570-120">Header</span></span>       | <span data-ttu-id="6e570-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6e570-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e570-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e570-122">Authorization</span></span>  | <span data-ttu-id="6e570-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e570-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e570-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e570-125">Content-Type</span></span>  | <span data-ttu-id="6e570-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e570-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e570-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e570-127">Request body</span></span>
<span data-ttu-id="6e570-128">No corpo da solicitação, forneça uma representação JSON do objeto [conversation](../resources/conversation.md) que contém um [conversationThread](../resources/conversationthread.md) e um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="6e570-128">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="6e570-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e570-129">Response</span></span>
<span data-ttu-id="6e570-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e570-130">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span> 

<span data-ttu-id="6e570-131">A resposta inclui as IDs da nova conversa e do thread, que você pode usar na operação [listar postagens](conversationthread-list-posts.md) para obter a nova postagem também.</span><span class="sxs-lookup"><span data-stu-id="6e570-131">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="6e570-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e570-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6e570-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e570-133">Request</span></span>
<span data-ttu-id="6e570-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e570-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6e570-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e570-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations
Content-type: application/json

{
  "topic":"New head count",
  "threads":[
    {
      "posts":[
        {
          "body":{
            "contentType":"html",
            "content":"The confirmation will come by the end of the week."
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
# <a name="c"></a>[<span data-ttu-id="6e570-136">C#</span><span class="sxs-lookup"><span data-stu-id="6e570-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e570-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e570-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e570-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e570-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e570-139">Java</span><span class="sxs-lookup"><span data-stu-id="6e570-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6e570-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e570-140">Response</span></span>
<span data-ttu-id="6e570-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6e570-141">The following is an example of the response.</span></span>
><span data-ttu-id="6e570-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e570-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
  "id":"AAQkADPxBgqECsrFDTuM=",
  "threads@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADPxBgqECsrFDTuM%3D')/threads",
  "threads":[
    {
      "id":"AAQkADUNO4xAAMbGA93Sw-EGCoQKysUNO4w=="
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


