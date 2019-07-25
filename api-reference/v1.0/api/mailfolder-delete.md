---
title: Excluir mailFolder
description: Exclua o mailFolder especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ab447e3e74f5ef078328d487ff06a88a74f7a899
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893104"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="75065-103">Excluir mailFolder</span><span class="sxs-lookup"><span data-stu-id="75065-103">Delete mailFolder</span></span>

<span data-ttu-id="75065-104">Exclua o [mailFolder](../resources/mailfolder.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="75065-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="75065-105">A pasta pode ser uma [mailSearchFolder](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="75065-105">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="75065-106">Você pode especificar uma pasta de email por sua ID de pasta ou por seu [nome de pasta conhecido](../resources/mailfolder.md), se houver uma.</span><span class="sxs-lookup"><span data-stu-id="75065-106">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="75065-107">**Observação** Você pode não conseguir excluir itens da pasta exclusão de itens recuperáveis (representado pelo nome `recoverableitemsdeletions`de pasta conhecido).</span><span class="sxs-lookup"><span data-stu-id="75065-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="75065-108">Veja [retenção de item excluído](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) e [limpar itens excluídos](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="75065-108">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="75065-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="75065-109">Permissions</span></span>
<span data-ttu-id="75065-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75065-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75065-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75065-112">Permission type</span></span>      | <span data-ttu-id="75065-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75065-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75065-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75065-114">Delegated (work or school account)</span></span> | <span data-ttu-id="75065-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75065-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="75065-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75065-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75065-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75065-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="75065-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75065-118">Application</span></span> | <span data-ttu-id="75065-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75065-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="75065-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75065-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="75065-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75065-121">Request headers</span></span>
| <span data-ttu-id="75065-122">Nome</span><span class="sxs-lookup"><span data-stu-id="75065-122">Name</span></span>       | <span data-ttu-id="75065-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="75065-123">Type</span></span> | <span data-ttu-id="75065-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="75065-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="75065-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="75065-125">Authorization</span></span>  | <span data-ttu-id="75065-126">string</span><span class="sxs-lookup"><span data-stu-id="75065-126">string</span></span>  | <span data-ttu-id="75065-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75065-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75065-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75065-129">Request body</span></span>
<span data-ttu-id="75065-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75065-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75065-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="75065-131">Response</span></span>

<span data-ttu-id="75065-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75065-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75065-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75065-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75065-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75065-135">Request</span></span>
<span data-ttu-id="75065-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75065-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="75065-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="75065-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="75065-138">C#</span><span class="sxs-lookup"><span data-stu-id="75065-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75065-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="75065-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="75065-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="75065-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="75065-141">Java</span><span class="sxs-lookup"><span data-stu-id="75065-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="75065-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="75065-142">Response</span></span>
<span data-ttu-id="75065-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75065-143">Here is an example of the response.</span></span> 
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
