---
title: Remover educationUser de uma educationSchool
description: Exclua um usuário de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7b6e706a181e71a32f70842db07e1a33048852f3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063720"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="0fddd-103">Remover educationUser de uma educationSchool</span><span class="sxs-lookup"><span data-stu-id="0fddd-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="0fddd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fddd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fddd-105">Exclua um usuário de uma escola.</span><span class="sxs-lookup"><span data-stu-id="0fddd-105">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fddd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fddd-106">Permissions</span></span>
<span data-ttu-id="0fddd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fddd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fddd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fddd-109">Permission type</span></span>      | <span data-ttu-id="0fddd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fddd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fddd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fddd-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="0fddd-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fddd-112">Not supported.</span></span>  |
|<span data-ttu-id="0fddd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fddd-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0fddd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fddd-114">Not supported.</span></span>  |
|<span data-ttu-id="0fddd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fddd-115">Application</span></span> | <span data-ttu-id="0fddd-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fddd-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0fddd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fddd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="0fddd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fddd-118">Request headers</span></span>
| <span data-ttu-id="0fddd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fddd-119">Header</span></span>       | <span data-ttu-id="0fddd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0fddd-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0fddd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fddd-121">Authorization</span></span>  | <span data-ttu-id="0fddd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fddd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fddd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fddd-124">Request body</span></span>
<span data-ttu-id="0fddd-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0fddd-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0fddd-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fddd-126">Response</span></span>
<span data-ttu-id="0fddd-127">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="0fddd-127">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fddd-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fddd-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fddd-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fddd-129">Request</span></span>
<span data-ttu-id="0fddd-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fddd-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0fddd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fddd-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="0fddd-132">C#</span><span class="sxs-lookup"><span data-stu-id="0fddd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fddd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fddd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fddd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fddd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fddd-135">Java</span><span class="sxs-lookup"><span data-stu-id="0fddd-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0fddd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fddd-136">Response</span></span>
<span data-ttu-id="0fddd-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0fddd-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

