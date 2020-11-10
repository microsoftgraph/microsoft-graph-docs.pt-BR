---
title: Excluir categoria do Outlook
description: Exclua o objeto outlookCategory especificado.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 645526a659dc7099067364cb0a7dd6d68584dec1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972883"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="26381-103">Excluir categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="26381-103">Delete Outlook category</span></span>

<span data-ttu-id="26381-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26381-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26381-105">Exclua o objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="26381-105">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26381-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="26381-106">Permissions</span></span>
<span data-ttu-id="26381-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26381-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26381-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26381-109">Permission type</span></span>      | <span data-ttu-id="26381-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26381-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26381-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26381-111">Delegated (work or school account)</span></span> | <span data-ttu-id="26381-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26381-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="26381-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26381-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26381-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26381-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="26381-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26381-115">Application</span></span> | <span data-ttu-id="26381-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26381-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="26381-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26381-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26381-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26381-118">Request headers</span></span>
| <span data-ttu-id="26381-119">Nome</span><span class="sxs-lookup"><span data-stu-id="26381-119">Name</span></span>      |<span data-ttu-id="26381-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="26381-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="26381-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="26381-121">Authorization</span></span>  | <span data-ttu-id="26381-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26381-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26381-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26381-124">Request body</span></span>
<span data-ttu-id="26381-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26381-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26381-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="26381-126">Response</span></span>

<span data-ttu-id="26381-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26381-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26381-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26381-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26381-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26381-130">Request</span></span>
<span data-ttu-id="26381-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26381-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26381-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="26381-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
# <a name="c"></a>[<span data-ttu-id="26381-133">C#</span><span class="sxs-lookup"><span data-stu-id="26381-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26381-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26381-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26381-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26381-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26381-136">Java</span><span class="sxs-lookup"><span data-stu-id="26381-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="26381-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="26381-137">Response</span></span>
<span data-ttu-id="26381-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26381-138">Here is an example of the response.</span></span>
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


