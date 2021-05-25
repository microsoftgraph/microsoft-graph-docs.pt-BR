---
title: 'message: send'
description: Envie uma mensagem de rascunho existente.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ea24ae69c3888e31124df758bc22199bde1048ea
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645518"
---
# <a name="message-send"></a><span data-ttu-id="f5c02-103">message: send</span><span class="sxs-lookup"><span data-stu-id="f5c02-103">message: send</span></span>

<span data-ttu-id="f5c02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5c02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5c02-105">Envie uma mensagem de rascunho existente.</span><span class="sxs-lookup"><span data-stu-id="f5c02-105">Send an existing draft message.</span></span> 

<span data-ttu-id="f5c02-106">A mensagem de rascunho pode ser um novo rascunho de [mensagem,](../api/user-post-messages.md)rascunho de [resposta,](../api/message-createreply.md)rascunho de [resposta-tudo](../api/message-createreplyall.md)ou um [rascunho de encaminhamento.](../api/message-createforward.md)</span><span class="sxs-lookup"><span data-stu-id="f5c02-106">The draft message can be a new message [draft](../api/user-post-messages.md), [reply draft](../api/message-createreply.md), [reply-all draft](../api/message-createreplyall.md), or a [forward draft](../api/message-createforward.md).</span></span> 

<span data-ttu-id="f5c02-107">Este método salva a mensagem na pasta **Itens** Enviados.</span><span class="sxs-lookup"><span data-stu-id="f5c02-107">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="f5c02-108">Como alternativa, [envie uma nova mensagem](../api/user-sendmail.md) em uma única operação.</span><span class="sxs-lookup"><span data-stu-id="f5c02-108">Alternatively, [send a new message](../api/user-sendmail.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5c02-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5c02-109">Permissions</span></span>
<span data-ttu-id="f5c02-110">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f5c02-110">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="f5c02-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5c02-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5c02-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5c02-112">Permission type</span></span>      | <span data-ttu-id="f5c02-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5c02-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5c02-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5c02-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f5c02-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f5c02-115">Mail.Send</span></span>    |
|<span data-ttu-id="f5c02-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5c02-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5c02-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f5c02-117">Mail.Send</span></span>    |
|<span data-ttu-id="f5c02-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5c02-118">Application</span></span> | <span data-ttu-id="f5c02-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="f5c02-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5c02-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5c02-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="f5c02-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c02-121">Request headers</span></span>

| <span data-ttu-id="f5c02-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f5c02-122">Name</span></span>       | <span data-ttu-id="f5c02-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5c02-123">Type</span></span> | <span data-ttu-id="f5c02-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5c02-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f5c02-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5c02-125">Authorization</span></span>  | <span data-ttu-id="f5c02-126">string</span><span class="sxs-lookup"><span data-stu-id="f5c02-126">string</span></span>  | <span data-ttu-id="f5c02-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5c02-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5c02-129">Content-Length</span><span class="sxs-lookup"><span data-stu-id="f5c02-129">Content-Length</span></span> | <span data-ttu-id="f5c02-130">number</span><span class="sxs-lookup"><span data-stu-id="f5c02-130">number</span></span> | <span data-ttu-id="f5c02-131">0. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5c02-131">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5c02-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c02-132">Request body</span></span>
<span data-ttu-id="f5c02-133">Como esse método envia uma mensagem de rascunho já existente, não é necessário especificar um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5c02-133">Since this method sends an already existing draft message, specifying a request body is not necessary.</span></span>

## <a name="response"></a><span data-ttu-id="f5c02-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c02-134">Response</span></span>

<span data-ttu-id="f5c02-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c02-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5c02-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f5c02-137">Examples</span></span>
### <a name="example-1-send-an-existing-draft-message"></a><span data-ttu-id="f5c02-138">Exemplo 1: Enviar uma mensagem de rascunho existente</span><span class="sxs-lookup"><span data-stu-id="f5c02-138">Example 1: Send an existing draft message</span></span>

<span data-ttu-id="f5c02-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f5c02-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f5c02-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c02-140">Request</span></span>

<span data-ttu-id="f5c02-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5c02-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5c02-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5c02-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```
# <a name="c"></a>[<span data-ttu-id="f5c02-143">C#</span><span class="sxs-lookup"><span data-stu-id="f5c02-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5c02-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5c02-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5c02-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5c02-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5c02-146">Java</span><span class="sxs-lookup"><span data-stu-id="f5c02-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f5c02-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c02-147">Response</span></span>

<span data-ttu-id="f5c02-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c02-148">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
