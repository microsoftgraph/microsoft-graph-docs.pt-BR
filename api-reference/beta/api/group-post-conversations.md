---
title: Criar conversa
description: 'Crie uma nova conversa incluindo um thread e uma postagem. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: e37e84b1e0744dacc7c9cc37cefea1e9deac859a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513155"
---
# <a name="create-conversation"></a><span data-ttu-id="49845-103">Criar conversa</span><span class="sxs-lookup"><span data-stu-id="49845-103">Create conversation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49845-104">Crie uma nova [conversa](../resources/conversation.md) incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="49845-104">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="49845-105">Use [reply thread](conversationthread-reply.md) ou [reply post](post-reply.md) para postar mais na conversa.</span><span class="sxs-lookup"><span data-stu-id="49845-105">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="49845-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="49845-106">Permissions</span></span>
<span data-ttu-id="49845-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49845-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49845-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49845-109">Permission type</span></span>      | <span data-ttu-id="49845-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49845-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49845-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49845-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49845-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49845-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="49845-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49845-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49845-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49845-114">Not supported.</span></span>    |
|<span data-ttu-id="49845-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49845-115">Application</span></span> | <span data-ttu-id="49845-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49845-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49845-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49845-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="49845-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49845-118">Request headers</span></span>
| <span data-ttu-id="49845-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49845-119">Header</span></span>       | <span data-ttu-id="49845-120">Valor</span><span class="sxs-lookup"><span data-stu-id="49845-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="49845-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="49845-121">Authorization</span></span>  | <span data-ttu-id="49845-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49845-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="49845-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49845-124">Content-Type</span></span>  | <span data-ttu-id="49845-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49845-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="49845-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49845-126">Request body</span></span>
<span data-ttu-id="49845-127">No corpo da solicitação, forneça uma representação JSON do objeto [conversation](../resources/conversation.md) que contém um [conversationThread](../resources/conversationthread.md) e um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="49845-127">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="49845-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="49845-128">Response</span></span>
<span data-ttu-id="49845-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49845-129">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span> 

<span data-ttu-id="49845-130">A resposta inclui as IDs da nova conversa e do thread, que você pode usar na operação [listar postagens](conversationthread-list-posts.md) para obter a nova postagem também.</span><span class="sxs-lookup"><span data-stu-id="49845-130">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="49845-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49845-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="49845-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49845-132">Request</span></span>
<span data-ttu-id="49845-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="49845-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations
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

#### <a name="response"></a><span data-ttu-id="49845-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="49845-134">Response</span></span>
<span data-ttu-id="49845-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="49845-135">The following is an example of the response.</span></span>
><span data-ttu-id="49845-136">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="49845-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="49845-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49845-137">All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/group-post-conversations.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
