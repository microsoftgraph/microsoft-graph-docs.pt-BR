---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d1df6b9d9b1b01d2960c12ce7cee1a927843626f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266084"
---
# <a name="delete-message"></a><span data-ttu-id="11995-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="11995-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11995-104">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="11995-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="11995-105">Por exemplo, você pode excluir uma [menção de @](../resources/mention.md) específica do usuário especificado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="11995-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="11995-106">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo [nome](../resources/mailfolder.md) `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="11995-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="11995-107">Veja [retenção de item excluído](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="11995-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="11995-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="11995-108">Permissions</span></span>
<span data-ttu-id="11995-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11995-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11995-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11995-111">Permission type</span></span>      | <span data-ttu-id="11995-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11995-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11995-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11995-113">Delegated (work or school account)</span></span> | <span data-ttu-id="11995-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11995-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="11995-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11995-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11995-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11995-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="11995-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11995-117">Application</span></span> | <span data-ttu-id="11995-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11995-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="11995-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11995-119">HTTP request</span></span>

<span data-ttu-id="11995-120">Para excluir a mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="11995-120">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="11995-121">Para excluir uma [menção](../resources/mention.md) específica em uma mensagem:</span><span class="sxs-lookup"><span data-stu-id="11995-121">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="11995-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11995-122">Request headers</span></span>
| <span data-ttu-id="11995-123">Nome</span><span class="sxs-lookup"><span data-stu-id="11995-123">Name</span></span>       | <span data-ttu-id="11995-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="11995-124">Type</span></span> | <span data-ttu-id="11995-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="11995-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="11995-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="11995-126">Authorization</span></span>  | <span data-ttu-id="11995-127">string</span><span class="sxs-lookup"><span data-stu-id="11995-127">string</span></span>  | <span data-ttu-id="11995-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11995-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11995-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11995-130">Request body</span></span>
<span data-ttu-id="11995-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11995-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11995-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="11995-132">Response</span></span>

<span data-ttu-id="11995-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11995-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11995-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11995-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="11995-136">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="11995-136">Request 1</span></span>
<span data-ttu-id="11995-137">O primeiro exemplo exclui a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="11995-137">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="11995-138">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="11995-138">Response 1</span></span>
<span data-ttu-id="11995-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11995-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="11995-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="11995-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="11995-141">C#</span><span class="sxs-lookup"><span data-stu-id="11995-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11995-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="11995-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="11995-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="11995-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="11995-144">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="11995-144">Request 2</span></span>
<span data-ttu-id="11995-145">O próximo exemplo exclui uma determinada **menção** na mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="11995-145">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="11995-146">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="11995-146">Response 2</span></span>
<span data-ttu-id="11995-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11995-147">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="11995-148">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="11995-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="11995-149">C#</span><span class="sxs-lookup"><span data-stu-id="11995-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11995-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="11995-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="11995-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="11995-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
