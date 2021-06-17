---
title: Obter educationCategory
description: Recupere um objeto category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 43e26c09b1f5c29e7c096ee0a905e5141d79191f
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991670"
---
# <a name="get-educationcategory"></a><span data-ttu-id="d9132-103">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="d9132-103">Get educationCategory</span></span>

<span data-ttu-id="d9132-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9132-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9132-105">Recupere um [objeto educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="d9132-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9132-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d9132-106">Permissions</span></span>

<span data-ttu-id="d9132-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9132-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9132-109">Permission type</span></span>                        | <span data-ttu-id="d9132-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9132-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d9132-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9132-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9132-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9132-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="d9132-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9132-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9132-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9132-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="d9132-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9132-115">Application</span></span>                            | <span data-ttu-id="d9132-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9132-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9132-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9132-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9132-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9132-118">Optional query parameters</span></span>

<span data-ttu-id="d9132-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9132-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9132-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9132-120">Request headers</span></span>
| <span data-ttu-id="d9132-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9132-121">Header</span></span>        | <span data-ttu-id="d9132-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d9132-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d9132-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9132-123">Authorization</span></span> | <span data-ttu-id="d9132-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9132-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9132-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9132-126">Request body</span></span>

<span data-ttu-id="d9132-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9132-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9132-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9132-128">Response</span></span>

<span data-ttu-id="d9132-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [educationCategory](../resources/educationcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9132-129">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9132-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9132-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d9132-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9132-131">Request</span></span>

<span data-ttu-id="d9132-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9132-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9132-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9132-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dacbf757-888d-42ae-b701-5e57cec300ae"],
  "name": "get_class_category"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/dacbf757-888d-42ae-b701-5e57cec300ae/assignmentCategories/7f64924d-4cdb-4e54-8c37-c0f3d46f0747
```
# <a name="c"></a>[<span data-ttu-id="d9132-134">C#</span><span class="sxs-lookup"><span data-stu-id="d9132-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-class-category-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9132-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9132-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-class-category-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9132-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9132-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-class-category-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9132-137">Java</span><span class="sxs-lookup"><span data-stu-id="d9132-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-class-category-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d9132-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9132-138">Response</span></span>

<span data-ttu-id="d9132-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9132-139">The following is an example of the response.</span></span>

><span data-ttu-id="d9132-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d9132-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes/dacbf757-888d-42ae-b701-5e57cec300ae/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "7f64924d-4cdb-4e54-8c37-c0f3d46f0747"
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
