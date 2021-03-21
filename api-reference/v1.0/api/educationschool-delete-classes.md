---
title: Remover educationClass
description: Exclua uma classe de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7b71f1f104a15b1772f92717cac6136f29b2a565
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956602"
---
# <a name="remove-educationclass"></a><span data-ttu-id="b3586-103">Remover educationClass</span><span class="sxs-lookup"><span data-stu-id="b3586-103">Remove educationClass</span></span>

<span data-ttu-id="b3586-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3586-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3586-105">Exclua uma classe de uma escola.</span><span class="sxs-lookup"><span data-stu-id="b3586-105">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3586-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3586-106">Permissions</span></span>
<span data-ttu-id="b3586-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3586-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3586-109">Permission type</span></span>      | <span data-ttu-id="b3586-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3586-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3586-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3586-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="b3586-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3586-112">Not supported.</span></span>  |
|<span data-ttu-id="b3586-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3586-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b3586-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3586-114">Not supported.</span></span>  |
|<span data-ttu-id="b3586-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3586-115">Application</span></span> | <span data-ttu-id="b3586-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3586-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b3586-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3586-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b3586-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3586-118">Request headers</span></span>
| <span data-ttu-id="b3586-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3586-119">Header</span></span>       | <span data-ttu-id="b3586-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b3586-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b3586-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3586-121">Authorization</span></span>  | <span data-ttu-id="b3586-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3586-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3586-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3586-124">Request body</span></span>
<span data-ttu-id="b3586-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3586-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b3586-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3586-126">Response</span></span>
<span data-ttu-id="b3586-127">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3586-127">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3586-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3586-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3586-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3586-129">Request</span></span>
<span data-ttu-id="b3586-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3586-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3586-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3586-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_3"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```
# <a name="c"></a>[<span data-ttu-id="b3586-132">C#</span><span class="sxs-lookup"><span data-stu-id="b3586-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3586-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3586-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3586-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3586-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3586-135">Java</span><span class="sxs-lookup"><span data-stu-id="b3586-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b3586-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3586-136">Response</span></span>
<span data-ttu-id="b3586-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3586-137">The following is an example of the response.</span></span> 

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

