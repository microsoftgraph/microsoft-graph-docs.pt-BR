---
title: Obter educationAssignment
description: Obter as propriedades e as relações de uma atribuição.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 94f2b3c7854ed650bd262acbac02005a5c8e60bd
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992552"
---
# <a name="get-educationassignment"></a><span data-ttu-id="aac2f-103">Obter educationAssignment</span><span class="sxs-lookup"><span data-stu-id="aac2f-103">Get educationAssignment</span></span>

<span data-ttu-id="aac2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aac2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aac2f-105">Obter as propriedades e as relações de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="aac2f-105">Get the properties and relationships of an assignment.</span></span> 

<span data-ttu-id="aac2f-106">Os alunos só podem ver atribuições atribuídas a eles; professores e aplicativos com permissões de aplicativo podem ver todas as atribuições em uma classe.</span><span class="sxs-lookup"><span data-stu-id="aac2f-106">Students can only see assignments assigned to them; teachers and applications with application permissions can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="aac2f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="aac2f-107">Permissions</span></span>
<span data-ttu-id="aac2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aac2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="aac2f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aac2f-110">Permission type</span></span>      | <span data-ttu-id="aac2f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aac2f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aac2f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aac2f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aac2f-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aac2f-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="aac2f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aac2f-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="aac2f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aac2f-115">Not supported.</span></span>  |
|<span data-ttu-id="aac2f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aac2f-116">Application</span></span> | <span data-ttu-id="aac2f-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aac2f-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aac2f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aac2f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aac2f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aac2f-119">Optional query parameters</span></span>
<span data-ttu-id="aac2f-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aac2f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aac2f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aac2f-121">Request headers</span></span>
| <span data-ttu-id="aac2f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aac2f-122">Header</span></span>       | <span data-ttu-id="aac2f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="aac2f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aac2f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="aac2f-124">Authorization</span></span>  | <span data-ttu-id="aac2f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aac2f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aac2f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aac2f-127">Request body</span></span>
<span data-ttu-id="aac2f-128">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="aac2f-128">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aac2f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="aac2f-129">Response</span></span>
<span data-ttu-id="aac2f-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aac2f-130">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac2f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aac2f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="aac2f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aac2f-132">Request</span></span>
<span data-ttu-id="aac2f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aac2f-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aac2f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="aac2f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "get_educationassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/5edb6a5f-fc6b-441b-8952-bcbfc33ef0e5/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0
```
# <a name="c"></a>[<span data-ttu-id="aac2f-135">C#</span><span class="sxs-lookup"><span data-stu-id="aac2f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aac2f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aac2f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aac2f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aac2f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aac2f-138">Java</span><span class="sxs-lookup"><span data-stu-id="aac2f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aac2f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="aac2f-139">Response</span></span>
<span data-ttu-id="aac2f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aac2f-140">The following is an example of the response.</span></span> 

><span data-ttu-id="aac2f-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="aac2f-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "id": "19002",
  "addedStudentAction": "none",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "classId": "11006",
  "createdBy": {
    "user": {
      "displayName": "Shawn Hughes",
      "id": "14012",
    }
  },
  "closeDateTime": "2014-01-11T00:00:00Z",
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
  "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!0sGAoOieeE6iSj1WXCV-nYYTuh2luKRDvUVGQBLOmvYpRzc5ARnCRorRht6P3MhU/items/01N74NOEZL7P3VK22SQFDKBZ3PHVPKDVAQ",
  "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType",
      "maxPoints": 100
  },
  "instructions": {
    "content": "Answer every question correctly",
    "contentType": "Text"
  },
  "lastModifiedBy": {
    "user": {
      "displayName": "Shawn Hughes",
      "id": "14012",
    }
  },
  "lastModifiedDateTime": "2014-01-01T00:00:00Z",
  "notificationChannelUrl": null,
  "status": "assigned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
