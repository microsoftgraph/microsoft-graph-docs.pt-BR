---
title: Criar conversa
description: 'Crie uma nova conversa incluindo um thread e uma postagem. '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 8fe80c3a7d226aaa2bfa3e4834623a84aa91a940
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870095"
---
# <a name="create-conversation"></a><span data-ttu-id="90b57-103">Criar conversa</span><span class="sxs-lookup"><span data-stu-id="90b57-103">Create conversation</span></span>

> <span data-ttu-id="90b57-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="90b57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90b57-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="90b57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90b57-106">Crie uma nova [conversa](../resources/conversation.md) incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="90b57-106">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="90b57-107">Use [reply thread](conversationthread-reply.md) ou [reply post](post-reply.md) para postar mais na conversa.</span><span class="sxs-lookup"><span data-stu-id="90b57-107">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="90b57-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="90b57-108">Permissions</span></span>
<span data-ttu-id="90b57-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90b57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90b57-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90b57-111">Permission type</span></span>      | <span data-ttu-id="90b57-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90b57-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90b57-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90b57-113">Delegated (work or school account)</span></span> | <span data-ttu-id="90b57-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90b57-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="90b57-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90b57-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90b57-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90b57-116">Not supported.</span></span>    |
|<span data-ttu-id="90b57-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90b57-117">Application</span></span> | <span data-ttu-id="90b57-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90b57-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90b57-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90b57-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="90b57-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90b57-120">Request headers</span></span>
| <span data-ttu-id="90b57-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90b57-121">Header</span></span>       | <span data-ttu-id="90b57-122">Valor</span><span class="sxs-lookup"><span data-stu-id="90b57-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="90b57-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90b57-123">Authorization</span></span>  | <span data-ttu-id="90b57-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90b57-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="90b57-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="90b57-126">Content-Type</span></span>  | <span data-ttu-id="90b57-127">application/json</span><span class="sxs-lookup"><span data-stu-id="90b57-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="90b57-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90b57-128">Request body</span></span>
<span data-ttu-id="90b57-129">No corpo da solicitação, forneça uma representação JSON do objeto [conversation](../resources/conversation.md) que contém um [conversationThread](../resources/conversationthread.md) e um [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="90b57-129">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="90b57-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="90b57-130">Response</span></span>
<span data-ttu-id="90b57-131">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90b57-131">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span> 

<span data-ttu-id="90b57-132">A resposta inclui as IDs da nova conversa e do thread, que você pode usar na operação [listar postagens](conversationthread-list-posts.md) para obter a nova postagem também.</span><span class="sxs-lookup"><span data-stu-id="90b57-132">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="90b57-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90b57-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="90b57-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90b57-134">Request</span></span>
<span data-ttu-id="90b57-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90b57-135">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="90b57-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="90b57-136">Response</span></span>
<span data-ttu-id="90b57-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90b57-137">The following is an example of the response.</span></span>
><span data-ttu-id="90b57-138">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="90b57-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="90b57-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90b57-139">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
