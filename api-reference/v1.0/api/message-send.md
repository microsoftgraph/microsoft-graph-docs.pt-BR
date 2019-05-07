---
title: 'message: send'
description: Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser o rascunho de uma mensagem nova, rascunho de resposta, rascunho de resposta a todos ou
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f5f23c48bcdbbca3f28cbc5927b659d9dde66be6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612483"
---
# <a name="message-send"></a><span data-ttu-id="23a48-104">message: send</span><span class="sxs-lookup"><span data-stu-id="23a48-104">message: send</span></span>

<span data-ttu-id="23a48-p102">Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser um rascunho de mensagem nova, rascunho de resposta, rascunho de resposta a todos ou rascunho de encaminhamento. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="23a48-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="23a48-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="23a48-108">Permissions</span></span>

<span data-ttu-id="23a48-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23a48-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23a48-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23a48-111">Permission type</span></span>      | <span data-ttu-id="23a48-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23a48-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23a48-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23a48-113">Delegated (work or school account)</span></span> | <span data-ttu-id="23a48-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="23a48-114">Mail.Send</span></span>    |
|<span data-ttu-id="23a48-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23a48-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23a48-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="23a48-116">Mail.Send</span></span>    |
|<span data-ttu-id="23a48-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23a48-117">Application</span></span> | <span data-ttu-id="23a48-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="23a48-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="23a48-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23a48-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="23a48-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23a48-120">Request headers</span></span>

| <span data-ttu-id="23a48-121">Nome</span><span class="sxs-lookup"><span data-stu-id="23a48-121">Name</span></span>       | <span data-ttu-id="23a48-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="23a48-122">Type</span></span> | <span data-ttu-id="23a48-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="23a48-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="23a48-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="23a48-124">Authorization</span></span>  | <span data-ttu-id="23a48-125">string</span><span class="sxs-lookup"><span data-stu-id="23a48-125">string</span></span>  | <span data-ttu-id="23a48-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23a48-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23a48-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="23a48-128">Content-Length</span></span> | <span data-ttu-id="23a48-129">number</span><span class="sxs-lookup"><span data-stu-id="23a48-129">number</span></span> | <span data-ttu-id="23a48-130">0. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23a48-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23a48-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23a48-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="23a48-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="23a48-132">Response</span></span>

<span data-ttu-id="23a48-p105">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23a48-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23a48-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23a48-135">Example</span></span>

<span data-ttu-id="23a48-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="23a48-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="23a48-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23a48-137">Request</span></span>

<span data-ttu-id="23a48-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23a48-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="23a48-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="23a48-139">Response</span></span>

<span data-ttu-id="23a48-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23a48-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="23a48-141">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="23a48-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="23a48-142">C#</span><span class="sxs-lookup"><span data-stu-id="23a48-142">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_send-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23a48-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="23a48-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_send-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-send.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-send.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
