---
title: Excluir mensagem
description: Exclua uma mensagem na caixa de correio do usuário especificado ou exclua uma relação da mensagem.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c890d5574b60069de6ac305786e6e146d633a131
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130568"
---
# <a name="delete-message"></a><span data-ttu-id="ccd8b-103">Excluir mensagem</span><span class="sxs-lookup"><span data-stu-id="ccd8b-103">Delete message</span></span>

<span data-ttu-id="ccd8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccd8b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ccd8b-105">Exclua uma mensagem na caixa de correio do usuário especificado ou exclua uma relação da mensagem.</span><span class="sxs-lookup"><span data-stu-id="ccd8b-105">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="ccd8b-106">**Observação** Talvez você não consiga excluir itens na pasta de exclusões de itens recuperáveis (representado pelo [nome de pasta conhecido).](../resources/mailfolder.md) `recoverableitemsdeletions`</span><span class="sxs-lookup"><span data-stu-id="ccd8b-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="ccd8b-107">Consulte [Retenção de itens excluídos](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e Limpar itens [excluídos](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="ccd8b-107">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccd8b-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="ccd8b-108">Permissions</span></span>
<span data-ttu-id="ccd8b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccd8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccd8b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccd8b-111">Permission type</span></span>      | <span data-ttu-id="ccd8b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccd8b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccd8b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccd8b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ccd8b-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccd8b-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ccd8b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccd8b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccd8b-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccd8b-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ccd8b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccd8b-117">Application</span></span> | <span data-ttu-id="ccd8b-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccd8b-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccd8b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccd8b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ccd8b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd8b-120">Request headers</span></span>
| <span data-ttu-id="ccd8b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ccd8b-121">Name</span></span>       | <span data-ttu-id="ccd8b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccd8b-122">Type</span></span> | <span data-ttu-id="ccd8b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccd8b-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ccd8b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccd8b-124">Authorization</span></span>  | <span data-ttu-id="ccd8b-125">string</span><span class="sxs-lookup"><span data-stu-id="ccd8b-125">string</span></span>  | <span data-ttu-id="ccd8b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccd8b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccd8b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd8b-128">Request body</span></span>
<span data-ttu-id="ccd8b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ccd8b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccd8b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccd8b-130">Response</span></span>

<span data-ttu-id="ccd8b-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccd8b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccd8b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ccd8b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccd8b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd8b-134">Request</span></span>
<span data-ttu-id="ccd8b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccd8b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ccd8b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccd8b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="ccd8b-137">C#</span><span class="sxs-lookup"><span data-stu-id="ccd8b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccd8b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccd8b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccd8b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccd8b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccd8b-140">Java</span><span class="sxs-lookup"><span data-stu-id="ccd8b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ccd8b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccd8b-141">Response</span></span>
<span data-ttu-id="ccd8b-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccd8b-142">Here is an example of the response.</span></span>
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

