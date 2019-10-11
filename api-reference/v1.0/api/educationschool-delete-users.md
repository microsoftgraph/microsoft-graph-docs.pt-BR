---
title: Remover educationUser de uma educationSchool
description: Exclua um usuário de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8ff75f7c40e1eade2b3fbfc67b16141f69b43bae
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37427890"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="41169-103">Remover educationUser de uma educationSchool</span><span class="sxs-lookup"><span data-stu-id="41169-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="41169-104">Exclua um usuário de uma escola.</span><span class="sxs-lookup"><span data-stu-id="41169-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="41169-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="41169-105">Permissions</span></span>
<span data-ttu-id="41169-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41169-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41169-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41169-108">Permission type</span></span>      | <span data-ttu-id="41169-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41169-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41169-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41169-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="41169-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41169-111">Not supported.</span></span>  |
|<span data-ttu-id="41169-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41169-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="41169-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41169-113">Not supported.</span></span>  |
|<span data-ttu-id="41169-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41169-114">Application</span></span> | <span data-ttu-id="41169-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41169-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="41169-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41169-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="41169-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41169-117">Request headers</span></span>
| <span data-ttu-id="41169-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41169-118">Header</span></span>       | <span data-ttu-id="41169-119">Valor</span><span class="sxs-lookup"><span data-stu-id="41169-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="41169-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="41169-120">Authorization</span></span>  | <span data-ttu-id="41169-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41169-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="41169-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41169-123">Request body</span></span>
<span data-ttu-id="41169-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41169-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="41169-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="41169-125">Response</span></span>
<span data-ttu-id="41169-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="41169-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="41169-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41169-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41169-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41169-128">Request</span></span>
<span data-ttu-id="41169-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41169-129">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="41169-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="41169-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="41169-131">C#</span><span class="sxs-lookup"><span data-stu-id="41169-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41169-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41169-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41169-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41169-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="41169-134">Java</span><span class="sxs-lookup"><span data-stu-id="41169-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="41169-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="41169-135">Response</span></span>
<span data-ttu-id="41169-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41169-136">The following is an example of the response.</span></span> 
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
