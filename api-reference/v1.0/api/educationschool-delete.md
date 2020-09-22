---
title: Excluir educationSchool
description: Exclua uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 14921cfd46bb9c6ac3ac60f7f65c027e9d3bd0aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063706"
---
# <a name="delete-educationschool"></a><span data-ttu-id="8a219-103">Excluir educationSchool</span><span class="sxs-lookup"><span data-stu-id="8a219-103">Delete educationSchool</span></span>

<span data-ttu-id="8a219-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a219-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a219-105">Exclua uma escola.</span><span class="sxs-lookup"><span data-stu-id="8a219-105">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a219-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a219-106">Permissions</span></span>
<span data-ttu-id="8a219-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a219-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a219-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a219-109">Permission type</span></span>      | <span data-ttu-id="8a219-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a219-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a219-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a219-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="8a219-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a219-112">Not supported.</span></span>  |
|<span data-ttu-id="8a219-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a219-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8a219-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a219-114">Not supported.</span></span>  |
|<span data-ttu-id="8a219-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a219-115">Application</span></span> | <span data-ttu-id="8a219-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a219-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8a219-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a219-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8a219-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a219-118">Request headers</span></span>
| <span data-ttu-id="8a219-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a219-119">Header</span></span>       | <span data-ttu-id="8a219-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8a219-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a219-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a219-121">Authorization</span></span>  | <span data-ttu-id="8a219-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a219-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a219-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a219-124">Request body</span></span>
<span data-ttu-id="8a219-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a219-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8a219-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a219-126">Response</span></span>
<span data-ttu-id="8a219-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a219-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a219-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a219-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a219-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a219-130">Request</span></span>
<span data-ttu-id="8a219-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a219-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a219-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a219-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="c"></a>[<span data-ttu-id="8a219-133">C#</span><span class="sxs-lookup"><span data-stu-id="8a219-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a219-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a219-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a219-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a219-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a219-136">Java</span><span class="sxs-lookup"><span data-stu-id="8a219-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8a219-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a219-137">Response</span></span>
<span data-ttu-id="8a219-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8a219-138">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

