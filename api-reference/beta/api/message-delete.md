---
title: Excluir mensagem
description: Exclua uma mensagem na caixa de correio do usuário especificado ou exclua uma relação da mensagem.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 71ab17fa25dee8c5158d5ef166de68ca934d7ae5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132813"
---
# <a name="delete-message"></a><span data-ttu-id="47e08-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="47e08-103">Delete message</span></span>

<span data-ttu-id="47e08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47e08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47e08-105">Exclua uma mensagem na caixa de correio do usuário especificado ou exclua uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="47e08-105">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="47e08-106">Por exemplo, você pode excluir uma [@menção específica](../resources/mention.md) do usuário especificado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="47e08-106">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="47e08-107">**Observação** Talvez você não consiga excluir itens na pasta de exclusões de itens recuperáveis (representado pelo [nome de pasta conhecido).](../resources/mailfolder.md) `recoverableitemsdeletions`</span><span class="sxs-lookup"><span data-stu-id="47e08-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="47e08-108">Consulte [Retenção de itens excluídos](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e Limpar itens [excluídos](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="47e08-108">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="47e08-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="47e08-109">Permissions</span></span>
<span data-ttu-id="47e08-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47e08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47e08-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47e08-112">Permission type</span></span>      | <span data-ttu-id="47e08-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47e08-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47e08-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47e08-114">Delegated (work or school account)</span></span> | <span data-ttu-id="47e08-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47e08-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="47e08-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47e08-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47e08-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47e08-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="47e08-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47e08-118">Application</span></span> | <span data-ttu-id="47e08-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47e08-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="47e08-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47e08-120">HTTP request</span></span>

<span data-ttu-id="47e08-121">Para excluir a mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="47e08-121">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="47e08-122">Para excluir uma [menção específica](../resources/mention.md) em uma mensagem:</span><span class="sxs-lookup"><span data-stu-id="47e08-122">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="47e08-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47e08-123">Request headers</span></span>
| <span data-ttu-id="47e08-124">Nome</span><span class="sxs-lookup"><span data-stu-id="47e08-124">Name</span></span>       | <span data-ttu-id="47e08-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="47e08-125">Type</span></span> | <span data-ttu-id="47e08-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="47e08-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="47e08-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="47e08-127">Authorization</span></span>  | <span data-ttu-id="47e08-128">string</span><span class="sxs-lookup"><span data-stu-id="47e08-128">string</span></span>  | <span data-ttu-id="47e08-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47e08-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47e08-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47e08-131">Request body</span></span>
<span data-ttu-id="47e08-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47e08-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47e08-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="47e08-133">Response</span></span>

<span data-ttu-id="47e08-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47e08-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47e08-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47e08-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="47e08-137">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="47e08-137">Request 1</span></span>
<span data-ttu-id="47e08-138">O primeiro exemplo exclui a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="47e08-138">The first example deletes the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="47e08-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="47e08-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="47e08-140">C#</span><span class="sxs-lookup"><span data-stu-id="47e08-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47e08-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47e08-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47e08-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47e08-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47e08-143">Java</span><span class="sxs-lookup"><span data-stu-id="47e08-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="47e08-144">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="47e08-144">Response 1</span></span>
<span data-ttu-id="47e08-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47e08-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="47e08-146">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="47e08-146">Request 2</span></span>
<span data-ttu-id="47e08-147">O próximo exemplo exclui uma determinada **menção** na mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="47e08-147">The next example deletes a certain **mention** in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="47e08-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="47e08-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
# <a name="c"></a>[<span data-ttu-id="47e08-149">C#</span><span class="sxs-lookup"><span data-stu-id="47e08-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mention-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47e08-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47e08-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mention-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47e08-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47e08-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mention-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47e08-152">Java</span><span class="sxs-lookup"><span data-stu-id="47e08-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-mention-in-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="47e08-153">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="47e08-153">Response 2</span></span>
<span data-ttu-id="47e08-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47e08-154">Here is an example of the response.</span></span>
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


