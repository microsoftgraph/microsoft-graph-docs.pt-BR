---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cd91b26948ed3ecdd6c1b07b66217466e59b56d3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981597"
---
# <a name="delete-message"></a><span data-ttu-id="97d8b-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="97d8b-103">Delete message</span></span>

<span data-ttu-id="97d8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97d8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97d8b-105">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="97d8b-105">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="97d8b-106">Por exemplo, você pode excluir uma [menção de @](../resources/mention.md) específica do usuário especificado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="97d8b-106">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="97d8b-107">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo [nome de pasta conhecido](../resources/mailfolder.md) `recoverableitemsdeletions` ).</span><span class="sxs-lookup"><span data-stu-id="97d8b-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="97d8b-108">Veja [retenção de item excluído](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="97d8b-108">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="97d8b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="97d8b-109">Permissions</span></span>
<span data-ttu-id="97d8b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97d8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97d8b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97d8b-112">Permission type</span></span>      | <span data-ttu-id="97d8b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97d8b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97d8b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97d8b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="97d8b-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97d8b-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="97d8b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97d8b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97d8b-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97d8b-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="97d8b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97d8b-118">Application</span></span> | <span data-ttu-id="97d8b-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97d8b-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="97d8b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97d8b-120">HTTP request</span></span>

<span data-ttu-id="97d8b-121">Para excluir a mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="97d8b-121">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="97d8b-122">Para excluir uma [menção](../resources/mention.md) específica em uma mensagem:</span><span class="sxs-lookup"><span data-stu-id="97d8b-122">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="97d8b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97d8b-123">Request headers</span></span>
| <span data-ttu-id="97d8b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="97d8b-124">Name</span></span>       | <span data-ttu-id="97d8b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="97d8b-125">Type</span></span> | <span data-ttu-id="97d8b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="97d8b-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="97d8b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="97d8b-127">Authorization</span></span>  | <span data-ttu-id="97d8b-128">string</span><span class="sxs-lookup"><span data-stu-id="97d8b-128">string</span></span>  | <span data-ttu-id="97d8b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97d8b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97d8b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97d8b-131">Request body</span></span>
<span data-ttu-id="97d8b-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97d8b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97d8b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="97d8b-133">Response</span></span>

<span data-ttu-id="97d8b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97d8b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97d8b-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97d8b-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="97d8b-137">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="97d8b-137">Request 1</span></span>
<span data-ttu-id="97d8b-138">O primeiro exemplo exclui a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="97d8b-138">The first example deletes the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="97d8b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="97d8b-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="97d8b-140">C#</span><span class="sxs-lookup"><span data-stu-id="97d8b-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97d8b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97d8b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97d8b-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97d8b-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97d8b-143">Java</span><span class="sxs-lookup"><span data-stu-id="97d8b-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="97d8b-144">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="97d8b-144">Response 1</span></span>
<span data-ttu-id="97d8b-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97d8b-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="97d8b-146">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="97d8b-146">Request 2</span></span>
<span data-ttu-id="97d8b-147">O próximo exemplo exclui uma determinada **menção** na mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="97d8b-147">The next example deletes a certain **mention** in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="97d8b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="97d8b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
# <a name="c"></a>[<span data-ttu-id="97d8b-149">C#</span><span class="sxs-lookup"><span data-stu-id="97d8b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mention-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97d8b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97d8b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mention-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97d8b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97d8b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mention-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97d8b-152">Java</span><span class="sxs-lookup"><span data-stu-id="97d8b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-mention-in-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="97d8b-153">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="97d8b-153">Response 2</span></span>
<span data-ttu-id="97d8b-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97d8b-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


