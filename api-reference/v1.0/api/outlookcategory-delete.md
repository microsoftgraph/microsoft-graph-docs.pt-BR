---
title: Excluir categoria do Outlook
description: Exclua o objeto outlookCategory especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fe40adbd592c2df0a4e36f40a1b2ca643df235f5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890559"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="92c20-103">Excluir categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="92c20-103">Delete Outlook category</span></span>


<span data-ttu-id="92c20-104">Exclua o objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="92c20-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="92c20-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="92c20-105">Permissions</span></span>
<span data-ttu-id="92c20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92c20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92c20-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92c20-108">Permission type</span></span>      | <span data-ttu-id="92c20-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92c20-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92c20-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92c20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="92c20-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92c20-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="92c20-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92c20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92c20-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92c20-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="92c20-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92c20-114">Application</span></span> | <span data-ttu-id="92c20-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92c20-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="92c20-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92c20-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="92c20-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92c20-117">Request headers</span></span>
| <span data-ttu-id="92c20-118">Nome</span><span class="sxs-lookup"><span data-stu-id="92c20-118">Name</span></span>      |<span data-ttu-id="92c20-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="92c20-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92c20-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="92c20-120">Authorization</span></span>  | <span data-ttu-id="92c20-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92c20-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92c20-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92c20-123">Request body</span></span>
<span data-ttu-id="92c20-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92c20-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92c20-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="92c20-125">Response</span></span>

<span data-ttu-id="92c20-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92c20-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92c20-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92c20-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92c20-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92c20-129">Request</span></span>
<span data-ttu-id="92c20-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92c20-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="92c20-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="92c20-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92c20-132">C#</span><span class="sxs-lookup"><span data-stu-id="92c20-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92c20-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="92c20-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92c20-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="92c20-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="92c20-135">Java</span><span class="sxs-lookup"><span data-stu-id="92c20-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92c20-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="92c20-136">Response</span></span>
<span data-ttu-id="92c20-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92c20-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
