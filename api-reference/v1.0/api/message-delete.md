---
title: Excluir mensagem
description: Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b944cb586b7da4580cf8242b25275e7e70e518e7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275667"
---
# <a name="delete-message"></a><span data-ttu-id="f7b30-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="f7b30-103">Delete message</span></span>

<span data-ttu-id="f7b30-104">Excluir uma mensagem na caixa de correio do usuário especificado ou excluir uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="f7b30-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="f7b30-105">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo [nome](../resources/mailfolder.md) `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="f7b30-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="f7b30-106">Veja [retenção de item excluído](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="f7b30-106">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7b30-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7b30-107">Permissions</span></span>
<span data-ttu-id="f7b30-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7b30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7b30-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7b30-110">Permission type</span></span>      | <span data-ttu-id="f7b30-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7b30-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7b30-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7b30-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7b30-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7b30-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f7b30-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7b30-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7b30-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7b30-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f7b30-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7b30-116">Application</span></span> | <span data-ttu-id="f7b30-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7b30-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7b30-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7b30-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f7b30-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b30-119">Request headers</span></span>
| <span data-ttu-id="f7b30-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f7b30-120">Name</span></span>       | <span data-ttu-id="f7b30-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7b30-121">Type</span></span> | <span data-ttu-id="f7b30-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7b30-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7b30-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7b30-123">Authorization</span></span>  | <span data-ttu-id="f7b30-124">string</span><span class="sxs-lookup"><span data-stu-id="f7b30-124">string</span></span>  | <span data-ttu-id="f7b30-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7b30-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7b30-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b30-127">Request body</span></span>
<span data-ttu-id="f7b30-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7b30-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7b30-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7b30-129">Response</span></span>

<span data-ttu-id="f7b30-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7b30-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7b30-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7b30-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7b30-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b30-133">Request</span></span>
<span data-ttu-id="f7b30-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7b30-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="f7b30-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7b30-135">Response</span></span>
<span data-ttu-id="f7b30-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7b30-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f7b30-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f7b30-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f7b30-138">C#</span><span class="sxs-lookup"><span data-stu-id="f7b30-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7b30-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7b30-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f7b30-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f7b30-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
