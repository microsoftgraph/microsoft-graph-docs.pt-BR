---
title: Excluir mailFolder
description: Exclua o mailFolder especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cc593576d2c31e8fdc1ca6cef822b3624dbdd952
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865570"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="9cab3-103">Excluir mailFolder</span><span class="sxs-lookup"><span data-stu-id="9cab3-103">Delete mailFolder</span></span>

<span data-ttu-id="9cab3-104">Exclua o [mailFolder](../resources/mailfolder.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="9cab3-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="9cab3-105">A pasta pode ser uma [mailSearchFolder](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9cab3-105">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="9cab3-106">Você pode especificar uma pasta de email por sua ID de pasta ou por seu [nome de pasta conhecido](../resources/mailfolder.md), se houver uma.</span><span class="sxs-lookup"><span data-stu-id="9cab3-106">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span>

><span data-ttu-id="9cab3-107">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo nome `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="9cab3-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="9cab3-108">Veja [retenção de item excluído](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="9cab3-108">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cab3-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cab3-109">Permissions</span></span>
<span data-ttu-id="9cab3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cab3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cab3-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cab3-112">Permission type</span></span>      | <span data-ttu-id="9cab3-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cab3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cab3-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cab3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9cab3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cab3-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9cab3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cab3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cab3-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cab3-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9cab3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cab3-118">Application</span></span> | <span data-ttu-id="9cab3-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9cab3-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cab3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cab3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9cab3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cab3-121">Request headers</span></span>
| <span data-ttu-id="9cab3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9cab3-122">Name</span></span>       | <span data-ttu-id="9cab3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cab3-123">Type</span></span> | <span data-ttu-id="9cab3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cab3-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9cab3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cab3-125">Authorization</span></span>  | <span data-ttu-id="9cab3-126">string</span><span class="sxs-lookup"><span data-stu-id="9cab3-126">string</span></span>  | <span data-ttu-id="9cab3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cab3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cab3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cab3-129">Request body</span></span>
<span data-ttu-id="9cab3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9cab3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cab3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cab3-131">Response</span></span>

<span data-ttu-id="9cab3-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cab3-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cab3-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cab3-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cab3-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cab3-135">Request</span></span>
<span data-ttu-id="9cab3-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cab3-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9cab3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cab3-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cab3-138">C#</span><span class="sxs-lookup"><span data-stu-id="9cab3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cab3-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cab3-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cab3-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cab3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9cab3-141">Java</span><span class="sxs-lookup"><span data-stu-id="9cab3-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9cab3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cab3-142">Response</span></span>
<span data-ttu-id="9cab3-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cab3-143">Here is an example of the response.</span></span>
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
