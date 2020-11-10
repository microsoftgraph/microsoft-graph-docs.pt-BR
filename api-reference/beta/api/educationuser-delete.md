---
title: Excluir educationUser
description: Exclua um usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e26b50d52078f7cebef30baee475639f4ef37374
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955305"
---
# <a name="delete-educationuser"></a><span data-ttu-id="3282d-103">Excluir educationUser</span><span class="sxs-lookup"><span data-stu-id="3282d-103">Delete educationUser</span></span>

<span data-ttu-id="3282d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3282d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3282d-105">Exclua um usuário.</span><span class="sxs-lookup"><span data-stu-id="3282d-105">Delete a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="3282d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3282d-106">Permissions</span></span>

<span data-ttu-id="3282d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3282d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3282d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3282d-109">Permission type</span></span>                        | <span data-ttu-id="3282d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3282d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3282d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3282d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3282d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3282d-112">Not supported.</span></span>                              |
| <span data-ttu-id="3282d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3282d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3282d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3282d-114">Not supported.</span></span>                              |
| <span data-ttu-id="3282d-115">Application</span><span class="sxs-lookup"><span data-stu-id="3282d-115">Application</span></span>                            | <span data-ttu-id="3282d-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3282d-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="3282d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3282d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3282d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3282d-118">Request headers</span></span>

| <span data-ttu-id="3282d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3282d-119">Header</span></span>        | <span data-ttu-id="3282d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3282d-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="3282d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3282d-121">Authorization</span></span> | <span data-ttu-id="3282d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3282d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3282d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3282d-124">Request body</span></span>

<span data-ttu-id="3282d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3282d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3282d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3282d-126">Response</span></span>

<span data-ttu-id="3282d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3282d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3282d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3282d-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3282d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3282d-130">Request</span></span>

<span data-ttu-id="3282d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3282d-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3282d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3282d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/users/13019
```
# <a name="c"></a>[<span data-ttu-id="3282d-133">C#</span><span class="sxs-lookup"><span data-stu-id="3282d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3282d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3282d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3282d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3282d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3282d-136">Java</span><span class="sxs-lookup"><span data-stu-id="3282d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3282d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3282d-137">Response</span></span>

<span data-ttu-id="3282d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3282d-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


