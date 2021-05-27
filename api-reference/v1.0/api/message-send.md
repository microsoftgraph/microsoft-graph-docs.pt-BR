---
title: 'message: send'
description: Enviar um rascunho da mensagem existente.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8be54552df8acf7faa67c070e85f63f48a5c23d4
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645490"
---
# <a name="message-send"></a><span data-ttu-id="b960f-103">message: send</span><span class="sxs-lookup"><span data-stu-id="b960f-103">message: send</span></span>

<span data-ttu-id="b960f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b960f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b960f-105">Enviar um rascunho da mensagem existente.</span><span class="sxs-lookup"><span data-stu-id="b960f-105">Send an existing draft message.</span></span> 

<span data-ttu-id="b960f-106">O rascunho da mensagem pode ser um novo [rascunho](../api/user-post-messages.md), [rascunho de resposta](../api/message-createreply.md), [responder a todos os rascunhos](../api/message-createreplyall.md) ou um [rascunho de encaminhamento](../api/message-createforward.md).</span><span class="sxs-lookup"><span data-stu-id="b960f-106">The draft message can be a new message [draft](../api/user-post-messages.md), [reply draft](../api/message-createreply.md), [reply-all draft](../api/message-createreplyall.md), or a [forward draft](../api/message-createforward.md).</span></span>

<span data-ttu-id="b960f-107">Este método salva a mensagem na pasta **Itens Enviados**.</span><span class="sxs-lookup"><span data-stu-id="b960f-107">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="b960f-108">Alternativamente, [envie uma nova mensagem](../api/user-sendmail.md) em uma única operação.</span><span class="sxs-lookup"><span data-stu-id="b960f-108">Alternatively, [send a new message](../api/user-sendmail.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="b960f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b960f-109">Permissions</span></span>
<span data-ttu-id="b960f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, consulte [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b960f-p101">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b960f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b960f-112">Permission type</span></span>      | <span data-ttu-id="b960f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b960f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b960f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b960f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b960f-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b960f-115">Mail.Send</span></span>    |
|<span data-ttu-id="b960f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b960f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b960f-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b960f-117">Mail.Send</span></span>    |
|<span data-ttu-id="b960f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b960f-118">Application</span></span> | <span data-ttu-id="b960f-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b960f-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="b960f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b960f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="b960f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b960f-121">Request headers</span></span>

| <span data-ttu-id="b960f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b960f-122">Name</span></span>       | <span data-ttu-id="b960f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b960f-123">Type</span></span> | <span data-ttu-id="b960f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b960f-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b960f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b960f-125">Authorization</span></span>  | <span data-ttu-id="b960f-126">string</span><span class="sxs-lookup"><span data-stu-id="b960f-126">string</span></span>  | <span data-ttu-id="b960f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b960f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b960f-129">Content-Length</span><span class="sxs-lookup"><span data-stu-id="b960f-129">Content-Length</span></span> | <span data-ttu-id="b960f-130">number</span><span class="sxs-lookup"><span data-stu-id="b960f-130">number</span></span> | <span data-ttu-id="b960f-131">0. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b960f-131">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b960f-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b960f-132">Request body</span></span>
<span data-ttu-id="b960f-133">Como este método envia um rascunho da mensagem existente, não é necessário especificar um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b960f-133">Since this method sends an already existing draft message, specifying a request body is not necessary.</span></span>

## <a name="response"></a><span data-ttu-id="b960f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b960f-134">Response</span></span>

<span data-ttu-id="b960f-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b960f-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b960f-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b960f-137">Examples</span></span>

### <a name="example-1-send-an-existing-draft-message"></a><span data-ttu-id="b960f-138">Exemplo 1: Enviar um rascunho da mensagem existente.</span><span class="sxs-lookup"><span data-stu-id="b960f-138">Example 1: Send an existing draft message</span></span>

<span data-ttu-id="b960f-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b960f-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b960f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b960f-140">Request</span></span>

<span data-ttu-id="b960f-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b960f-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b960f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b960f-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```
# <a name="c"></a>[<span data-ttu-id="b960f-143">C#</span><span class="sxs-lookup"><span data-stu-id="b960f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b960f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b960f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b960f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b960f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b960f-146">Java</span><span class="sxs-lookup"><span data-stu-id="b960f-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b960f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b960f-147">Response</span></span>

<span data-ttu-id="b960f-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b960f-148">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

