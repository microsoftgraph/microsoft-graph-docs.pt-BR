---
title: Excluir educationClass
description: Exclua uma aula. Como uma aula também é um grupo universal, excluir uma aula exclui o grupo.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 84ac58abc25a8cf0d7559179692372db9e1b936a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966360"
---
# <a name="delete-educationclass"></a><span data-ttu-id="0373f-104">Excluir educationClass</span><span class="sxs-lookup"><span data-stu-id="0373f-104">Delete educationClass</span></span>

<span data-ttu-id="0373f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0373f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0373f-106">Exclua uma aula.</span><span class="sxs-lookup"><span data-stu-id="0373f-106">Delete a class.</span></span> <span data-ttu-id="0373f-107">Como uma aula também é um grupo universal, excluir uma aula exclui o grupo.</span><span class="sxs-lookup"><span data-stu-id="0373f-107">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="0373f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0373f-108">Permissions</span></span>
<span data-ttu-id="0373f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0373f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0373f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0373f-111">Permission type</span></span>      | <span data-ttu-id="0373f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0373f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0373f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0373f-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="0373f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0373f-114">Not supported.</span></span>  |
|<span data-ttu-id="0373f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0373f-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0373f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0373f-116">Not supported.</span></span>  |
|<span data-ttu-id="0373f-117">Application</span><span class="sxs-lookup"><span data-stu-id="0373f-117">Application</span></span> | <span data-ttu-id="0373f-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0373f-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0373f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0373f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0373f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0373f-120">Request headers</span></span>
| <span data-ttu-id="0373f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0373f-121">Header</span></span>       | <span data-ttu-id="0373f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0373f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0373f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0373f-123">Authorization</span></span>  | <span data-ttu-id="0373f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0373f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0373f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0373f-126">Request body</span></span>
<span data-ttu-id="0373f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0373f-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0373f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0373f-128">Response</span></span>
<span data-ttu-id="0373f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0373f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0373f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0373f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0373f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0373f-132">Request</span></span>
<span data-ttu-id="0373f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0373f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0373f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0373f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
# <a name="c"></a>[<span data-ttu-id="0373f-135">C#</span><span class="sxs-lookup"><span data-stu-id="0373f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0373f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0373f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0373f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0373f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0373f-138">Java</span><span class="sxs-lookup"><span data-stu-id="0373f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0373f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0373f-139">Response</span></span>
<span data-ttu-id="0373f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0373f-140">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


