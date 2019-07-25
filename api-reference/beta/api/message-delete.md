---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 11cfe6f226b07b2acee3d09ac5e9e739f6df573e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879694"
---
# <a name="delete-message"></a><span data-ttu-id="c8db8-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="c8db8-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8db8-104">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c8db8-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="c8db8-105">Por exemplo, você pode excluir uma [menção de @](../resources/mention.md) específica do usuário especificado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="c8db8-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="c8db8-106">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo [nome](../resources/mailfolder.md) `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="c8db8-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="c8db8-107">Veja [retenção de item excluído](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="c8db8-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8db8-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8db8-108">Permissions</span></span>
<span data-ttu-id="c8db8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8db8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8db8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8db8-111">Permission type</span></span>      | <span data-ttu-id="c8db8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8db8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8db8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8db8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c8db8-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8db8-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c8db8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8db8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8db8-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8db8-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c8db8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8db8-117">Application</span></span> | <span data-ttu-id="c8db8-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8db8-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8db8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8db8-119">HTTP request</span></span>

<span data-ttu-id="c8db8-120">Para excluir a mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="c8db8-120">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="c8db8-121">Para excluir uma [menção](../resources/mention.md) específica em uma mensagem:</span><span class="sxs-lookup"><span data-stu-id="c8db8-121">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c8db8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8db8-122">Request headers</span></span>
| <span data-ttu-id="c8db8-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c8db8-123">Name</span></span>       | <span data-ttu-id="c8db8-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8db8-124">Type</span></span> | <span data-ttu-id="c8db8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8db8-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c8db8-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8db8-126">Authorization</span></span>  | <span data-ttu-id="c8db8-127">string</span><span class="sxs-lookup"><span data-stu-id="c8db8-127">string</span></span>  | <span data-ttu-id="c8db8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8db8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8db8-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8db8-130">Request body</span></span>
<span data-ttu-id="c8db8-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8db8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8db8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8db8-132">Response</span></span>

<span data-ttu-id="c8db8-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8db8-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8db8-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8db8-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c8db8-136">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="c8db8-136">Request 1</span></span>
<span data-ttu-id="c8db8-137">O primeiro exemplo exclui a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="c8db8-137">The first example deletes the specified message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c8db8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8db8-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c8db8-139">C#</span><span class="sxs-lookup"><span data-stu-id="c8db8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8db8-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8db8-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c8db8-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c8db8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c8db8-142">Java</span><span class="sxs-lookup"><span data-stu-id="c8db8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="c8db8-143">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="c8db8-143">Response 1</span></span>
<span data-ttu-id="c8db8-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8db8-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="c8db8-145">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="c8db8-145">Request 2</span></span>
<span data-ttu-id="c8db8-146">O próximo exemplo exclui uma determinada **menção** na mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="c8db8-146">The next example deletes a certain **mention** in the specified message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c8db8-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8db8-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c8db8-148">C#</span><span class="sxs-lookup"><span data-stu-id="c8db8-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mention-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8db8-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8db8-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mention-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c8db8-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c8db8-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mention-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c8db8-151">Java</span><span class="sxs-lookup"><span data-stu-id="c8db8-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-mention-in-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="c8db8-152">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="c8db8-152">Response 2</span></span>
<span data-ttu-id="c8db8-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8db8-153">Here is an example of the response.</span></span> 
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
