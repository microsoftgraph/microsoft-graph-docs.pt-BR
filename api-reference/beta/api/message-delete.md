---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0c221b08d895bcc19ebbb87996b8ef3c5f3c029a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598571"
---
# <a name="delete-message"></a><span data-ttu-id="535c7-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="535c7-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="535c7-104">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="535c7-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="535c7-105">Por exemplo, você pode excluir uma [menção de @](../resources/mention.md) específica do usuário especificado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="535c7-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="535c7-106">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo [nome](../resources/mailfolder.md) `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="535c7-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="535c7-107">Veja [retenção de item excluído](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="535c7-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="535c7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="535c7-108">Permissions</span></span>
<span data-ttu-id="535c7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="535c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="535c7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="535c7-111">Permission type</span></span>      | <span data-ttu-id="535c7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="535c7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="535c7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="535c7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="535c7-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="535c7-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="535c7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="535c7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="535c7-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="535c7-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="535c7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="535c7-117">Application</span></span> | <span data-ttu-id="535c7-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="535c7-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="535c7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="535c7-119">HTTP request</span></span>

<span data-ttu-id="535c7-120">Para excluir a mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="535c7-120">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="535c7-121">Para excluir uma [menção](../resources/mention.md) específica em uma mensagem:</span><span class="sxs-lookup"><span data-stu-id="535c7-121">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="535c7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="535c7-122">Request headers</span></span>
| <span data-ttu-id="535c7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="535c7-123">Name</span></span>       | <span data-ttu-id="535c7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="535c7-124">Type</span></span> | <span data-ttu-id="535c7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="535c7-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="535c7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="535c7-126">Authorization</span></span>  | <span data-ttu-id="535c7-127">string</span><span class="sxs-lookup"><span data-stu-id="535c7-127">string</span></span>  | <span data-ttu-id="535c7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="535c7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="535c7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="535c7-130">Request body</span></span>
<span data-ttu-id="535c7-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="535c7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="535c7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="535c7-132">Response</span></span>

<span data-ttu-id="535c7-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="535c7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="535c7-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="535c7-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="535c7-136">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="535c7-136">Request 1</span></span>
<span data-ttu-id="535c7-137">O primeiro exemplo exclui a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="535c7-137">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="535c7-138">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="535c7-138">Response 1</span></span>
<span data-ttu-id="535c7-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="535c7-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="535c7-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="535c7-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="535c7-141">Basic</span><span class="sxs-lookup"><span data-stu-id="535c7-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="535c7-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="535c7-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="535c7-143">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="535c7-143">Request 2</span></span>
<span data-ttu-id="535c7-144">O próximo exemplo exclui uma determinada **menção** na mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="535c7-144">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="535c7-145">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="535c7-145">Response 2</span></span>
<span data-ttu-id="535c7-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="535c7-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="535c7-147">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="535c7-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="535c7-148">Basic</span><span class="sxs-lookup"><span data-stu-id="535c7-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="535c7-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="535c7-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_mention_in_message-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
