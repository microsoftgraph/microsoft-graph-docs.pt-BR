---
title: Remover educationUser de uma educationSchool
description: Exclua um usuário de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3dfdb0e2f0bcefefc4b4d0f6c35926cf36b08d43
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787461"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="ac1de-103">Remover educationUser de uma educationSchool</span><span class="sxs-lookup"><span data-stu-id="ac1de-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="ac1de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac1de-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac1de-105">Exclua um usuário de uma escola.</span><span class="sxs-lookup"><span data-stu-id="ac1de-105">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac1de-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac1de-106">Permissions</span></span>
<span data-ttu-id="ac1de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac1de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac1de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac1de-109">Permission type</span></span>      | <span data-ttu-id="ac1de-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac1de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac1de-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac1de-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="ac1de-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac1de-112">Not supported.</span></span>  |
|<span data-ttu-id="ac1de-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac1de-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ac1de-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac1de-114">Not supported.</span></span>  |
|<span data-ttu-id="ac1de-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac1de-115">Application</span></span> | <span data-ttu-id="ac1de-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac1de-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ac1de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac1de-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ac1de-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac1de-118">Request headers</span></span>
| <span data-ttu-id="ac1de-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac1de-119">Header</span></span>       | <span data-ttu-id="ac1de-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ac1de-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ac1de-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac1de-121">Authorization</span></span>  | <span data-ttu-id="ac1de-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac1de-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ac1de-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac1de-124">Request body</span></span>
<span data-ttu-id="ac1de-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac1de-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ac1de-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac1de-126">Response</span></span>
<span data-ttu-id="ac1de-127">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="ac1de-127">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac1de-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac1de-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac1de-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac1de-129">Request</span></span>
<span data-ttu-id="ac1de-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac1de-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac1de-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac1de-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_4"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="ac1de-132">C#</span><span class="sxs-lookup"><span data-stu-id="ac1de-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac1de-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac1de-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac1de-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac1de-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac1de-135">Java</span><span class="sxs-lookup"><span data-stu-id="ac1de-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ac1de-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac1de-136">Response</span></span>
<span data-ttu-id="ac1de-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ac1de-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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

