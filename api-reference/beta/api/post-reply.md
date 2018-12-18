---
title: 'post: reply'
description: 'Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar '
author: dkershaw10
ms.openlocfilehash: 33cd99fd24dc5acfca4b96f232f748a0377d1564
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324224"
---
# <a name="post-reply"></a><span data-ttu-id="abb4c-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="abb4c-104">post: reply</span></span>

> <span data-ttu-id="abb4c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="abb4c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abb4c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="abb4c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="abb4c-p103">Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai.</span><span class="sxs-lookup"><span data-stu-id="abb4c-p103">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="abb4c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="abb4c-109">Permissions</span></span>
<span data-ttu-id="abb4c-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abb4c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abb4c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abb4c-112">Permission type</span></span>      | <span data-ttu-id="abb4c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="abb4c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abb4c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abb4c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="abb4c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abb4c-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="abb4c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abb4c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abb4c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abb4c-117">Not supported.</span></span>    |
|<span data-ttu-id="abb4c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abb4c-118">Application</span></span> | <span data-ttu-id="abb4c-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abb4c-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="abb4c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abb4c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="abb4c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abb4c-121">Request headers</span></span>
| <span data-ttu-id="abb4c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abb4c-122">Header</span></span>       | <span data-ttu-id="abb4c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="abb4c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="abb4c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="abb4c-124">Authorization</span></span>  | <span data-ttu-id="abb4c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abb4c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="abb4c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abb4c-127">Request body</span></span>
<span data-ttu-id="abb4c-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abb4c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="abb4c-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="abb4c-129">Parameter</span></span>    | <span data-ttu-id="abb4c-130">Type</span><span class="sxs-lookup"><span data-stu-id="abb4c-130">Type</span></span>   |<span data-ttu-id="abb4c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="abb4c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abb4c-132">post</span><span class="sxs-lookup"><span data-stu-id="abb4c-132">post</span></span>|[<span data-ttu-id="abb4c-133">post</span><span class="sxs-lookup"><span data-stu-id="abb4c-133">post</span></span>](../resources/post.md)|<span data-ttu-id="abb4c-134">A nova postagem que está sendo respondida.</span><span class="sxs-lookup"><span data-stu-id="abb4c-134">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="abb4c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="abb4c-135">Response</span></span>

<span data-ttu-id="abb4c-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abb4c-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abb4c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abb4c-138">Example</span></span>
<span data-ttu-id="abb4c-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="abb4c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="abb4c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abb4c-140">Request</span></span>
<span data-ttu-id="abb4c-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abb4c-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="abb4c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="abb4c-142">Response</span></span>
##### <a name="response"></a><span data-ttu-id="abb4c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="abb4c-143">Response</span></span>
<span data-ttu-id="abb4c-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abb4c-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
