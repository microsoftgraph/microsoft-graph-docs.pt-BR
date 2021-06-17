---
title: Criar educationCategory
description: Cria uma nova categoria.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 943cf7abbd9a91e10249f6cafd675e6844d5b1e9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992329"
---
# <a name="create-educationcategory"></a><span data-ttu-id="2107e-103">Criar educationCategory</span><span class="sxs-lookup"><span data-stu-id="2107e-103">Create educationCategory</span></span>

<span data-ttu-id="2107e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2107e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2107e-105">Cria uma nova [educationCategory](../resources/educationcategory.md) em uma [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="2107e-105">Creates a new [educationCategory](../resources/educationcategory.md) on an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2107e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2107e-106">Permissions</span></span>
<span data-ttu-id="2107e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2107e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2107e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2107e-109">Permission type</span></span>      | <span data-ttu-id="2107e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2107e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2107e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2107e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2107e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2107e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2107e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2107e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2107e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2107e-114">Not supported.</span></span>  |
|<span data-ttu-id="2107e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2107e-115">Application</span></span> | <span data-ttu-id="2107e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2107e-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2107e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2107e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories

```
## <a name="request-headers"></a><span data-ttu-id="2107e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2107e-118">Request headers</span></span>
| <span data-ttu-id="2107e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2107e-119">Header</span></span>       | <span data-ttu-id="2107e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2107e-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2107e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2107e-121">Authorization</span></span>  | <span data-ttu-id="2107e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2107e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2107e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2107e-124">Content-Type</span></span>  | <span data-ttu-id="2107e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2107e-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2107e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2107e-126">Request body</span></span>
<span data-ttu-id="2107e-127">No corpo da solicitação, fornece uma representação JSON de um [objeto educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="2107e-127">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="2107e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2107e-128">Response</span></span>
<span data-ttu-id="2107e-129">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2107e-129">If successful, this method returns a `201 Created` response code and an [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2107e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2107e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2107e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2107e-131">Request</span></span>
<span data-ttu-id="2107e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2107e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2107e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2107e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["9a5e4047-c1dc-4243-9628-580d3c64b80c"],
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/9a5e4047-c1dc-4243-9628-580d3c64b80c/assignmentCategories
Content-type: application/json
Content-length: 33

{ 
  "displayName": "Quizzes"
}
```
# <a name="c"></a>[<span data-ttu-id="2107e-134">C#</span><span class="sxs-lookup"><span data-stu-id="2107e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationcategory-from-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2107e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2107e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationcategory-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2107e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2107e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationcategory-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2107e-137">Java</span><span class="sxs-lookup"><span data-stu-id="2107e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationcategory-from-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2107e-138">No corpo da solicitação, fornece uma representação JSON de um [objeto educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="2107e-138">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="2107e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2107e-139">Response</span></span>
<span data-ttu-id="2107e-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2107e-140">The following is an example of the response.</span></span> 

><span data-ttu-id="2107e-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2107e-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 85

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('9a5e4047-c1dc-4243-9628-580d3c64b80c')/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


