---
title: Remover educationCategory
description: Remover uma educationCategory existente deste educationAssignment
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 70bde8c8549486347542ff90f9088f1c78bde14a
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992468"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="fba92-103">Remover educationCategory</span><span class="sxs-lookup"><span data-stu-id="fba92-103">Remove educationCategory</span></span>

<span data-ttu-id="fba92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fba92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fba92-105">Remover uma [educationCategory](../resources/educationcategory.md) de [um educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fba92-105">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fba92-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fba92-106">Permissions</span></span>
<span data-ttu-id="fba92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fba92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fba92-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fba92-109">Permission type</span></span>      | <span data-ttu-id="fba92-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fba92-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fba92-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fba92-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="fba92-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fba92-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="fba92-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fba92-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fba92-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fba92-114">Not supported.</span></span>  |
|<span data-ttu-id="fba92-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fba92-115">Application</span></span> | <span data-ttu-id="fba92-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fba92-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="fba92-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fba92-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fba92-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fba92-118">Request headers</span></span>
| <span data-ttu-id="fba92-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fba92-119">Header</span></span>       | <span data-ttu-id="fba92-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fba92-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fba92-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fba92-121">Authorization</span></span>  | <span data-ttu-id="fba92-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fba92-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fba92-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fba92-124">Content-Type</span></span>  | <span data-ttu-id="fba92-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fba92-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fba92-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fba92-126">Request body</span></span>
<span data-ttu-id="fba92-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="fba92-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fba92-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fba92-128">Response</span></span>
<span data-ttu-id="fba92-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fba92-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fba92-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fba92-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fba92-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fba92-131">Request</span></span>
<span data-ttu-id="fba92-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fba92-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fba92-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fba92-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ec98f158-341d-4fea-9f8c-14a250d489ac"],
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```
# <a name="c"></a>[<span data-ttu-id="fba92-134">C#</span><span class="sxs-lookup"><span data-stu-id="fba92-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-educationcategory-to-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fba92-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fba92-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-educationcategory-to-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fba92-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fba92-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-educationcategory-to-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fba92-137">Java</span><span class="sxs-lookup"><span data-stu-id="fba92-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-educationcategory-to-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fba92-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fba92-138">Response</span></span>
<span data-ttu-id="fba92-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fba92-139">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content

{
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an educationCategory from an educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


