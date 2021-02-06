---
title: Excluir categoria do Outlook
description: Exclua o objeto outlookCategory especificado.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ca806485be224394af8f715fde26c737d8e90fd7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133084"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="28ab3-103">Excluir categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="28ab3-103">Delete Outlook category</span></span>

<span data-ttu-id="28ab3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28ab3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28ab3-105">Exclua o objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="28ab3-105">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="28ab3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="28ab3-106">Permissions</span></span>
<span data-ttu-id="28ab3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28ab3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28ab3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28ab3-109">Permission type</span></span>      | <span data-ttu-id="28ab3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28ab3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28ab3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28ab3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28ab3-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28ab3-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="28ab3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28ab3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28ab3-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28ab3-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="28ab3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28ab3-115">Application</span></span> | <span data-ttu-id="28ab3-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28ab3-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="28ab3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28ab3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="28ab3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28ab3-118">Request headers</span></span>
| <span data-ttu-id="28ab3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="28ab3-119">Name</span></span>      |<span data-ttu-id="28ab3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="28ab3-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28ab3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="28ab3-121">Authorization</span></span>  | <span data-ttu-id="28ab3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28ab3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28ab3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28ab3-124">Request body</span></span>
<span data-ttu-id="28ab3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28ab3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28ab3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="28ab3-126">Response</span></span>

<span data-ttu-id="28ab3-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28ab3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28ab3-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28ab3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28ab3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28ab3-130">Request</span></span>
<span data-ttu-id="28ab3-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28ab3-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28ab3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="28ab3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
# <a name="c"></a>[<span data-ttu-id="28ab3-133">C#</span><span class="sxs-lookup"><span data-stu-id="28ab3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28ab3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28ab3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28ab3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28ab3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28ab3-136">Java</span><span class="sxs-lookup"><span data-stu-id="28ab3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28ab3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="28ab3-137">Response</span></span>
<span data-ttu-id="28ab3-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28ab3-138">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


