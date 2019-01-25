---
title: 'post: reply'
description: 'Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: dfdc25b3e99c26d266631a331d7d58c73042e64b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511132"
---
# <a name="post-reply"></a><span data-ttu-id="2daf1-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="2daf1-104">post: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2daf1-p102">Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="2daf1-p102">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="2daf1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2daf1-107">Permissions</span></span>
<span data-ttu-id="2daf1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2daf1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2daf1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2daf1-110">Permission type</span></span>      | <span data-ttu-id="2daf1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2daf1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2daf1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2daf1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2daf1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2daf1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2daf1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2daf1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2daf1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2daf1-115">Not supported.</span></span>    |
|<span data-ttu-id="2daf1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2daf1-116">Application</span></span> | <span data-ttu-id="2daf1-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2daf1-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2daf1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2daf1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="2daf1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2daf1-119">Request headers</span></span>
| <span data-ttu-id="2daf1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2daf1-120">Header</span></span>       | <span data-ttu-id="2daf1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2daf1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2daf1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2daf1-122">Authorization</span></span>  | <span data-ttu-id="2daf1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2daf1-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2daf1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2daf1-125">Request body</span></span>
<span data-ttu-id="2daf1-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2daf1-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2daf1-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2daf1-127">Parameter</span></span>    | <span data-ttu-id="2daf1-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="2daf1-128">Type</span></span>   |<span data-ttu-id="2daf1-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2daf1-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2daf1-130">post</span><span class="sxs-lookup"><span data-stu-id="2daf1-130">post</span></span>|[<span data-ttu-id="2daf1-131">post</span><span class="sxs-lookup"><span data-stu-id="2daf1-131">post</span></span>](../resources/post.md)|<span data-ttu-id="2daf1-132">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="2daf1-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="2daf1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2daf1-133">Response</span></span>

<span data-ttu-id="2daf1-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2daf1-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2daf1-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2daf1-136">Example</span></span>
<span data-ttu-id="2daf1-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2daf1-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2daf1-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2daf1-138">Request</span></span>
<span data-ttu-id="2daf1-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2daf1-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "2016-10-19T10:37:00Z",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "2016-10-19T10:37:00Z",
    "lastModifiedDateTime": "2016-10-19T10:37:00Z",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "2016-10-19T10:37:00Z",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="2daf1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2daf1-140">Response</span></span>
##### <a name="response"></a><span data-ttu-id="2daf1-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2daf1-141">Response</span></span>
<span data-ttu-id="2daf1-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2daf1-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-reply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
