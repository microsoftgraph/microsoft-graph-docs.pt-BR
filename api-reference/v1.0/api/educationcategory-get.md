---
title: Obter educationCategory
description: Recupere um objeto category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 97930cf5436eedf88543d6b0946559e573ff4449
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993119"
---
# <a name="get-educationcategory"></a><span data-ttu-id="a7d1a-103">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="a7d1a-103">Get educationCategory</span></span>

<span data-ttu-id="a7d1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7d1a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a7d1a-105">Recupere um [objeto educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="a7d1a-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7d1a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7d1a-106">Permissions</span></span>

<span data-ttu-id="a7d1a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7d1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a7d1a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7d1a-109">Permission type</span></span>                        | <span data-ttu-id="a7d1a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7d1a-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a7d1a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7d1a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7d1a-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7d1a-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="a7d1a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7d1a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7d1a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7d1a-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="a7d1a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7d1a-115">Application</span></span>                            | <span data-ttu-id="a7d1a-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7d1a-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7d1a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7d1a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7d1a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a7d1a-118">Optional query parameters</span></span>

<span data-ttu-id="a7d1a-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a7d1a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7d1a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7d1a-120">Request headers</span></span>
| <span data-ttu-id="a7d1a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7d1a-121">Header</span></span>        | <span data-ttu-id="a7d1a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a7d1a-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="a7d1a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7d1a-123">Authorization</span></span> | <span data-ttu-id="a7d1a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7d1a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7d1a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7d1a-126">Request body</span></span>

<span data-ttu-id="a7d1a-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="a7d1a-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7d1a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7d1a-128">Response</span></span>

<span data-ttu-id="a7d1a-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7d1a-129">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7d1a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7d1a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7d1a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7d1a-131">Request</span></span>

<span data-ttu-id="a7d1a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7d1a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7d1a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7d1a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["acdefc6b-2dc6-4e71-b1e9-6d9810ab1793"],
  "name": "get_class_category"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/96821157-5efb-4706-8ca2-a90b26c44852
```
# <a name="c"></a>[<span data-ttu-id="a7d1a-134">C#</span><span class="sxs-lookup"><span data-stu-id="a7d1a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-class-category-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7d1a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7d1a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-class-category-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7d1a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7d1a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-class-category-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7d1a-137">Java</span><span class="sxs-lookup"><span data-stu-id="a7d1a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-class-category-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a7d1a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7d1a-138">Response</span></span>

<span data-ttu-id="a7d1a-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a7d1a-139">The following is an example of the response.</span></span>

><span data-ttu-id="a7d1a-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a7d1a-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 85

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "96821157-5efb-4706-8ca2-a90b26c44852"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get category",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
