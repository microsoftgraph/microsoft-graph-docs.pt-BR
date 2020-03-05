---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d6eb7477f251ee51c2baa09216d5d0e87d8bf968
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456940"
---
# <a name="delete-message"></a><span data-ttu-id="efb80-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="efb80-103">Delete message</span></span>

<span data-ttu-id="efb80-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="efb80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efb80-105">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="efb80-105">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="efb80-106">Por exemplo, você pode excluir uma [menção de @](../resources/mention.md) específica do usuário especificado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="efb80-106">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="efb80-107">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo [nome](../resources/mailfolder.md) `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="efb80-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="efb80-108">Veja [retenção de item excluído](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="efb80-108">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="efb80-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="efb80-109">Permissions</span></span>
<span data-ttu-id="efb80-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efb80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efb80-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efb80-112">Permission type</span></span>      | <span data-ttu-id="efb80-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="efb80-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efb80-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efb80-114">Delegated (work or school account)</span></span> | <span data-ttu-id="efb80-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efb80-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="efb80-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efb80-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efb80-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efb80-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="efb80-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efb80-118">Application</span></span> | <span data-ttu-id="efb80-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efb80-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="efb80-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efb80-120">HTTP request</span></span>

<span data-ttu-id="efb80-121">Para excluir a mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="efb80-121">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="efb80-122">Para excluir uma [menção](../resources/mention.md) específica em uma mensagem:</span><span class="sxs-lookup"><span data-stu-id="efb80-122">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="efb80-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efb80-123">Request headers</span></span>
| <span data-ttu-id="efb80-124">Nome</span><span class="sxs-lookup"><span data-stu-id="efb80-124">Name</span></span>       | <span data-ttu-id="efb80-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="efb80-125">Type</span></span> | <span data-ttu-id="efb80-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="efb80-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="efb80-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="efb80-127">Authorization</span></span>  | <span data-ttu-id="efb80-128">string</span><span class="sxs-lookup"><span data-stu-id="efb80-128">string</span></span>  | <span data-ttu-id="efb80-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efb80-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="efb80-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efb80-131">Request body</span></span>
<span data-ttu-id="efb80-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="efb80-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efb80-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="efb80-133">Response</span></span>

<span data-ttu-id="efb80-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efb80-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efb80-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efb80-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="efb80-137">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="efb80-137">Request 1</span></span>
<span data-ttu-id="efb80-138">O primeiro exemplo exclui a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="efb80-138">The first example deletes the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="efb80-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="efb80-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="efb80-140">C#</span><span class="sxs-lookup"><span data-stu-id="efb80-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efb80-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efb80-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efb80-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efb80-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="efb80-143">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="efb80-143">Response 1</span></span>
<span data-ttu-id="efb80-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efb80-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="efb80-145">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="efb80-145">Request 2</span></span>
<span data-ttu-id="efb80-146">O próximo exemplo exclui uma determinada **menção** na mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="efb80-146">The next example deletes a certain **mention** in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="efb80-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="efb80-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
# <a name="c"></a>[<span data-ttu-id="efb80-148">C#</span><span class="sxs-lookup"><span data-stu-id="efb80-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mention-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efb80-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efb80-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mention-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efb80-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efb80-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mention-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="efb80-151">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="efb80-151">Response 2</span></span>
<span data-ttu-id="efb80-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efb80-152">Here is an example of the response.</span></span>
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
