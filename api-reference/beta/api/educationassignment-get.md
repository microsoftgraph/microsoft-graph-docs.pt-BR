---
title: Obter educationAssignment
description: " os professores podem ver todas as atribuições em uma classe."
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 28f129d1621be6a54510a8ef1dd4b48e25e2f5ff
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061711"
---
# <a name="get-educationassignment"></a><span data-ttu-id="cc034-103">Obter educationAssignment</span><span class="sxs-lookup"><span data-stu-id="cc034-103">Get educationAssignment</span></span>

<span data-ttu-id="cc034-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc034-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc034-105">Obter as propriedades e as relações de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="cc034-105">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="cc034-106">Os alunos só podem ver atribuições atribuídas a eles; professores e aplicativos com permissões de aplicativo podem ver todas as atribuições em uma classe.</span><span class="sxs-lookup"><span data-stu-id="cc034-106">Students can only see assignments assigned to them; teachers and applications with application permissions can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc034-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc034-107">Permissions</span></span>
<span data-ttu-id="cc034-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc034-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cc034-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc034-110">Permission type</span></span>      | <span data-ttu-id="cc034-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc034-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc034-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc034-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cc034-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc034-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="cc034-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc034-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cc034-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc034-115">Not supported.</span></span>  |
|<span data-ttu-id="cc034-116">Application\*</span><span class="sxs-lookup"><span data-stu-id="cc034-116">Application\*</span></span> | <span data-ttu-id="cc034-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc034-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="cc034-118">\*As permissões de aplicativo estão disponíveis apenas para clientes de visualização privada.</span><span class="sxs-lookup"><span data-stu-id="cc034-118">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="cc034-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc034-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cc034-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cc034-120">Optional query parameters</span></span>
<span data-ttu-id="cc034-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cc034-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc034-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc034-122">Request headers</span></span>
| <span data-ttu-id="cc034-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc034-123">Header</span></span>       | <span data-ttu-id="cc034-124">Valor</span><span class="sxs-lookup"><span data-stu-id="cc034-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc034-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc034-125">Authorization</span></span>  | <span data-ttu-id="cc034-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc034-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc034-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc034-128">Request body</span></span>
<span data-ttu-id="cc034-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc034-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc034-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc034-130">Response</span></span>
<span data-ttu-id="cc034-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignment](../resources/educationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc034-131">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc034-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc034-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc034-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc034-133">Request</span></span>
<span data-ttu-id="cc034-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc034-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc034-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc034-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="c"></a>[<span data-ttu-id="cc034-136">C#</span><span class="sxs-lookup"><span data-stu-id="cc034-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc034-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc034-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc034-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc034-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc034-139">Java</span><span class="sxs-lookup"><span data-stu-id="cc034-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cc034-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc034-140">Response</span></span>
<span data-ttu-id="cc034-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc034-141">The following is an example of the response.</span></span> 

><span data-ttu-id="cc034-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cc034-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "closeDateTime": "2014-01-11T00:00:00Z",
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
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
      "displayName": "Susana Rocha",
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
