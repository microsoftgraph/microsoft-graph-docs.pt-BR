---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b0e1d62dfe82c79f154a39a18d7878636687d1af
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864667"
---
# <a name="delete-message"></a><span data-ttu-id="e9a93-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="e9a93-103">Delete message</span></span>

<span data-ttu-id="e9a93-104">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e9a93-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="e9a93-105">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo [nome](../resources/mailfolder.md) `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="e9a93-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="e9a93-106">Veja [retenção de item excluído](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e9a93-106">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9a93-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9a93-107">Permissions</span></span>
<span data-ttu-id="e9a93-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9a93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9a93-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9a93-110">Permission type</span></span>      | <span data-ttu-id="e9a93-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9a93-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9a93-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9a93-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e9a93-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9a93-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e9a93-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9a93-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9a93-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9a93-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e9a93-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9a93-116">Application</span></span> | <span data-ttu-id="e9a93-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9a93-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9a93-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9a93-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e9a93-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a93-119">Request headers</span></span>
| <span data-ttu-id="e9a93-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e9a93-120">Name</span></span>       | <span data-ttu-id="e9a93-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9a93-121">Type</span></span> | <span data-ttu-id="e9a93-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9a93-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e9a93-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9a93-123">Authorization</span></span>  | <span data-ttu-id="e9a93-124">string</span><span class="sxs-lookup"><span data-stu-id="e9a93-124">string</span></span>  | <span data-ttu-id="e9a93-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9a93-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9a93-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a93-127">Request body</span></span>
<span data-ttu-id="e9a93-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9a93-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9a93-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9a93-129">Response</span></span>

<span data-ttu-id="e9a93-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9a93-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9a93-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9a93-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9a93-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9a93-133">Request</span></span>
<span data-ttu-id="e9a93-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9a93-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e9a93-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9a93-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e9a93-136">C#</span><span class="sxs-lookup"><span data-stu-id="e9a93-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9a93-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9a93-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e9a93-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9a93-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e9a93-139">Java</span><span class="sxs-lookup"><span data-stu-id="e9a93-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e9a93-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9a93-140">Response</span></span>
<span data-ttu-id="e9a93-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9a93-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
